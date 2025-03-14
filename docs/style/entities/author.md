# Author

[TOC]

## What is an Author?
An author is someone who writes, translates or provides a story<br>
In BookBrainz the "[entity](about entities aka /entities.md)[^1]" "Author" is basically any person who performs any number of book-related roles: writing, drawing, compiling, commissioning, even people who are [just related to two or more other authors may be eligible](#what-about-people-who-have-not-written-anything)
Generally they will fall into these 3 types:

## Types of Authors:

#### Person
This is the most common type of Author entity, use for individual people.
Before adding a new Author always check if someone with that name already exists (including searching for any [pen names](#pen-names), aliases, misspellings etc.) before creating a new one.
If two authors bear the same name, use the [disambiguation field](../disambiguation.md) to tell them apart and add as much identifying information as possible.

#### Group
Use this for groups of Authors, like [collective pseudonyms](https://en.wikipedia.org/wiki/Category:Collective_pseudonyms) (pseudonyms used by multiple individuals), [house pseudonyms](https://en.wikipedia.org/wiki/Pen_name#Collective_names) (owned by a publisher and used by the writers working for them) and similar.

#### Persona
Sometimes Authors create characters and also write under that name, while giving this character things like a backstory or have them appear in their work.
This is different from regular pen names in that a Persona is presented as its own thing, not just a character *in* the story, but also as the writer of the work in question. [^5]<br>
Examples:<br>
The writer [Daniel Handler](https://bookbrainz.org/author/394ac1e3-69e8-4eed-afaa-bb06f877c96e) who writes under the pseudonym *Lemony Snicket*, a character and the supposed author of *A Series of Unfortunate Events*.[^2]
[^2]: add more examples

#### Pen Names [^4]
We do not add pen names as separate authors, instead we use [author credits](#author-credits) to show how an edition was credited with another name. 
(note an illustration would be good here)
Additionally an alias[link to section about aliases] should also be added to the author entity.
Examples:<br>
[Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) has aliases and is credited as, Richard Bachman and Beryl Evans [^2]

### What about people who have not written anything?
Someone who never wrote anything, but about whom several biographies have been written, for example, can be added to BookBrainz.
Another relevant metric is if they link 2 or more Author entities. [^3]
These non-writer people can be to be added as <u>Authors</u>, despite not having written anything themselves.

Additionally, there are many other roles an "Author"(entity) can have in BookBrainz: Photographer, penciller, translator, illustrator, and so on (see section below)

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
This section explains about author credits

When entering books into BookBrainz, it's important to understand the difference between the concept of an <u>Edition</u>, the physical item you can hold in your hands, and the literary concept of <u>Works</u> that books contain. (see also [Wikipedia](https://en.wikipedia.org/wiki/Creative_work) for more information.)<br>
{add an example of small collection of short stories by differnt author but only one autor name on the cover}

BookBrainz is a _relationable database_ that tracks the links between different entities, such as, which <u>Author</u> (entity) actually wrote what <u>Work</u> (entity) and so on. But it also is a database of _credited_ information, that is, who is _credited_ as the author.<br>
For the relationable part, we use _relationships_ in the database, typically, an "\[Author\] wrote \[Work\]" relationship.

Examples:<br>
Imagine a collection of short stories written by different authors, were only one author's name is written prominently on the book's cover.<br>
This is where Author Credits come in: here the \[Edition\] should be *credited to* \[that one author\].

An Author, let's call them "Anchovy", wrote a novel under the [pen name](#pen-names) "Betta"; that Work should have a relationship, "Anchovy *wrote* \[Work\]" while the Edition should have the <u>author credit</u> "Anchovy *credited as* Betta"

## Current Author-linking relationships are:

1. Other authors:
    * persona<br>
        (see [above](#persona))[^5] links an author to their persona.
    * Member of group
        * founder<br>
           (link a person as founder of a group of authors)
        * subgroup<br>
           (links a collective as a sub-group to another collective)
    * Marriage<br>
        (link two authors as married, note that [non-authors might be eligible here](#what-about-people-who-have-not-written-anything))
    * involved with<br>
        (link two authors as involved, see note above)
    * parent<br>
        (link an author as being the parent to another, see note above)
    * sibling relations<br>
        (link two (or more) authors as being siblings. take care to link everyone to everyone else!, see note above)

   **Obsolete relationships**, if you see any author with these you are encouraged to fix them!:
    *  ~~collaboration~~<br>
        obsolete, we encourage people to fix old relationships and to use [author credits](#author-credits) and to create collectives (groups) for more permanent collaborations instead.
    * ~~\-pen name~~<br>
        obsolete, (see [above](#persona))[^5] 
1. Works
    * wrote<br>
        (links an author to a work they've written)<br>
        note, several authors can be linked to the same work, and naturally an author can be linked to several works
        * provided story<br>
         (links an author to a work they provided the story for)<br>
         this is used for translated works, because while the author *wrote* the original story, this translated work wasn't *literally* written by them
        * translated<br>
         (links an author to a work they have translated)<br>
          note that the translator should be linked to the *translated* work, not the original work
        * was previously attributed to<br>
         (links an author to a work they've previously been attributed to writing)<br>
          this is used for mostly historical works, where new research finds that so and such author was not actually the one who wrote it (add [example])
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
2. Editions 
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
3. Publishers
    * founder
    * employee
4. Series see [series section]()
5. Edition groups
    *  There are no relationships between Authors and Edition Groups. Youn might be looking for relationships with specific Editions instead, see the 3. Editions section above
  
[^1]: I created /entities.md under "entities"
[^4]: add some kind of formatting here, like italics or slightly grey, to signify that it is not used
[^3]: c.f https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16
[^5]: c.f. https://community.metabrainz.org/t/pen-names-as-aliases-or-as-separate-entries/497086
