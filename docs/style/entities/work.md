# Work

A work is a distinct, notable literary creation. The work entity captures information about the *content* that was created, not any physical or digital representation.

[TOC]

## What distinguishes a Work from another?

A work is considered distinct based on the substantive uniqueness of its content. A work is distinct from another if it is revised, adapted, translated or reconstructed. Content is not considered a distinct work if it only contains minor variations such as spelling or typographical differences.

Sometimes content is integral to a work and is not considered distinct from it. In general, chapters of a novel are *not* considered to be their own distinct works. Poems, essays, articles and short stories *are* generally considered distinct works.

### When should I create a new Work ?
- Not to create works for simple "introduction/preface/foreword" but to create a link between the Edition and Author instead UNLESS the specific part has become a Thing unto it self and is re-used (cf the discussion in the community thread)

Explain about creating new works for translations (link to sections about which Author-Work links, which Work-Work links (and discussion about Edition-groups) to use).

- How big is a thing before it is a work?<br>
Like, is a sentence by Famous Author that is put in the pretext of a lot of Books a "work" in and of itself?<br>
Answer: NO. However, we should clarify that it is not about length but more about conceptual "content": for example a haiku is very short but would deserve a work.
Might link to notes about quotations/excerpts as well (wait could this be handled by quotations?! e.g. "contains quotation by {author}" i.e. a new rel??)

### What about translations?

Each translation of a work is distinct from the original work as well as from any other translation. A translated work should have a relationship added to the original
work as a translation, have a *writer* relationship to the original work’s author, and a *translator* relationship to its translator. Example:

- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) has story written by [Πλάτων](https://bookbrainz.org/author/3efc11ba-87ae-4cd0-9677-373f7618925a)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) is a translation of [Πολιτεία](https://bookbrainz.org/work/40002c97-41df-4659-b0e0-b30dfa5cbc59)
- [Republic](https://bookbrainz.org/work/c1b11cb0-38b0-49ea-88e8-83566c5589ad) was translated by [Benjamin Jowett](https://bookbrainz.org/author/dc98466f-9e81-4fb1-a714-3b62b625b455)

If the translator is unknown or unidentified, the translator should be [[unknown]](https://bookbrainz.org/author/6c1b8f55-4c7e-4739-bfa2-1979da4c68e1).

Notable information about a translation should be documented in the work's annotation.

## What should I name the Work?

The name of a work should be its canonical title, in the language it was written by its author, or translator for translated works. Additional names, such as descriptive titles, known variations or transliterations should be included as aliases.

The language of a work’s name can differ from the language of the actual work. For example, a work written in English can have a Latin name. The name of the work should be capitalized based on the rules for the language of its name.

### Untitled works

If a work does not have a title, use the first line or sentence of the work’s text, enclosed in square brackets as its name. Do not apply title capitalization rules; retain the case of the original text. Examples:

- [[At that hour when all things have repose]](https://bookbrainz.org/work/c0b50c4b-d57d-43bf-83b2-4930d938a0e4)
- [[Rash mortal! stay thy feet and look around]](https://bookbrainz.org/work/ed6d8c28-fe3c-4fde-b399-6663c2225805)

The sort name of an untitled work should be the same name, omitting the square brackets.


## Linking Works to other entities


### Link to other works
A work should have a relationship added to another work if:

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

### Link to Authors

#### Writer

The primary relationship of a work is to its main author, aka its *writer*; every work should have at least one writer.

See the [Author](./author.md) page for a description of the types of authors and the difference between the "written by" Work relationship and Author Credits on Editions.

#### Other
- (work about author, what authors to create if at all for this)(c.f. "marriage ref")
- section above, I'd move these here maybe?
- (it makes sense that explicit work > author ordered relationship would be here.)

### Link to Editions
- contains (the most important rel, specify that works can belong to several editions, and that an edition can have several works

### Link to Publishers
- commission
- licensor

### Link to Series
See [series section](./series.md)
