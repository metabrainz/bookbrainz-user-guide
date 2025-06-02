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
Use this for groups of Authors, like [collective pseudonyms](https://en.wikipedia.org/wiki/Category:Collective_pseudonyms) (pseudonyms used by multiple individuals), [house pseudonyms](https://en.wikipedia.org/wiki/Pen_name#Collective_names) (owned by a publisher and used by the writers working for them) and similar.
Examples:
[Ellery Queen](https://bookbrainz.org/author/a2532a57-11fa-43d4-aa5d-c2892a2d0320), the group pseudonym of *Frederic Dannay* and *Manfred Bennington Lee* used for their [series of the same name](https://bookbrainz.org/series/a807a7e6-6704-48a1-b53c-fee9860b4f2d).
[James S. A. Corey](https://bookbrainz.org/author/c5c71242-f54c-4327-9510-a81064a9a852) pen name used by *Daniel Abraham* and *Ty Franck* for [*The Expanse* series](https://bookbrainz.org/series/c190a1c3-5391-41da-8473-c2bbec5df9a1).
[Carolyn Keene](https://bookbrainz.org/author/25da6396-c97b-44a0-b684-33c09deb34fd) is a group pseudonym of ghost writers used by the [Stratemeyer Syndicate](https://bookbrainz.org/publisher/24818507-c14c-404e-b04c-a052bc0244a2) to publish the [Nancy Drew mystery stories](https://bookbrainz.org/series/9d4c7f75-ebdb-4f68-a54e-fc38ff414f50) and others.

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
These non-writer people can be to be added as <u>Authors</u>, despite not having written anything themselves.

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

## Author Credits
This section explains about author credits.

When entering books into BookBrainz, it's important to understand the difference between the concept of an <u>Edition</u>, the physical item you can hold in your hands, and the literary concept of <u>Works</u> that books contain. (see also [Wikipedia](https://en.wikipedia.org/wiki/Creative_work) for more information.)
To illustrate the difference, see these two Editions which contain the same underlying Work, the novel [The Handmaid’s Tale](https://bookbrainz.org/work/f23d22e8-11ba-440a-a990-075152266c21): this [mass market paperback](https://bookbrainz.org/edition/a70f9eb1-b19b-4467-8f6b-c96c4616d829) published by [Seal Books](https://bookbrainz.org/publisher/e8b15024-7b26-4258-9d32-9367890b8a6d), and this [hardcover edition](https://bookbrainz.org/edition/c5d0a3e0-0eb6-4f07-b9f4-5d49a6819524) published by [Heinemann](https://bookbrainz.org/publisher/62754764-fcbd-469a-8ee1-579ccc7747b4)

BookBrainz is a _relationable database_ that tracks the links between different entities, such as, which <u>Author</u> (entity) actually wrote what <u>Work</u> (entity) and so on. But it also is a database of _credited_ information, that is, who is _credited_ as the author.
For the relationable part, we use _relationships_ in the database, typically, an "\[Author\] wrote \[Work\]" relationship.

Examples:

1. [Rogues](https://bookbrainz.org/edition/6c051f2b-3d49-4e07-9282-eeb85dd35655) is a short story collection edited by [George R. R. Martin](https://bookbrainz.org/author/8b0b4bfa-16c4-48f1-bd45-b416a3ca420b) and [Gardner Dozois](https://bookbrainz.org/author/b87edc09-87ec-4d92-b589-fec1cea47a63).
It contains stories by 21 authors, but on the cover of the book the most prominent names are "George R. R. Martin & Gardner Dozois", with 6 other authors' names appearing in smaller lettering (original stories by...).
      - This is where Author Credits come in: here the Edition of [*Rogues* ](https://bookbrainz.org/edition/6c051f2b-3d49-4e07-9282-eeb85dd35655) is *credited to* [George R. R. Martin](https://bookbrainz.org/author/8b0b4bfa-16c4-48f1-bd45-b416a3ca420b) & [Gardner Dozois](https://bookbrainz.org/author/b87edc09-87ec-4d92-b589-fec1cea47a63) following the cover.
      - The 6 other authors named on the cover as well as the other 15 authors represented in the book do not appear in the Author Credits.
2. The children's book [*Charlie the Choo-Choo*](https://bookbrainz.org/edition/dd16f9d9-3ee1-436e-a0b2-a216377e93ef) was published by [Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) under the [pen name](#pen-names) "Beryl Evans".
      - The Edition is *credited to* [Beryl Evans](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) (links to the Stephen king entry)
      - The Work entity [*Charlie the Choo-Choo*](https://bookbrainz.org/work/b0b5f6d7-39e7-4515-924b-974277593f54) contained in the Edition has the relationship "was written by [Stephen King]((https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5))"


## Current Author-linking relationships are:

 1. **Other Authors**
      * **persona**
         (see [above](#persona)) links an Author to their persona.
      * **member of group**
         * **founder**
            (link a person as founder of a group of authors)
         * **subgroup**
            (links a collective as a sub-group to another collective)
      * **marriage**
         (link two authors as married, Note: [non-authors might be eligible here](#what-about-people-who-have-not-written-anything))
      * **involved with**
         (link two authors as involved, see above note)
      * **parent**
         (link an author as being the parent to another, see above note)
      * **sibling relations**
         (link two (or more) authors as being siblings. Take care to link everyone to everyone else!, see above note)
      * **obsolete relationships**, if you see any author with these you are encouraged to fix them!:
         * <del>collaboration</del>
            obsolete, we encourage people to fix old relationships and to use [author credits](#author-credits) and to create collectives (groups) for more permanent collaborations instead.
         * <del>pen name</del>
            obsolete, (see [above](#persona))
2. **Works**
   Works are the conceptional part of writing! (See [about Works](work.md) for more information)
    * **wrote**
        links an author to a work they've written
         Note: Several authors can be linked to the same work, and naturally an author can be linked to several works
        * **provided story**
          links an author to a work they provided the story for
           this is used for translated works, because while the author *wrote* the original story, this translated work wasn't *literally* written by them
        * **translated**
         links an author to a work they have translated from its original language
          Note: the translator should be linked to the *translated* work, not the original work.
          Example: [Taylor Engel](https://bookbrainz.org/author/9b76929e-9967-49ed-a838-e1e23464f00f) is a prolific Japanese to English translator
        * **was previously attributed to**
          links an author to a work they've previously been attributed to writing
           this is used for mostly historical works, where new research finds that so and such author was not actually the one who wrote it (add [example])
    * **worked on**
        links an Author to a work they have worked on in some miscellaneous way
        * **adapted**
          links an author to a work they have adapted ([see Wikipedia for more information about adaptions](https://en.wikipedia.org/wiki/Adaptation_(arts))
           Note: you should also add a work-work "adaptation of" link between the Original Work and the Adapted Work [(see the Work page)](./work.md#links-to-other-works)
        * **revised**
          links an author to a work they have revised ([see Wikipedia for more information about revisions](https://en.wikipedia.org/wiki/Revision_(writing))
           Note: you should also add a work-work "revision of" link between the Original Work and the Revised Work [(see the Work page)](./work.md#links-to-other-works)
        * **reconstructed**
          links an author to a work they have reconstructed [link to wikipedia that explains reconstructions].
           Note: you should also add a work-work "reconstruction of" link between the Original Work and the Reconstructed Work [(see the Work page)](./work.md#links-to-other-works)
    * **artist**
      rtists are people with roles that encompass all artistic work *except* writing. (see [#what-about-people-who-have-not-written-anything](#what-about-people-who-have-not-written-anything))
      ote: while these are not writers, they are still added with "add author" [link to how to add author page we don't yet have]
        * **photographer**
          links a photographer to a work they have provided photography for.
         Note: you should only add photographers to *Works* when their photography is intrinsically part of the Work, that is, if the story makes just as much sense without it, you should instead link them to the *Edition* [^7])
        * **illustrator**
          (links an illustrator to a work they have illustrated)
           Note: you should only add illustrators to *works* when their illustrations are intrinsically part of the work, that is, if the story makes just as much sense without it, you should instead link them to the (see below) *edition*)
        * **penciller**
          (links a penciller to a work they have pencilled, this is used ostencibly for comics, manga and graphic novels)
        * **inker**
          (links an inker to a work they have inked, ostencibly comics, manga and graphic novels)
        * **colourist**
          (links a colourist to a work they have coloured, this is used ostensibly for comics, manga and graphic novels)
        * **letterer**
          (links a letterer to a work they have provided letters for, this is used ostensibly in comics, manga and graphic novels)
          Example: [Abigail Blackman](https://bookbrainz.org/author/6a41c5d8-96fa-475a-8795-769ac22cf8b4)
    * **other**
        (link authors (people) in some other, unspecified or not-yet available relation (also see [how to suggests changes aka JIRA tickets] and [community discussion])).
        * **commissioner**
          (link someone to the work they have commissioned [see Wikipedia for more information about Commissions](https://en.wikipedia.org/wiki/Commission_(art)))
        * **dedication**
          (links a work to an author it contains a dedication to) (see [Wikipedia](https://en.wikipedia.org/wiki/Dedication_(publishing)) )
            * (note about [marriage](https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16) applies here as well)
        * **biography **
          (links a work to an author that it is about) (see [Wikipedia](https://en.wikipedia.org/wiki/Biography).)
          Example: [Albert Einstein](https://bookbrainz.org/author/43021f4f-4fda-4b32-bbf0-f2601181e32d) is the subject of [Einsteins Dilemma](https://bookbrainz.org/work/ee781ecd-55fb-4e97-b8f7-0cb19c0fa963) by [Peter Ustinov](https://bookbrainz.org/author/f3c32e2f-a15b-4489-bbb9-ee399cf10d38)
            * (note about [marriage](https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16) applies here as well)
    * **copyright**
        (links an Author to a work they own the copyright for)
           Authors don't always own or hold the copyright for their Work. For example a publishing house can hire writers and maintain copyright on the produced work.
           Look for the © symbol on the (aptly named) _"copyright page"_.
    * **licensor**
        (links an Author to a work they have licensed)
         Book licensing, in the context of author-relationships, refers to the legal permission the Author grants to other parties such as publishers, distributors or translators; to use, reproduce, distribute or adapt their literary work under specific terms, while typically *retaining* ownership of that work.
3. **Editions**
   Editions are the actual physical books in our hands! (see [about editions for more info](edition.md).)
    * **foreword**
      links an author to an edition they wrote a foreword for ([Wikipedia](https://en.wikipedia.org/wiki/Foreword).)
         Note: the foreword shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * **preface**
      links an author to an edition they wrote a preface for ([Wikipedia](https://en.wikipedia.org/wiki/Preface).)
         Note: the preface shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * **introduction**
      links an author to an edition they wrote an introduction for ([Wikipedia](https://en.wikipedia.org/wiki/Introduction_(writing)).)
         Note: the introduction shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * **illustrator (see above)**
      links a person to an edition they have provided illustrations for
         Note: the illustrator should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *Edition* level relationship.
    * **photographer [^7] (see above)**
      links a person to an edition they have provided photography for
         Note: the photographer should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *Edition* level relationship.
      Example: [Annie Leibovitz](https://bookbrainz.org/author/f2957c29-8257-4d2d-aac2-500ec84c2478)
    * **designer (see [Wikipedia](https://en.wikipedia.org/wiki/Print_design).)**
      links a person to an edition they have done design work on
      Example: [Clay Gardner](https://bookbrainz.org/author/a45ce3bf-0208-4745-85dc-d395e37a4772)
    * **editor (see [Wikipedia](https://en.wikipedia.org/wiki/Editing).)**
      links a person to an edition they have edited
      Example: [Jennifer LeBlanc](https://bookbrainz.org/author/68cc3e13-d796-44db-bdcf-61251ce92aff)
    * **typesetter (see [Wikipedia](https://en.wikipedia.org/wiki/Typesetting).)**
      links a person to an edition they have typesetted
    * **compiler (see [Wikipedia](https://en.wikipedia.org/wiki/Anthology).)**
      links a person to an edition they have compiled or done compilation work on, commonly, an Anthology
      The difference between an Author and a Compiler: Generally the Author is the one who came up with the idea, writes the work, uses their own ideas and research. A Compiler on the other hand, collects and organizes existing materials, sometimes from several sources, to create a comprehensive whole, but does not necessarily add any new original content (as opposed to the "reconstructed" relationship defined above).
    * **proofreader (see [Wikipedia](https://en.wikipedia.org/wiki/Proofreading).)**
      links a person to an edition they have proofread
      Example: [Dayna Abel](https://bookbrainz.org/author/5eb369d9-5a73-4e02-a8a5-e43db8b7553e)
    * **art director (see [Wikipedia](https://en.wikipedia.org/wiki/Art_director#In_publishing).)**
      links a person to an edition they have provided art directing on
      Example: [Peter Feierabend](https://bookbrainz.org/author/8b34cdce-c8ce-4b79-91d1-5c380ec4eb43)
    * **blurb (see [Wikipedia](https://en.wikipedia.org/wiki/Blurb).)**
        * blurbs are short quotes, reviews, summaries of the plot, author bio or other promotional content, usually found on book jackets
          (Note: you should only add this if the author of the blurb is *known*, don't use [unknown] etcetera as noted above)
4. **Publishers**
    * **founder**
      links a Person to a Publisher-company they have founded
    * **employee**
      links a Person to a Publisher-company they are employed with
5. **Series**
   See the [series entity page](./series.md)
6. **Edition groups**
   There are no relationships between Authors and Edition Groups. You might be looking for relationships with specific Editions instead, see the *3. Editions* section above
  

[^1]: c.f. https://community.metabrainz.org/t/pen-names-as-aliases-or-as-separate-entries/497086
[^2]: c.f https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16
