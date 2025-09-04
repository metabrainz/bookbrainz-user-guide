# Work

Works are distinct literary creations, they represent the _conceptional_ idea of a book, the work entity is for the abstract content of a book, article, paper or comic. For the physical or digital representation, see [edition](edition.md).

[TOC]

## When to create new works?
New works should be created when either:

1. The work in question is not in the database
2. There are a significant changes to it, for example:
    * adaptations
        * Example: comic book, stage play
        * Example: [Jurassic Park (Guided Reader Version)](https://bookbrainz.org/work/c6f3b5a5-646e-46ed-8565-c9551c8a67d4), is based on [the original novel](https://bookbrainz.org/work/5479960d-a3a4-4028-a085-ca5bde76c32b) of the same name.
3. It is a translation:<br>
        * Example: [Alice i eventyrland](https://bookbrainz.org/work/50437b54-68db-4c26-871a-23d1546758d7) is a translation of [Alice's Adventures in Wonderland](https://bookbrainz.org/work/337a8c0a-3574-404e-abb5-df606cc36109)


### When is a work considered different from another work?

A work is different from another work if it is distinctly _different_, like adaptations, translations, rewritings, and so on.<br>
A work is not a separate one if there are only minor spelling corrections or typographical changes (these aren't on the level of conceptional changes, only edit(orial) ones).

Usually divisions like chapters are considered integral to the work and not distinct from it, while poems, essays, articles and short stories *are* considered distinct.<br>
 * Example: A novel (with chapters) entered as a single Work entity: [The Long Earth](https://bookbrainz.org/edition/73dc9e04-997d-4c0f-94ac-63c0c7f3c1c0)
 * Example: An anthology of poems, each poem entered as a separate work: [Spoon River Anthology](https://bookbrainz.org/edition/7cb01eb1-735a-4184-af7f-8f021067d6da)
 * However, sometimes things are more complex:
   * The novel [The Graveyard Book](https://bookbrainz.org/work/06fa3810-218e-4246-93da-f850537d1158) is composed of multiple chapters
   * One of those chapters was previously published separately as a short story: [The Witch's Headstone](https://bookbrainz.org/work/85e25493-3851-47e7-a25c-730ceaf6389d), for which we want a separate Work entity

#### What about a book's introduction/foreword/preface?

Usually we do not create works for simple introductions, prefaces and forewords.<br>
* To register that an author wrote an introduction or foreword to a novel, you can simply use the "Author wrote introduction for Edition" relationship.
* However, since more details cannot yet be captured that way, if needed, you can create a separate Work entity to capture those details, or write them in the edition's Annotation.
* Say the introduction is denoted with emphasis (for example "Foreword by XXXXX" on the cover), contains more literary content or is a whole essay in itself, or otherwise has notable literary or historical value."<br>
        * Example:


### More about translations

Explain about creating new works for translations (link to sections about which Author-Work links, which Work-Work links (and discussion about Edition-groups) to use).
Each translation of a work is distinct from the original work as well as any other language translation.<br>
Additionally, a work can be translated into the same language several times, each of these are also separate works.<br>
A translated work should have:<br>

- a relationship added to the original work it is a translation of
- a relationship to the author that wrote the original (see [provided story](author.md#current-author-linking-relationships-are) relationship)
- and a translator relationship to its translator.

Examples:

- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) has story written by [Πλάτων](https://bookbrainz.org/author/3efc11ba-87ae-4cd0-9677-373f7618925a)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) is a translation of [Πολιτεία](https://bookbrainz.org/work/40002c97-41df-4659-b0e0-b30dfa5cbc59)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) was translated by [Benjamin Jowett](https://bookbrainz.org/author/dc98466f-9e81-4fb1-a714-3b62b625b455)

If the translator is unknown or unidentified, the translator can be set as [[unknown]](https://bookbrainz.org/author/6c1b8f55-4c7e-4739-bfa2-1979da4c68e1).<br>
Notable information about a translation should be documented in the work's annotation.


<!-- ### What is the difference between an anthology, a short story cycle and a book of short stories?

An anthology is:
example:
a short story cycle:
example:
book of short stories
example: -->


## What should works be named?
Generally this should be straightforward, e.g. the work for the book [The Silmarillion](https://bookbrainz.org/edition/6d2273eb-2f4e-444f-be61-15f0c23e7451) by Tolkien is called "[The Silmarillion](https://bookbrainz.org/work/e6b73035-4bf5-4989-a877-291d98309e8b)"<br>
Adaptations can often have descriptive subtitles, but if not this information should be put in the disambiguation, for translations, the name should be what is on that translation's cover. Any additional names, such as descriptive titles, known variations or transliterations, should be added as [Aliases](../../glossary.md).

The language the work's _name_ is in, can differ from the language the work as a whole is written in. For example, a work written in English can have a Latin name. The name of the work should _generally_ be capitalized based on the rules for the language of its name.<br>

bit about sortnames and authors intent<br>
Sortnames are used to, as the name suggests, sort works, editions, authors and so on. To anyone who has ever tried finding anything at a library, the reason is apparent: some kind of consistent system must be in place, or finding things will be needlessly time-consuming or at worst impossible.<br>
Generally Works are sorted on their name omitting any leading articles, like "The", "A", "Le", "Den" and so fort, which are added to the end after a comma, like so: "The Bookinator" -> "Bookinator, The". <br>
Examples:<br>
* "Le Tour du monde en quatre-vingts jours" -> "Tour du monde en quatre-vingts jours, Le"
* 

<br>
Sometimes authors have clear intent for the capitalisation or punctuation of the work's title; this is done for comedic, apropos or stylistic reasons, and should be followed.<br>
Examples:<br>

* [VALIS](https://bookbrainz.org/work/983a2d75-522a-41fc-9657-0c6fcf8964c7) - Philip K Dick
* [`<script>alert("!Mediengruppe Bitnik");</script>`](https://bookbrainz.org/work/160fc57a-87f5-4adc-ba19-0384fa382cf8) 

<br>


But what if the book _has_ no name, then what?

### Untitled works
If a work has no title, the first line or sentence of the work should be used, and since this is technically an unofficial name we use square brackets around it like so: [It was the best of times and it was the worst of times]<br>
Generally you should also not use title case in this case, but the original sentence's capitalisation<br>
Examples:

- [[At that hour when all things have repose]](https://bookbrainz.org/work/c0b50c4b-d57d-43bf-83b2-4930d938a0e4)
- [[Rash mortal! Stay thy feet and look around]](https://bookbrainz.org/work/ed6d8c28-fe3c-4fde-b399-6663c2225805)

The sort names of untitled works should be the same, just omitting the square brackets.


## Linking Works to other entities

### Links to Authors
For the full Author-Work relationships, see the [Author page](author.md).

#### Writer
The main Author-Work relationship is that of a work to it's author(s), aka its *writer(s)*; most every work should have at least one of these.<br>
See the [Author](./author.md) page for a description of the types of authors and also the difference between the "written by" Work relationship and [Author Credits](./author.md#author-credits) on Editions.

#### Others
Notably there is one Work-Author relationship we'll cover here: that of biographies, a work that is *about* an Author entity.<br>
This is a work that is _about_ an Author, someone already in the database. However, someone who never wrote anything, but is in some other way notable, for example; if they link other authors together, via parental or marriage relationships, if they are teachers of other authors, if they have several biographies written about them, they may be be added to BookBrainz, despite not having written anything themselves.<br>
Examples:<br>
- [Henry Kissinger](https://bookbrainz.org/author/8eca361c-99f3-46c6-9c8a-a53e92d10694) is the subject of multiple biographies but has not written any work himself

### Links to other works
Linking works together:

* works
 * adaptation
links a work that is an [adaptation](#when-to-create-new-works) of another work.
     * translation
links a work that is a translation of another work, remember to add a link to the works translator here, but the original author should have *provided story*
     * revision
links a work to a revision of it
 * derivative
links a work that is in some way a derivation.
     * inspiration
only use this if the work is generally understood to be inspired by another
     * parody
se this when it is explicitly stated, or is generally understood to be a parody.
 * reconstruction
links a work to a work it is a reconstruction of:
a reconstruction is a work that is created by (usually) another person than the original writer, using already written bits and pieces to create a consistent whole.<br>
example: https://en.wikipedia.org/wiki/The_Silmarillion#Posthumous_publication
* parts (work has part)
when a work consists of several sub-parts, this is used to link each part to the mother work.
 * excerpts: links a work to another work that is quoted verbatim
 * quotation
 * citation/reference: contrarily to excerpts, cites or refers to another work without copying its content
* derived from another work, for example: a translation, an adaptation, a revision, a reconstruction, a parody, an inspiration;
* contains/is contained in another work, for example: a [fix-up](https://en.wikipedia.org/wiki/Fix-up), a poetry cycle, an excerpt, a quote;
*  for example: a citation.

Except for cases such as a fix-up or a poetry cycle as mentioned above, a discrete work should not represent a collection of works.


### Link to Editions

* contains
the most important relationship, specify that works can belong to several editions, and that an edition can have several works
Editions are the physical book that the conceptual work exists in. An edition can contain more than one work, and a work can be published in several editions. See [Edition](./edition.md)


### Link to Publishers
* publisher
links a work to a publisher that published it
here must we clarify the difference between the in-page "publisher" field and the use of this(pita)
* commission
links a work to a publisher that commissioned it
* licensor
see above for author 

### Link to Series
See [series page](./series.md)
