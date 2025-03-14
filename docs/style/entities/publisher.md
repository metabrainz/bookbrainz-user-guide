# Publisher

[TOC]

## What is a Publisher?
- Different type of publishers
- How to identify what kind of publisher it is

## How do I create a Publisher?

(Insert details here)

## Publisher in edition (what to do if there are several)

How/When to create a different Edition Group than what is auto suggested (I feel the actual datamodels code here is kinda unevolved and we should do better (more like mb))

## Linking Publishers to other entities

### Link to other Publishers

Publishing companies change over time, merge within their parent company, get bought by a bigger fish, change ownership, etc.
Most of these Publisher-Publisher relationships are there to track these structural aspects:

- Owner
- Renamed
    - Explain to only do this if when the company is a new one, conceptually, and not just for name-changes, additional &co, etc.
- Split (split into)
- Split (merged into)

### Link to Author
- was founder of
- employee (should rename to "worked as" to match mb)

### Link to Edition
Publishers do have links to Editions because those are the actual real items they interact with (the obvious 'Publisher published Edition', but also copyright, licenses, typesetting, etc that refer to tangible editions [physical or digital])

### Link to Work
(something about copyrights are on spesific editions, etc.)
- commision
- licenced

### Link to Edition Group
We do not create relationships to Edition Groups. For more information see the [Edition Group page](./edition-group.md#linking-edition-groups-to-other-entities)

### Link to Series
See [series section](../../tutorials/series.md)