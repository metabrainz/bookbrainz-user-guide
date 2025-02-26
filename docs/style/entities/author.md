# Author

[TOC]

## Author Credits
Section that explain what about author credits (link to [How to add Authors](#when-to-add-an-author))

When entering a book into BookBrainz, you will need to understand the difference between the Edition you hold in your hands and the litterary Work (or Works) that it contains.

To track authorship, Work entities are related to one or more Authors via an "Author wrote Work" relationship.

Now imagine a collection of short stories written by different authors, with only one of the author's name written prominently on the book cover.
This is where Author Credits come in: the Edition is *credited to* AuthorName.

Another example is [pen names](#pen-names): Author A wrote a novel under the pen name "Author B"; the Work has a relationship "Author A *wrote* Work" while the Edition has the author credit "Author A *credited as* Author B"

## When to add an author?
explain about [personas](#persona), collectives

## Types of Authors:

#### Person
For individual writers and the most common type of Author entities.
Do check if an author with that name exists (including searching for their [pen names](#pen-names)) before creating a new one.
If two authors bear the same name, use the [disambiguation field](../disambiguation.md) to tell them apart and add as much identifying information as possible.

#### Group
This type of author can be used for [collective pseudonyms](https://en.wikipedia.org/wiki/Category:Collective_pseudonyms) (pseudonyms used by multiple individuals), but also [house pseudonyms](https://en.wikipedia.org/wiki/Pen_name#Collective_names) (owned by a publisher and used by the writers working for them).

#### Persona
Sometimes an author uses creates a character and writes under that pen name, while giving the character a backstory or having them appear in their work.
This is different from other pen names in that a persona is presented as a character, but the work in question is credited to the persona.
A good example of this comes from writer (Daniel Handler)[https://bookbrainz.org/author/394ac1e3-69e8-4eed-afaa-bb06f877c96e] who writes under the pseudonym Lemony Snicket, a character and supposed author of 'A Series of Unfortunate Events'.

#### Pen Names
We do not add pen names as separate authors, instead we use [author credits](#author-credits) to XXX how an edition was credited as another name.
Additionally an alias (link to section about aliases) should also be added to the author entity (see for example [Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5)/Richard Bachman/Beryl Evans)

### What about people who are not writers?

Someone who never wrote anything, but about whom several biographies have been written, for example, can be added to BookBrainz.
Another relevant metric is if they link 2 or more Author entities.
c.f https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16 
These non-writer people need to be added as an Author entity despite their lack of authorship.

## What if a Work doesnt *have* a known author?
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

## How/when to link Authors to:

1. Other authors (link back to the pen names/personas section above)
    * persona
        (see above, and we should explain what is the diff between pen name and persona)  c.f. https://community.metabrainz.org/t/pen-names-as-aliases-or-as-separate-entries/497086
    * Member of group
        * founder
        * subgroup
    * Marriage
        See [non-authors section above](#what-about-people-who-are-not-writers)
    * ditto involved with.
    * same with the parent, sibling relations.
    *  ~~collaboration~~
        obsolete, we encurage people to fix old relationships and to use [author credits](#author-credits) and to create collectives (groups) for more permanent collaborations instead.
    * ~~\-pen name~~
2. Works
    * wrote
        * provided story
            * explain the difference between "wrote" and "provided story"
        * translated
            * explain that the translator should be linked to the *translated* work, not the original work
        * was previously attributed to
    * worked on
        * adapted
        * revised
        * reconstructed
    * artist
        * photographer
            * (specify when to link photographers to *works* and when to link to (see below) *editions*)
        * illustrator
            * (specify when to link illustrators to works and when to link to (see below) *editions*)
        * penciller
        * inker
        * colourist
        * letterer
    * other
        * commissioner
        * dedication
            * (note about marriage c.f. https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16 applies here too)
        * biography
            * (note about marriage c.f. https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16 applies here too)
    * copyright
    * licensor
3. Editions 
    * foreword
    * preface
    * introduction
    * blurb
        * (short quotes, reviews, summary of the plot, author bio or other promotional content, usually found on book jackets) from https://en.wikipedia.org/wiki/Blurb\#Books
        * (specify that this should only be added if the author is *known*)
    * illustrator (see above)
        * (specify that illustrator should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *edition* level rel.)
    *  photographer (see above)
        * (specify that photographer should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *edition* level rel.)
    *  designer
    *  editor
    *  typesetter
    *  compiler
    *  proofreader
    *  art director
4. Publishers
    * founder
    * employee
5. Series see [series section]()
6. Edition groups
    *  There are no relationships between Authors and Edition Groups. Youn might be looking for relationships with specific Editions instead, see the 3. Editions section above