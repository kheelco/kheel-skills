# Format, rendering and where it lives

## The glossary document

The glossary is one Markdown document (or one per sub-domain, for a large glossary, each in its sub-domain's folder)
in two parts:

- **the summary**: a table with a row per term, holding what defines it (its word and synonyms, kind, definition and
  example, and relations), with related things combined into a cell so the table stays narrow. For many readers it is
  the whole glossary.
- **the entries**: a full entry for each term that has more to say than its row (boundaries, rules, variation, source,
  notes), and for every term when the glossary is synced. An entry **repeats what the row says** and adds the rest, so a
  reader has the whole term in one place without moving back and forth.

Where a term has an entry, the entry is authoritative and its row is a summary of it: change the entry, then bring
the row into line in the same edit. A row and an entry that disagree are a defect.

Every other shape (a list, a diagram, an external system's pages) is rendered from this document.

````markdown
# Billing glossary

One or two paragraphs of orientation: the domain in scope, who it was elicited from, what is deliberately out.

## Terms

| Term | Kind | Definition | Relations |
|---|---|---|---|
| **[Billing address](#billing-address)** | Characteristic of Invoice | The address the invoice was sent to. | captures Customer address — as at issue |
| **Customer** | Agent | A person or organisation that buys goods or services and is liable to pay for them.<br>*e.g.* Harbour Joinery Ltd. | |
| **[Invoice](#invoice)**<br>*also* "Bill" (customers); "Tax invoice" (Australia) | Concept | A demand for payment, issued to a customer, for goods or services supplied, itemising what is charged.<br>*e.g.* Invoice 4471 to Harbour Joinery for March's timber deliveries. | refers to Customer — reads: the Customer is liable to pay the Invoice |
| **Line item** | Concept | One charge on an invoice: a product supplied, in a quantity, at a price.<br>*e.g.* 40 lengths of 90×45 pine at $12.50. | is part of Invoice — reads: an Invoice has at least one Line item<br>refers to Product — role: product charged for |

## Entries

### Billing address

- **Kind:** Characteristic
- **Of:** Invoice
- **Definition:** The address the invoice was sent to.
- **Relations:**
  - captures Customer address — as at issue
- **Source:** Sample invoices from the accounts team.
- **Notes:** Open: inferred from the sample invoices that it is the customer's address as at issue; confirm with the
  accounts team.

### Invoice

- **Synonyms:** "Bill" (customers); "Tax invoice" (Australia)
- **Kind:** Concept
- **Definition:** A demand for payment, issued to a customer, for goods or services supplied, itemising what is
  charged.
- **Example:** Invoice 4471 to Harbour Joinery for March's timber deliveries.
- **Relations:**
  - refers to Customer — reads: the Customer is liable to pay the Invoice
- **Not to be confused with:**
  - Quote — offers a price before anything is supplied; an invoice demands payment for what has been.
  - Statement — summarises what is owed across invoices; it demands nothing new.
- **Variation (Jurisdiction):**
  - Australia: terminology differs ("Tax invoice" where GST is charged)
- **Source:** Accounts team workshop, 2026-03-02.

## Dimensions

| Dimension | Settings |
|---|---|
| Jurisdiction | New Zealand, Australia |
````

There is no document-level front matter: what a term needs travels with its entry (see *Syncing*).

### The summary table

Four columns, terms in alphabetical order:

| Column | Holds |
|---|---|
| **Term** | The preferred word in bold, linked to its entry if it has one. Then, on a new line (`<br>`), its synonyms after *also*: `"word" (who or where)`, separated by `;`. |
| **Kind** | Agent, Concept or Activity; for a characteristic, `Characteristic of <bearer>`. |
| **Definition** | The definition. Then, on a new line, an example after *e.g.*, if there is one. |
| **Relations** | One relation per line (`<br>` between them): `<kind> <Term>`, optionally followed by ` — ` and its labels, `reads: <phrase>` and/or `role: <noun phrase>`, separated by `; `. The kind is one of the six in [relations](relations.md), lower case. A *captures* names its moment: `captures Customer address — as at issue`. |

Relations are written once, on the term they start from; the inverse (*has parts*, *has types*) is never written.
Terms named in relations, in *Of*, and in boundaries use the exact preferred word of another term; one not yet in the
table is a placeholder. A table cell cannot contain `|` or a line break other than `<br>`.

### The entries

`## Entries` holds a `###` section per term that has one, headed by its preferred word, in the same order as the
table. Directly under the heading comes the entry's YAML block, when it has one (see *Syncing*). Then a bullet list
of every field in [terms](terms.md) that applies, summary fields first and in that order, written `**Name:**`:

- **Synonyms**, **Kind**, **Of**, **Definition**, **Example** and **Relations** say exactly what the row says, in the
  same notation (relations as a nested list, one per line).
- **Not to be confused with** is a nested list of `<Term or word> — <the line between them>`.
- **Variation** is one field per dimension, `**Variation (Jurisdiction):**`, with a nested list
  `<Setting>: <what differs>`, using the property names in [rules and variation](rules-and-variation.md) (*absent*,
  *terminology differs*, *rules differ*). Dimensions and their settings are declared in `## Dimensions`.
- Open questions in **Notes** start with *Open:*, so they can be found and counted.

A large glossary may group the table and the entries under `##` headings by sub-domain, with an alphabetical index;
better still, split it into one document per sub-domain folder.

### Drafts

A draft (terms harvested from an interview, a first pass over an area) has the same shape, kept apart from the agreed
glossary: a separate document beside it (`glossary.draft.md`), or just the console. In a draft, the definition ends
with the status of the definition, `[attested]`, `[inferred]` or `[proposed]`, and any other claim (a kind, a
relation, an example) whose status differs ends with its own mark, in the row and the entry alike. Inferred and
proposed marks say from what, or awaiting whom, in the term's notes. When the user agrees terms into the glossary,
they move across without their marks (see [terms](terms.md), *Evidence*).

## Syncing

A glossary that is not synced has no IDs; each term is identified by its preferred word, and renames keep the old word
as a synonym. Only when the glossary is synced with an external system that holds a glossary natively does each term
carry:

- **id**: the external system's identifier for the term;
- **version**: the external system's version of the term, as last pulled or pushed;
- **lastUpdated**: the external system's last-modified time, or its ETag where it gives one, for optimistic locking.

Every term of a synced glossary has an entry, and these go in the entry's own YAML block, directly under its heading,
as its front matter:

````markdown
### Invoice

```yaml
id: 8f3c2a
version: 7
lastUpdated: 2026-10-02T04:11:09Z
```

- **Synonyms:** "Bill" (customers); "Tax invoice" (Australia)
- **Kind:** Concept
…
````

The block travels with the entry, so a rename, a reorder or a move to another sub-domain's document carries its
binding along. Where the sync mechanism prescribes other names or a document-level binding as well, follow it; where a
platform skill for it is available (for example `page-sync`), it says how a push and a pull go.

**Never invent an id, version or timestamp.** A term without them has not been seen by the external system yet, and
the push assigns them: its entry has no YAML block until then. Before editing a synced document, check whether it is
behind its source; before pushing, check each term's version or ETag against the source so a change made there is not
overwritten.

## Rendering

**Default to the console.** Someone asking what a word means, or whether two words are the same, wants an answer they
can argue with, not a file.

| Shape | Good for |
|---|---|
| **A list** | Term and definition, one line each, alphabetical. The lookup shape. |
| **The summary table** | The glossary as most readers need it, and what a diagram is drawn from. |
| **Summary and entries** | The whole glossary document: for analysts and for review. |
| **A boundary table** | Term, definition, not to be confused with. The review shape: boundaries side by side. |
| **A variation table** | Terms down, settings across, what differs in each cell. For any question that begins "in which markets…". |
| **A diagram** | Derived, never drawn from scratch (below). |
| **Part of a specification** | A *Terms* section ahead of the actors and use cases, so the rest is read with the vocabulary in hand. |

## Deriving a diagram

Mermaid (`classDiagram` or `flowchart`) is the default notation unless the project uses another.

1. **Choose the terms to place**: a handful the perspective is about, with agents where the view needs them.
2. **Fill in from the glossary.** Every *is a type of*, *is part of* and *refers to* between placed boxes becomes an
   edge, labelled with its reading where it has one (otherwise its kind), with any role written at the far end. Every
   characteristic whose bearer is placed becomes a line inside the bearer's box, annotated with its relation where it
   has one: *captures Customer address, as at issue*; *derived from Charged price and Quantity*; *identifies Product*;
   and any general relation it has, the same way (*part of Address*, *type of Holder identifier*).
3. **Draw no multiplicity of your own.** Show it only where a label states it, in the label's words.
4. **Add the commentary**: why these terms, what the view shows that the table does not, and which relation on it is
   the one people get wrong.

A placed term that refers to one not placed shows the referent as a plain box with no characteristics, or leaves the
edge off and says so. Never widen the selection silently. A diagram that needs something the glossary does not say is
a finding: fix the glossary, not the picture.

**A set of diagrams across a glossary.** The cuts are a judgement; the grounds, in order:

- **Sub-domain is the first cut.** A diagram rarely crosses one usefully.
- **A whole stays with its parts**, and a type hierarchy with its base (a diagram of its own past three or so types).
- ***Refers to* is where to cut.** The referent has its own existence, so it can be drawn elsewhere and appear here as
  a plain box.
- **Five to nine boxes.** Fewer says nothing the table did not; more and nobody reads it.
- **Each diagram is about something.** Name its central term and give it a line of orientation. A diagram that is
  merely "the rest" means the cuts are wrong.

A term may appear on several diagrams, but one is its home, where its characteristics are written out; elsewhere it is
a plain box. List the terms that appear on no diagram: activities, which are not drawn here, or a gap.

## Where it lives

The console is where the glossary is argued into shape. Where it is kept after that is a separate decision.

- **A document in the project**, in the folder that stands for its domain (for example `specs/concept/`); ask if that
  is not evident. Diagrams go after the entries, each with its commentary, or in separate documents the glossary links
  to.
- **An external system that holds a glossary natively.** Elicitation stays in the console; the result is pushed when
  settled and pulled back when work resumes.
- **Both: a local document synced with an external system**, as in *Syncing*.

Whatever the shape, keep **synonyms pointing** at their preferred term, keep the **kind on every relation**, keep every
**characteristic naming its bearer**, and keep **not to be confused with** intact: it is the part that turns a word
list into a language.
