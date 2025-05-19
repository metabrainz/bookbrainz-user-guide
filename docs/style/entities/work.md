# Work

Works are distinct literary creations, they represent the _conceptional_ idea of a book, the work entity is for the abstract content of a book, article, paper or comic. For the physical or digital representation, see [edition](edition.md).

[TOC]

## When is a work considered different from another work?

A work is different from another work if there are distinct differences to it, like adaptations, translations, rewritings, and so on.<br>
A work is not a separate one if there are only minor spelling corrections or typographical changes (these aren't on the level of conceptional changes, only edit(orial) ones).

Usually divisions like chapters are considered integral to the work and not distinct from it. While poems, essays, articles and short stories *are* considered distinct.<br>
Examples:<br>
counter Examples: [^1] [^1](the graveyard book is  great counter example here because one chapter was released as a short-story prior, another is the short story in "an apple for the creature" which would go on to be basically most of the first chapter of "The girl with all the gifts")


### When to create new works?
New works should be created when either<br>
a) The work in question is not in the database
b) There are a significant changes to it:<br>
 * Examples:
    * adaptation (comic book)
    * abridged (Jurassic example) [Jurassic park](https://bookbrainz.org/work/c6f3b5a5-646e-46ed-8565-c9551c8a67d4)
    * translations

- Not to create works for simple "introduction/preface/foreword" but to create a link between the Edition and Author instead UNLESS the specific part has become a Thing unto it self and is re-used (cf the discussion in the community thread)

Explain about creating new works for translations (link to sections about which Author-Work links, which Work-Work links (and discussion about Edition-groups) to use).

- How big is a thing before it is a work?<br>
Like, is a sentence by Famous Author that is put in the pretext of a lot of Books a "work" in and of itself?<br>
Answer: NO. However, we should clarify that it is not about length but more about conceptual "content": for example a haiku is very short but would deserve a work.<br>
Might link to notes about quotations/excerpts as well (wait could this be handled by quotations?! e.g. "contains quotation by {author}" i.e. a new rel??)

### What about translations?

Each translation of a work is distinct from the original work as well as any other language translation. Additionally, a work can be translated into the same language several times, each of these are also separate works.<br>
A translated work should have:
 * a relationship added to the original work it is a translation of
 * a relationship to the author that wrote the original (provided story)
 * and a translator relationship to its translator.

Examples:<br>
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) has story written by [Πλάτων](https://bookbrainz.org/author/3efc11ba-87ae-4cd0-9677-373f7618925a)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) is a translation of [Πολιτεία](https://bookbrainz.org/work/40002c97-41df-4659-b0e0-b30dfa5cbc59)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) was translated by [Benjamin Jowett](https://bookbrainz.org/author/dc98466f-9e81-4fb1-a714-3b62b625b455)

If the translator is unknown or unidentified, the translator can be set as [[unknown]](https://bookbrainz.org/author/6c1b8f55-4c7e-4739-bfa2-1979da4c68e1).<br>
Notable information about a translation should be documented in the work's annotation.

## What should works be named?
Generally this should be straightforward, e.g the work for the book [The Silmarillion](https://bookbrainz.org/edition/6d2273eb-2f4e-444f-be61-15f0c23e7451) by Tolkien is called "[The Silmarillion](https://bookbrainz.org/work/e6b73035-4bf5-4989-a877-291d98309e8b)"<br>
Adaptations can often have descriptive subtitles, but if not this information should be put in the disambiguation, for translations, the name should be what is on that translation's cover. Any additional names, such as descriptive titles, known variations or transliterations, should be added as [Aliases](about aliases).

about aliases:
work alias 
(idk)


The language of a work's name can differ from the language of the actual work. For example, a work written in English can have a Latin name. The name of the work should be capitalized based on the rules for the language of its name.<br>
<br>

But what if the book has no name, then what?

### Untitled works
If a work has no title, the first line or sentence of the work should be used, and since this is technically an unofficial name we use square brackets around it like so: [It was the best of times and it was the worst of times]
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
See the [Author](./author.md) page for a description of the types of authors and also the difference between the "written by" Work relationship and Author Credits on Editions.

#### Others
Notably there is one Work-Author link we'll cover here; That of a work that is *about* an Author; Biographies or bio's.<br>
This is a work that is _about_ an Author, someone already in the database. However, someone who never wrote anything, but is in some other way notable, for example; if they link other authors together, via parental or marriage relationships, if they are teachers of other authors, if they have several biographies written about them, they may be be added to BookBrainz, despite not having written anything themselves.<br>
Examples:

### Links to other works
Link works together when:
* works
 * adaptation
     * translation
     * revision
 * derative
     * inspiration
     * parody
 * reconstruction?
* parts (work has part)
 * excerpts
 * quotation
 * citation/refrence
   something about references can also be things like informations
   specify "parafrases" -> cites is these are the sources of that text
   explain the difference between citation and excerpt. excerpt is a section of text verbatim, a paragraph taken from whatever
a citation is instead a work (book) used as a source for whatever in *this* work, usually this is more common for non-fiction.
reference material will often have a bunch of these.


- *it is derived from another work*, for example: a translation, an adaptation, a revision, a reconstruction, a parody, an inspiration;
- *it contains the content from another work or is contained in another work*, for example: a [fix-up](https://en.wikipedia.org/wiki/Fix-up), a poetry cycle, an excerpt, a quote;
-  for example: a citation.

Except for cases such as a fix-up or a poetry cycle as mentioned above, a discrete work should not represent a collection of works.

- derivative: *it is derived from another work*
    - translation
    - adaption
    - inspiration
    - parody
    - revision
    - reconstruction
- parts:
    - *it contains the content from another work or is contained in another work*
        - excerpts
        - quotation
    - *it references another work*
        - citation
        - reference



### Link to Editions
- contains (the most important rel, specify that works can belong to several editions, and that an edition can have several works

### Link to Publishers
- commission
- licensor

### Link to Series
See [series page](./series.md)
