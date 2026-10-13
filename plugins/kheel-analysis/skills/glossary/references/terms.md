# Terms

## Kinds of term

Each term has a kind. The kind says which other artefacts will cite it and which relations make sense for it. It is
a classification of how the term is used **in this domain**, not of what the thing intrinsically is: the same word
may be a concept in one glossary and a characteristic in another.

| Kind | What it names | Examples |
|---|---|---|
| **Agent** | Someone or something that acts: a role, an organisation, a body, an external system | *Director*, *Registrar*, *Auditor* |
| **Concept** | A thing the domain talks about in its own right | *Invoice*, *Special resolution*, *Annual return*, *Share class* |
| **Activity** | An act or process the domain names as a thing in its own right, usually with a noun | *Audit*, *Settlement*, *Onboarding*, *Annual general meeting* |
| **Characteristic** | Something this glossary describes as a property of another term: a state, a quality, a handle, an amount | *Fully paid* (of a share), *Holder identifier* (of a shareholder), *Holding balance* (of a shareholding) |

**Nouns beget activities.** Most of what a domain does is said as a verb on one of its nouns: *pass a special
resolution*, *file an annual return*, *transfer shares*. The glossary holds the nouns (*Special resolution*, *Annual
return*, *Share*); the doing belongs to activity modelling, where jobs and their steps are written as a verb and a
glossary noun. Do not coin activity terms by turning those verbs into entries (*Passing a special resolution*). Record
an activity term only when the domain names the act itself, as something it talks about in its own right: an *Audit* is
scheduled, scoped and signed off; a *Settlement* can fail; an *Onboarding* is in progress.

**Act or product.** Many domain words name both an act and what the act produces: an *audit* is the examination and
the report it ends in; a *transfer* is an act and the instrument that records it; a *settlement* is a process and the
agreement it reaches. That is polysemy, and it is the commonest one. When the domain talks about both senses, record
each as its own term, qualified so its kind is plain (*Audit* the activity, *Audit report* the document), each not to
be confused with the other. When it only ever talks about one, record that one and say in its notes which sense it is;
when the act is only ever spoken of as a verb on the product, record the product alone (*Special resolution*, a
concept) and leave the act to activity modelling.

**Concept or characteristic.** A useful heuristic is identity: if you can point at two and say they are different
ones, it is probably a concept. Treat that as indicative, not decisive. *Address*, *Qualification* or *Status* may be
a property of something in one domain and a thing with its own definition, rules and relations in another. Ask what
the domain needs to say about it: if it is only ever spoken of as what some other term is or has, it is a
characteristic of that term; once the domain talks about it in its own right, it is a concept. A characteristic that
gains relations does not have to be promoted; promote it when the domain treats it as a thing.

