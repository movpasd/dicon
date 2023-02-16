# DICON (WIP)
An improved superset of JSON for data interchange


## Scope

DICON is my attempt to extend the JSON format to allow for a more 

Advantages of JSON:
* Flexible semantics = extreme interoperability
* Extremely simple to describe
* Extremely simple to parse
* Relatively human-readable

Disadvantages of JSON:
* Cumbersome to exactly encode numerical data
* Lack of normative data model can lead to quirks
* Whitespace a bit weird

### Normativity of numeric data semantics

JSON has certain limitations in its data encoding system which make it cumbersome to encode certainly commonly used data types, especially numerical data types. This keeps JSON extremely lightweight, but at the expense of usability. Furthermore, the lack of an explicit semantic model results in quirks across implementations.

This is not a flaw with JSON, but a design choice:

> _JSON is agnostic about the semantics of numbers. In any programming language, there can be a variety of number types of various capacities and complements, fixed or floating, binary or decimal. That can make interchange between different programming languages difficult. JSON instead offers only the representation of numbers that humans use: a sequence of digits. All programming languages know how to make sense of digit sequences even if they disagree on internal representations. That is enough to allow interchange._ (ECMA-404, 2nd edition)



### Comments

Yes

### Trailing commas

Yes

### Multi-line strings

Yes -- newlines are not treated specially anymore

### Datetime formats

No

### Objectives 

Provide a specification for an extension of JSON which includes 


## Todo list

- [ ] Create state diagram for DICON syntax parsing
- [ ] Describe normative semantic model for data types
- [ ] Provide canonical lossy semantic conversion algorithm from DICON to JSON
- [ ] Provide canonical lossless conversion of DICON to JSON
