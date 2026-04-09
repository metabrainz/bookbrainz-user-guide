# Author

[TOC]

## What is an Author?
An author is someone who writes, translates or provides a story
In BookBrainz the "[entity](../../getting-started.md#what-is-an-entity-in-bookbrainz)" "Author" is basically any person who performs any number of book-related roles: writing, drawing, compiling, commissioning, even people who are [just related to two or more other authors may be eligible](#what-about-people-who-have-not-written-anything)
Generally they will fall into these 3 types:

## Types of Authors:

#### Person
This is the most common type of Author entity, used for individual people.
Before adding a new Author, always check if there is already an entry in the database for them (make sure to check not only the main author name but also any [pen names](#pen-names), aliases and common misspellings).
In general, try to add as much identifying information as possible and also add a [disambiguation](../disambiguation.md). This is required if another author with the same name exists, but it is always a good idea to add disambiguations, because it makes it easier for users to make sure they are choosing the right author."
Try to create short, concise disambiguations.
Examples: "18th century novelist", "19th century Belgian playwright" or "Nigerian Africanfuturist writer"

#### Group
Use this for groups of Authors, like [collective pseudonyms](https://en.wikipedia.org/wiki/Category:Collective_pseudonyms) (pseudonyms used by multiple individuals), [house pseudonyms](https://en.wikipedia.org/wiki/Pen_name#Collective_names) (owned by a publisher and used by the writers working for them) and the like.
Examples:
- [Ellery Queen](https://bookbrainz.org/author/a2532a57-11fa-43d4-aa5d-c2892a2d0320), the group pseudonym of *Frederic Dannay* and *Manfred Bennington Lee* used for their [series of the same name](https://bookbrainz.org/series/a807a7e6-6704-48a1-b53c-fee9860b4f2d).
- [James S. A. Corey](https://bookbrainz.org/author/c5c71242-f54c-4327-9510-a81064a9a852) pen name used by *Daniel Abraham* and *Ty Franck* for [*The Expanse* series](https://bookbrainz.org/series/c190a1c3-5391-41da-8473-c2bbec5df9a1).
- [Carolyn Keene](https://bookbrainz.org/author/25da6396-c97b-44a0-b684-33c09deb34fd) is a group pseudonym of ghost writers used by the [Stratemeyer Syndicate](https://bookbrainz.org/publisher/24818507-c14c-404e-b04c-a052bc0244a2) to publish the [Nancy Drew mystery stories](https://bookbrainz.org/series/9d4c7f75-ebdb-4f68-a54e-fc38ff414f50) and others.
- The [lettering](https://en.wikipedia.org/wiki/Letterer) studio [AndWorld Design](https://bookbrainz.org/author/9268a7af-2f90-49d8-91a1-9684620aaae9)

#### Persona
Sometimes Authors create characters and also write under that name, whilst giving this character things like a backstory or have them appear in their work.
This is different from regular pen names in that a Persona is presented as its own thing, not just a character *in* the story, but also as the writer of the work in question. [^1]
Examples:
The writer [Daniel Handler](https://bookbrainz.org/author/394ac1e3-69e8-4eed-afaa-bb06f877c96e) who writes under the pseudonym *Lemony Snicket*, a character and the supposed author of [*A Series of Unfortunate Events*](https://bookbrainz.org/series/abc21a37-600e-4e4f-9fbc-8839249fcdb9).

#### Pen Names
We do not add pen names as separate authors, instead we use [author credits](#author-credits) to show how an edition was credited with another name. 
(Note: an illustration would be good here)
Additionally, an alias [link to section about aliases] matching the pen name should also be added to the author entity.
Examples:
[Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) has aliases *Richard Bachman* and *Beryl Evans*, and is credited as such when appropriate.

### What about people who have not written anything?
Authors can also be created for people who are relevant to the data, but have not written anything themselves. For example, a person about whom several biographies have been written can be added to BookBrainz and be linked to the biographies with [link to the appropriate relationship doc].
Another case where an entry can be added is where it is needed to link 2 or more Author entities (for example, to link a grandparent to a grandchild). [^2]

Additionally, there are many other roles an "Author (entity)" can have in BookBrainz: Photographer, penciller, translator, illustrator, and so on (see section below)

## What if a Work doesn't *have* a known author?
There are special-purpose authors for these specific cases:

- *Anonymous writer*. If a work cannot be attributed to a specific writer
(e.g. published anonymously or writer attribution has been irrecoverably lost)
it should be related to
[[anonymous]](https://bookbrainz.org/author/fd47e471-a994-4ed9-bf52-531d5f184dd3).
- *Unknown writer*. If the author of a work is currently unknown, but can
potentially be determined at a later date, it should be related to
[[unknown]](https://bookbrainz.org/author/6c1b8f55-4c7e-4739-bfa2-1979da4c68e1). 
- *Oral tradition*. If a work has been preserved in the oral tradition (e.g.
received, preserved and transmitted orally from one generation to another) it
should be related to
[[traditional]](https://bookbrainz.org/author/415a1f7c-a793-4107-9f2f-c38caf15116d).

**Note** that special-purpose authors should _not_ be created villy-nilly, but be agreed upon by the community and the style-monkey

## Author Credits
This section explains about author credits.

When entering books into BookBrainz, it's important to understand the difference between the concept of an <u>Edition</u>, the physical item you can hold in your hands, and the literary concept of <u>Works</u> that books contain. (see also [Wikipedia](https://en.wikipedia.org/wiki/Creative_work) for more information.)
To illustrate the difference, see these two Editions which contain the same underlying Work, the novel [The Handmaid’s Tale](https://bookbrainz.org/work/f23d22e8-11ba-440a-a990-075152266c21): this [mass market paperback](https://bookbrainz.org/edition/a70f9eb1-b19b-4467-8f6b-c96c4616d829) published by [Seal Books](https://bookbrainz.org/publisher/e8b15024-7b26-4258-9d32-9367890b8a6d), and this [hardcover edition](https://bookbrainz.org/edition/c5d0a3e0-0eb6-4f07-b9f4-5d49a6819524) published by [Heinemann](https://bookbrainz.org/publisher/62754764-fcbd-469a-8ee1-579ccc7747b4).

BookBrainz is a _relational database_ that tracks the links between different entities, such as which <u>Author</u> (entity) wrote which <u>Work</u> (entity) and so on. But it is also a database of _credited_ information, that is, who is _credited_ as the author.
For the relational part, we use _relationships_ in the database, typically, an "\[Author\] wrote \[Work\]" relationship.

Examples:

1. [Rogues](https://bookbrainz.org/edition/6c051f2b-3d49-4e07-9282-eeb85dd35655) is a short story collection edited by [George R. R. Martin](https://bookbrainz.org/author/8b0b4bfa-16c4-48f1-bd45-b416a3ca420b) and [Gardner Dozois](https://bookbrainz.org/author/b87edc09-87ec-4d92-b589-fec1cea47a63).
It contains stories by 21 authors, but on the cover of the book the most prominent names are "George R. R. Martin & Gardner Dozois", with 6 other authors' names appearing in smaller lettering (original stories by...).
      - This is where Author Credits come in: here the Edition of [*Rogues* ](https://bookbrainz.org/edition/6c051f2b-3d49-4e07-9282-eeb85dd35655) is *credited to* [George R. R. Martin](https://bookbrainz.org/author/8b0b4bfa-16c4-48f1-bd45-b416a3ca420b) & [Gardner Dozois](https://bookbrainz.org/author/b87edc09-87ec-4d92-b589-fec1cea47a63) following the cover.
      - The 6 other authors named on the cover as well as the other 15 authors represented in the book do not appear in the Author Credits.
2. The children's book [*Charlie the Choo-Choo*](https://bookbrainz.org/edition/dd16f9d9-3ee1-436e-a0b2-a216377e93ef) was published by [Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) under the [pen name](#pen-names) "Beryl Evans".
      - The Edition is *credited to* [Beryl Evans](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) (links to the Stephen king entry)
      - The Work entity [*Charlie the Choo-Choo*](https://bookbrainz.org/work/b0b5f6d7-39e7-4515-924b-974277593f54) contained in the Edition has the relationship "was written by [Stephen King]((https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5))"


[^1]: c.f. https://community.metabrainz.org/t/pen-names-as-aliases-or-as-separate-entries/497086
[^2]: c.f https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16
