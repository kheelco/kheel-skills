# Relations

## When to record one

Record a relation only when knowing it changes how a practitioner understands or distinguishes the terms. Every
relation has its own evidence while it is drafted, and is recorded once, on the term its kind starts from; renderings show the
inverse (*has types*, *has parts*) on the other term.

A relation has two parts:

- its **kind**: what sort of connection it is, one of the six below. The kind is the glossary's classification. It is
  what lets a reader, a review or a diagram treat relations consistently, and it implies no multiplicity.
- its **labels**: how the domain says it, in the domain's own words (*Labels*, below). The labels carry the domain
  meaning; the kind says what sort of meaning it is.

The three general kinds (*is a type of*, *is part of*, *refers to*) correspond broadly to the generic, partitive
and associative relations of terminology work (ISO 704). They describe how concepts are understood in relation to one
another, not how a system represents them.

## The kinds

Three are **general** relations between terms, of any kind, characteristics included where meaningful. Between
concepts, agents and activities they are drawn as edges on a diagram:

| Kind | Holds when | What it tells the reader |
|---|---|---|
| **is a type of** | The narrower term is a case of the broader one. Both ends are the same kind of term. | Whatever the broader term's definition and definitional rules say holds for the narrower term too. |
| **is part of** | The domain understands the part as a component of the whole: something the whole is made up of. | That the part is understood as a component of the whole. Nothing more: not that the part is exclusive to one whole, cannot be referred to from elsewhere, or ceases with the whole. Where the domain attests any of those, write it as a definitional rule on the part. |
| **refers to** | One term involves another that the domain treats as existing in its own right, and is associated with it rather than made up of it. | That the other term has its own existence and may change while this one stands. A label says what the association is. |

Three are **specialised** relations that run only from a characteristic, and are written on it rather than drawn:

| Kind | Holds when | What it tells the reader |
|---|---|---|
| **identifies** | The characteristic is a handle for its bearer. | The handle can change without the bearer becoming a different thing, and a bearer may have several. |
| **captures** | The characteristic is another term's characteristic **as it stood at a named moment**. | Later changes to the source do not change what this one means: it is a record of what was so, not a view of what is so. Always name the moment. |
| **is derived from** | The characteristic's meaning is defined in terms of others. | It follows from its sources by the rule its definition states. It adds no independent information about the domain; if it disagrees with its sources, one of them is wrong. |

*Captures* and *is derived from* are about meaning, not storage. Whether a system stores the captured value, rebuilds it
from history or computes the derived value on demand is a design question, not a glossary one.

All six remain subject to their tests and to the glossary's scope.

**Characteristics and the general kinds.** *Is a type of* applies to characteristics as readily as to concepts:
*Holder identifier* has types *CSN*, *HIN* and *SRN*, and the base's *identifies Shareholder* holds for each. *Is part
of* and *refers to* may also run from a characteristic, but apply the usual test first: does the relation materially
clarify what the characteristic means?

- *Street*, *City* and *Postcode* could be described as parts of an *Address*. Record that only when it clarifies what
  an address is in this domain; otherwise breaking a characteristic into its components is attribute modelling, and
  belongs to domain modelling.
- *Approval status* might refer to an *Approval decision*. Record it where the association is genuinely part of the
  characteristic's meaning. First ask whether the characteristic needs a clearer definition, or whether it really
  *captures* something of the decision as it stood at a moment.

**A bearer is not a relation.** A characteristic's **Of** names its bearer: the term it is a property of. That is not a
*refers to*, and does not imply one; record a *refers to* from a characteristic only for an association beyond being
its bearer's property.

*Refers to* and *captures* are the pair most often confused, and the same two terms often carry both: an invoice
*refers to* its customer (who is liable) and has a billing address that *captures* the customer's address as at issue
(where it was sent). The reference outlives the accuracy of the capture, and that is the point.

Do not invent relation kinds to carry what a label can say: the lightness of six kinds is deliberate.

## Labels

A kind names the sort of connection in the glossary's vocabulary; a label says it the way the domain does. A label
takes one of two forms.

**A reading** is a phrase that connects the two terms as a practitioner would say it, in either direction, whichever
way the kind runs:

- *Line item is part of Invoice*, read from the whole: "an Invoice **has at least one** Line item".
- *Invoice refers to Customer*: "the Customer **is liable to pay** the Invoice".
- *Department is part of Company*: "a Company **is organised into** Departments".

**A role** is a noun phrase naming what the other term is, seen from the term the relation is recorded on, the way a
practitioner would name a property of it:

- *Use case refers to Actor*, role **primary actor**: "the use case's primary actor".
- *Use case refers to Actor*, role **secondary actors (optional)**: a second relation between the same pair.
- *Company refers to Director*, role **directors**.