**Activities**, where the glossary has them, are recorded as vocabulary: their word, definition, boundaries, types and
parts. Who performs them, what they act on and in what order belong to activity modelling. A definition may still
mention participants in words (*An independent examination of a company's financial statements by an auditor…*),
using glossary terms, but the glossary records no participant relations.

**Unsettled kind.** If the kind cannot be settled, record the likeliest kind and put the question in the term's notes.
A term whose kind keeps flipping is often two terms. There is no catch-all kind: a term of art that seems to fit none
(*Down round*, *Waterfall*) usually names a concept or an activity once you ask what it is in this domain.

## What a term says

Every term has a **summary**: the row of the glossary table that defines it. Many terms need nothing more. A term with
more to say also has a full **entry**, which repeats the summary fields and adds the detail fields, so the whole term
reads in one place (see [format](format.md)).

**Summary** (in the row, and repeated in the entry)

| Field | |
|---|---|
| **Term** | The preferred word or phrase, singular, in the form and casing the domain uses. Required. |
| **Synonyms** | Other words for it, each with who uses it and, where scoped, at which setting. |
| **Kind** | Agent, concept, activity or characteristic. Required. |
| **Of** | Characteristics only: the term it is a property of (its bearer). Required for a characteristic. |
| **Definition** | One or two sentences in the domain's language: what kind of thing it is and what sets it apart. No screens, features, tables or technology. Required. |
| **Example** | A concrete instance a practitioner would recognise. |
| **Relations** | Each naming its kind, the other term and, where needed, its labels: a reading or a role in the domain's words ([relations](relations.md)). |

**Detail** (in the entry only)

| Field | |
|---|---|
| **Not to be confused with** | Its near neighbours, each with the line that separates them. The field most often left empty and the one that pays back most. |
| **Must hold** | Definitional rules, if any ([rules and variation](rules-and-variation.md)). Most terms have none. |
| **Governed by** | Contextual domain rules and the instruments that set them, referenced rather than restated. |
| **Variation** | Where it is absent, called differently or governed by different rules, by setting, if anywhere. Never a different meaning ([rules and variation](rules-and-variation.md)). |
| **Domain** | The sub-domain that owns its meaning, only where one glossary covers several (below). |
| **Source** | Where the word and its meaning came from: a document, a role, a regulation; or *coined*, with why. |
| **Notes** | Open questions (including claims kept although not yet confirmed), unresolved competing definitions, decisions taken (such as the choice of preferred term), and anything handed to other analysis. |

Leave a field out rather than filling it to look complete; an absent example is a gap the review counts.

When the glossary is synced with an external system, every term has an entry, and the entry carries that system's
**id**, **version** and **lastUpdated** in a YAML block of its own (see [format](format.md), *Syncing*). A glossary that
is not synced has no IDs: a term is identified by its preferred word.

## Evidence

Evidence attaches to **claims**, not to entries. A term makes several: its word, its definition, its kind, its
example, each relation, each rule, each synonym, each variation. Each is **attested** (a source or practitioner says
so), **inferred** (concluded from evidence; say from what) or **proposed** (a modelling choice awaiting agreement), and
they are established independently: a term may have an attested definition, a proposed kind and an inferred relation.

Evidence is working state, tracked while terms are **drafted**:

- In a draft, mark each term by the status of its definition, because the definition is what the term is for, and
  mark every other claim whose status differs ([format](format.md), *Drafts*).
- An attested definition never vouches for the rest of the term. Before relying on a claim (citing it, deriving a
  diagram from it, building on it), read its own status.
- An attested claim has a source; an inferred one says what it was inferred from; a proposed one says who has to agree.

The **agreed glossary** carries no status. A term joins it when the user agrees it. **Agreement establishes what the
glossary says, not what the evidence establishes**: a practitioner can agree that an inferred relation belongs in the
glossary without confirming that it is true. Where an agreed claim remains materially uncertain, keep its evidential
basis and the uncertainty in the term's notes as an open question (*Open: inferred from the sample invoices that it is
the customer's address as at issue; confirm with the accounts team*), so the doubt stays visible without a status on
every term. The term's **Source** keeps where its meaning came from.

## The preferred term

A glossary entry represents **one domain meaning**, designated by its preferred term. Several words may designate the
same meaning (synonymy), and one word may designate different meanings (polysemy). The preferred term identifies the
entry for practical purposes; it is not the meaning itself. That is why a rename changes the designation and leaves the
meaning alone, a merge finds two designations of one meaning, and a split finds two meanings behind one designation.

Where several words compete, choose the one practitioners use, not the one the product team likes or that is easier to
code, and let the rest point to it as synonyms. Record who uses each other word, and where, so a reader arriving with
it finds the term. The choice is a decision: note it, because whoever used the other word will question it.

Since the preferred word is the term's identity (unless the glossary is synced), other artefacts cite a term by it,
and a renamed term keeps its old word as a synonym so those citations still land.

**Check for collisions first.** Before introducing a preferred word, adding a synonym, or keeping an old word as a
synonym after a rename, split or merge, check whether that word already names another term, as its preferred word or as
one of its synonyms. If it does, the word is ambiguous: resolve it by qualifying one or both uses (*Billing account*,
*Access account*), or by scoping the synonym to who uses it, and record each term as not to be confused with the other.
Never leave one word pointing at two terms unmarked.

## Domains and collisions

A glossary usually lives in a folder that stands for its domain, and that folder is every term's **home domain**: no
field needed. A glossary in a sub-folder belongs to a sub-domain: it inherits the terms of the glossary above it and
may specialise them with *is a type of*. Use the **Domain** field only when one glossary covers several sub-domains.

A **collision** is a sub-domain using a name it already inherited with a meaning of its own. It is found, not declared:
the hierarchy and the names reveal it. The rule: **the narrower sense must be a case of the broader.** Where it is, the
sub-domain has specialised and should record the type relation. Where it is not, one of the two is misnamed; qualify
one (*Billing account*, *Access account*) and record each as not to be confused with the other.

## Errors to watch for

- **Defining by the system.** *A Candidate is a record in the ATS.* The domain had candidates before it had an ATS.
- **Circularity.** *A Placement is when a candidate is placed.* A definition that uses its own term, or leans on an
  undefined one, defines nothing.
- **Hidden polysemy.** One term whose examples do not all fit its definition: the word is doing two jobs.
- **Hidden synonymy.** Two terms whose definitions differ only in wording: two teams' words for one thing.
- **Characteristic with no bearer.** *Fully paid*, of what?
- **Forced classification.** A term pushed into concept or characteristic by the identity test alone, against how the
  domain speaks of it.
- **Inferred structure presented as fact.** A type or part relation drawn from similar wording and agreed into the
  glossary without anyone confirming it.
- **Specialising for a setting.** *NZ special resolution* and *AU special resolution* as two terms, when the
  resolution means the same and only its rules differ.
- **Varying a meaning.** The opposite error: one term whose definition is quietly different in some setting. A
  different meaning is a different term.
- **Act and product in one term.** *Audit* defined as the examination in one sentence and the report in the next.
- **Verbs turned into entries.** *Passing a special resolution* as a term, when the domain only ever says *pass* a
  special resolution. The noun is the term; the act belongs to activity modelling.
- **Over-definition.** Defining ordinary words with ordinary meanings. If nobody in the domain would disagree about
  it, it needs no entry.
- **Swallowed detail.** Multiplicity the domain never stated, lifecycle states, full attribute lists, participants or
  system behaviour written into terms. They belong to later work.
