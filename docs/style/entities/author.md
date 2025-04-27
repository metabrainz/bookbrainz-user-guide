# Author

[TOC]

## What is an Author?
An author is someone who writes, translates or provides a story<br>
In BookBrainz the "[entity](../../getting-started.md#what-is-an-entity-in-bookbrainz)" "Author" is basically any person who performs any number of book-related roles: writing, drawing, compiling, commissioning, even people who are [just related to two or more other authors may be eligible](#what-about-people-who-have-not-written-anything)<br>
Generally they will fall into these 3 types:

## Types of Authors:

#### Person
This is the most common type of Author entity, use for individual people.<br>
Before adding a new Author always check if one exists already with that name (also remember to search for any [pen names](#pen-names), aliases, misspellings and so on) before creating a new one.<br>
In general, try to add as much identifying information as possible and also add a [disambiguation](../disambiguation.md). This is necessary if another author with the same name exists, but it is always a good idea to add disambiguations, because it makes it easier for users to choose the right author, and also easier to make sure they have right one."<br>
Try to create short, concise disambiguations.<br>
Examples: "18th century novelist", "19th century Belgian playwright" or "Nigerian Africanfuturist writer"

#### Group
Use this for groups of Authors, like [collective pseudonyms](https://en.wikipedia.org/wiki/Category:Collective_pseudonyms) (pseudonyms used by multiple individuals), [house pseudonyms](https://en.wikipedia.org/wiki/Pen_name#Collective_names) (owned by a publisher and used by the writers working for them) and similar.<br>
Examples:<br>
[Ellery Queen](https://bookbrainz.org/author/a2532a57-11fa-43d4-aa5d-c2892a2d0320), the group pseudonym of *Frederic Dannay* and *Manfred Bennington Lee*.<br>
[James S. A. Corey](https://bookbrainz.org/author/c5c71242-f54c-4327-9510-a81064a9a852) pen name used by *Daniel Abraham* and *Ty Franck*.

#### Persona
Sometimes Authors create characters and also write under that name, whilst giving this character things like a backstory or have them appear in their work.
This is different from regular pen names in that a Persona is presented as its own thing, not just a character *in* the story, but also as the writer of the work in question. [^5]<br>
Examples:<br>
The writer [Daniel Handler](https://bookbrainz.org/author/394ac1e3-69e8-4eed-afaa-bb06f877c96e) who writes under the pseudonym *Lemony Snicket*, a character and the supposed author of *A Series of Unfortunate Events*.

#### Pen Names
We do not add pen names as separate authors, instead we use [author credits](#author-credits) to show how an edition was credited with another name. 
(note an illustration would be good here)
Additionally, an alias[link to section about aliases] should also be added to the author entity.<br>
Examples:<br>
[Stephen King](https://bookbrainz.org/author/128d9490-ee19-4270-a070-32e0a36847f5) has aliases and is credited as *Richard Bachman* and *Beryl Evans*.

### What about people who have not written anything?
Someone who never wrote anything, but about whom several biographies have been written, for example, can be added to BookBrainz.
Another relevant metric is if they link 2 or more Author entities. [^3]
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

When entering books into BookBrainz, it's important to understand the difference between the concept of an <u>Edition</u>, the physical item you can hold in your hands, and the literary concept of <u>Works</u> that books contain. (see also [Wikipedia](https://en.wikipedia.org/wiki/Creative_work) for more information.)<br>
{add an example of small collection of short stories by different author but only one autor name on the cover}

BookBrainz is a _relationable database_ that tracks the links between different entities, such as, which <u>Author</u> (entity) actually wrote what <u>Work</u> (entity) and so on. But it also is a database of _credited_ information, that is, who is _credited_ as the author.<br>
For the relationable part, we use _relationships_ in the database, typically, an "\[Author\] wrote \[Work\]" relationship.

Examples:<br>
Imagine a collection of short stories written by different authors, were only one author's name is written prominently on the book's cover.<br>
This is where Author Credits come in: here the \[Edition\] should be *credited to* \[that one author\].

An Author, let's call them "Anchovy", wrote a novel under the [pen name](#pen-names) "Betta"; that Work should have a relationship, "Anchovy *wrote* \[Work\]" while the Edition should have the <u>author credit</u> "Anchovy *credited as* Betta"

## Current Author-linking relationships are:

 1. Other Authors:
    * persona<br>
        (see [above](#persona)) links an Author to their persona.
    * Member of group
        * founder<br>
           (link a person as founder of a group of authors)
        * subgroup<br>
           (links a collective as a sub-group to another collective)
    * Marriage<br>
        (link two authors as married, note that [non-authors might be eligible here](#what-about-people-who-have-not-written-anything))
    * involved with<br>
        (link two authors as involved, see above note)
    * parent<br>
        (link an author as being the parent to another, see above note)
    * sibling relations<br>
        (link two (or more) authors as being siblings. Take care to link everyone to everyone else!, see above note)<br>
* **Obsolete relationships**, if you see any author with these you are encouraged to fix them!:
    *  ~~collaboration~~<br>
        obsolete, we encourage people to fix old relationships and to use [author credits](#author-credits) and to create collectives (groups) for more permanent collaborations instead.
    * ~~\-pen name~~<br>
        obsolete, (see [above](#persona))
      
2. Works<br>
   Works are the conceptional part of writing! (See [about Works](work.md) for more information)
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
    * worked on<br>
        (links an Author to a work they have worked on in some miscellaneous way)
        * adapted<br>
          (links an author to a work they have adapted ([see Wikipedia for more information about adaptions](https://en.wikipedia.org/wiki/Adaptation_(arts)))<br>
           note you should also add a work-work "adaptation of" link between the Original Work and the Adapted Work [see the work-entity page relevant section]()
        * revised<br>
          (links an author to a work they have revised ([see Wikipedia for more information about revisions](https://en.wikipedia.org/wiki/Revision_(writing)))<br>
           note you should also add a work-work "revision of" link between the original work and the revised work [link to the work-entity page relevant  section]
        * reconstructed<br>
          (links an author to a work they have reconstructed [link to wikipedia that explains reconstructions])<br>
           note you should also add a work-work "reconstruction of" link between the original work and the reconstructed work [link to the work-entity page relevant section]
    * artist<br>
       artists are people with roles that encompass all artistic work *except* writing. (see [#what-about-people-who-have-not-written-anything](#what-about-people-who-have-not-written-anything))<br>
       note while these are not writers, they are still added with "add author" [link to how to add author page we don't yet have]
        * photographer<br>
          (links a photographer to a work they have provided photography for)<br>
           note you should only add photographers to *works* when their photography is intrinsically part of the work, that is, if the story makes just as much sense without it, you should instead link them to the (see below) *edition*)
        * illustrator<br>
          (links an illustrator to a work they have illustrated)<br>
           note you should only add illustrators to *works* when their illustrations are intrinsically part of the work, that is, if the story makes just as much sense without it, you should instead link them to the (see below) *edition*)
        * penciller<br>
          (links a penciller to a work they have pencilled, this is used ostencibly for comics, manga and graphic novels)
        * inker<br>
          (links an inker to a work they have inked, ostencibly comics, manga and graphic novels)
        * colourist<br>
          (links a colourer to a work they have coloured, this is used ostensibly for comics, manga and graphic novels)
        * letterer<br>
          (links a letterer to a work they have provided letters for, this is used ostensibly in comics, manga and graphic novels)
    * other<br>
        (link authors (people) in some other, unspecified or not-yet available relation (also see [how to suggests changes aka JIRA tickets] and [community discussion].
        * commissioner<br>
          (link someone to the work they have commissioned [see Wikipedia for more information about Commissions](https://en.wikipedia.org/wiki/Commission_(art)))
        * dedication<br>
          (links a work to an author it contains a dedication to) (see [wikipedia](https://en.wikipedia.org/wiki/Dedication_(publishing)) )
            * (note about [marriage](https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16) applies here as well)
        * biography<br>
          (links a work to an author that it is about) (see [wikipedia](https://en.wikipedia.org/wiki/Biography).)
            * (note about [marriage](https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16) applies here as well)
    * copyright<br>
      (idk)
    * licensor<br>
       (no idea)
3. Editions<br>
   Editions are the actual physical books in our hands! (see [about editions for more info](edition.md).)
    * foreword<br>
       (links an author to an edition they wrote a foreword for) ([wikipedia](https://en.wikipedia.org/wiki/Foreword).)<br>
         note that the foreword shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * preface<br>
       (links an author to an edition they wrote a preface for) ([wikipedia](https://en.wikipedia.org/wiki/Preface).)<br>
         note that the preface shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * introduction<br>
       (links an author to an edition they wrote an introduction for) ([wikipedia](https://en.wikipedia.org/wiki/Introduction_(writing)).)<br>
         note that the introduction shouldn't be it's own separate work *unless* it's notably reused for completely *other* editions, this will usually be fairly rare.
    * illustrator (see above)<br>
       (links a person to an edition they have provided illustrations for)
         note that the illustrator should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *edition* level rel.
    *  photographer (see above)<br>
       (links a person to an edition they have provided photography for)
         note that the photographer should be add to edition only if its a "variable addition", that is, if the story makes just as much sense without the art, if there exists versions without it, or with different art, then this is an *edition* level rel.
    *  designer (see [wikipedia](https://en.wikipedia.org/wiki/Print_design).)<br>
       (links a person to an edition they have done design work on)
    *  editor (see [wikipedia](https://en.wikipedia.org/wiki/Editing).)<br>
       (links a person to an edition they have edited)
    *  typesetter [wikipedia](https://en.wikipedia.org/wiki/Typesetting).)<br>
       (links a person to an edition they have typesetted)
    *  compiler<br>
       (links a person to an edition they have compiled or done compilation work on)
    *  proofreader (see [wikipedia](https://en.wikipedia.org/wiki/Proofreading).)<br>
       (links a person to an edition they have proofread)
    *  art director (see [wikipedia](https://en.wikipedia.org/wiki/Art_director#In_publishing).)<br>
       (links a person to an edition they have provided art directing on)
    * blurb (see [wikipedia](https://en.wikipedia.org/wiki/Blurb).)<br>
        * blurbs are short quotes, reviews, summaries of the plot, author bio or other promotional content, usually found on book jackets
          (note you should only add this if the author of the blurb is *known*, don't use [unknown] etcetera as noted above)
4. Publishers
    * founder<br>
       (links a Person to a Publisher-company they have founded)
    * employee<br>
       (links a Person to a Publisher-company they are employed with) 
5. Series see the [series entity page](./series.md)
6. Edition groups
    *  There are no relationships between Authors and Edition Groups. You might be looking for relationships with specific Editions instead, see the 2. Editions section above
  

[^4]: add some kind of formatting here, like italics or slightly grey, to signify that it is not used
[^3]: c.f https://community.metabrainz.org/t/concerning-the-new-is-about-relation/497088/16
[^5]: c.f. https://community.metabrainz.org/t/pen-names-as-aliases-or-as-separate-entries/497086