A relation may have both a reading and a role, and may have neither when the kind and the two definitions say it all
(*CSN is a type of Holder identifier* needs no label). Give every *refers to* a label unless the association is
self-evident from the two definitions: *refers to* on its own says only that the other term exists in its own right.

### What labels may say

- **The domain's words.** A label quotes or closely follows how practitioners say it, using glossary terms. It is a
  claim like any other, with its own evidence status.
- **Multiplicity and optionality, when the domain states them.** The kinds imply none, but a label may carry "at least
  one", "exactly one", "optional" or a plural when that is how the domain says it, because then it is part of the
  meaning: *an Invoice has at least one Line item*. Stated in a label, it is a definitional claim, not repeated under
  **Must hold**. Never add multiplicity the domain did not state because it seems obvious; if you infer it, mark it
  inferred.
- **A label can make more than one claim.** "An Invoice has at least one Line item" asserts a relation and a minimum.
  Where a label states multiplicity, optionality or another constraint, confirm that claim independently of the
  relation itself: evidence that lines are part of invoices is not evidence that every invoice has one. If only the
  relation is established, keep the constraint out of the label, or mark it (in a draft) or note it as open (in the
  agreed glossary).
- **One association per relation.** Two different associations between the same pair are two relations, each with
  its own label (a use case's primary actor and its secondary actors; an order's customer who placed it and the
  customer to deliver to).

### The label does not decide the kind

The same words can label different kinds. "Has at least one" labels *is part of* in "an Invoice has at least one Line
item" and *refers to* in "a Contract has at least two Parties". "Has" covers both. Decide the kind by the test below,
then label it in the domain's words. If one label recurs across many relations, it may be naming a term the glossary
is missing (*Holding*, between shareholder and share).

### Is part of, or refers to?

Ask: **is the other thing understood as a component of the whole, or as something independently associated with
it?** The question is about how the domain understands the connection, not about whether the part has an identity of
its own: a department has its own name and head and is still part of an organisation.

| Statement | Relation | Why |
|---|---|---|
| A company has departments | Department *is part of* Company | The company is organised into its departments; they are its components. |
| A company has shareholders | Company *refers to* Shareholder, role *shareholders* | Shareholders are associated with the company through what they hold, not components of it. |
| A company has directors | Company *refers to* Director, role *directors* | A director holds an office in the company; the board, not the company, is what the directors make up (Director *is part of* Board, if the domain speaks of it so). |
| An invoice has line items | Line item *is part of* Invoice, reading "has at least one" | The lines are what the invoice is made of. |
| A use case has a primary actor | Use case *refers to* Actor, role *primary actor* | The actor exists apart from any use case; the role says what it is to this one. |

## Not recorded here

- **Multiplicity and optionality the domain does not state.** Working them out is domain modelling, where the
  evidence supports it.
- **Participation in activities** (*performed by*, *acts on*). Activity modelling.
- **Lifecycle and state transitions.** Domain modelling.
- **Aggregation versus composition.** *Is part of* covers the domain's sense of parthood; any stronger commitment is
  a definitional rule with its evidence, or a later modelling decision.

## Worked: an invoice

| Term | Kind | Relations |
|---|---|---|
| Invoice | Concept | refers to Customer, reading "the Customer is liable to pay the Invoice" |
| Line item | Concept | is part of Invoice, reading "an Invoice has at least one Line item"; refers to Product, role *product charged for* |
| Customer | Agent | |
| Product | Concept | |
| Product code | Characteristic of Product | identifies Product |
| Customer address | Characteristic of Customer | |
| Billing address | Characteristic of Invoice | captures Customer address, as at issue |
| Unit price | Characteristic of Product | |
| Charged price | Characteristic of Line item | captures Unit price, as at issue |
| Quantity | Characteristic of Line item | |
| Line amount | Characteristic of Line item | is derived from Charged price and Quantity |
| Invoice subtotal | Characteristic of Invoice | is derived from the Line amounts of its line items |

The example leaves out tax, discounts and other adjustments to keep it small; in a domain that has them, they are
further characteristics and further sources of each derivation. A derivation names **all** of its sources: one that
names only some of them records an incomplete definition as if it were complete.

Notes on the choices:

- *Line item is part of Invoice* says no more than that lines make up an invoice. "At least one" is in the reading
  because the accounts team says an invoice with no lines is not an invoice. If they also say a line has no existence
  apart from its invoice, that becomes a definitional rule on *Line item*, attested to them. An auditor citing a
  single line does not contradict it.
- *Product code* is a characteristic because the domain only speaks of it as Product's code; a product can be re-coded
  without becoming another product. In a domain that manages codes in their own right (a classification authority),
  it could well be a concept.
- The subtotal, the codes and the addresses could each have been given a box. Keeping them as characteristics of the
  term they describe keeps the diagram about the four things the domain actually talks about.
