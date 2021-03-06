---
layout: page
title: "UCSD CSE11 S20 – PA3"
doodle: "/doodle.png"
---

# Programming Assignment 3 – Class Practice

<p style="border: 2px dotted red; padding: 1em; background-color: #fce803">
This is a draft, this notice will be released when the PA is finalized.
</p>

This programming assignment will help you practice writing classes.

You will upload _several_ Java files for this assignment, detailed below.

## Drill 1 (auto)

Write three classes as described below. They do not need to have any methods or
constructors. Save them in a file called `Drill1.java`.

- A class named `A` with two fields, `int f1` and `String f2`
- A class named `B` with two fields, `A field1` and `String field2`
- A class named `C` with three fields, `B fieldB`, `A fieldA`, `int field3`

## Drill 2 (auto)

Create a file called `Drill2.java` containing the following class definitions
(you can copy/paste them from here):

```
class C1 {
  C2 other;
  C1(C2 other) {
    this.other = other;
  }
}

class C2 {
  int x;
  C2(int x) {
    this.x = x;
  }
}
```

Then add a class definition called `Drill2` with the following fields:

- A field named `first` of type `C2` with its `x` field equal to 10
- A field named `second` of type `C1`. It's value should be a reference to a
  `C1` object with its `other` field set to any `C2` object _other than the
  one stored in_ `first` (you can create another `C2` object for this).
- A field named `third` of type `C1`. It's value should be a reference to a
  `C1` object with its `other` field _the same C2 object_ as the one stored in
  the `first` field.


## Drill 3 (auto)

In a file called `Drill3.java`, write a class called `TextTweet` that has two
fields: one field called `contents` of type `String`, and one field called
`likes` of type `int`. Give it a default constructor of one argument that
initializes that field. In it, write the following methods:

- `hasMention` which takes a `String` called `username` and checks if the
  string `@` followed by that username apppears in the Tweet contents
- `hasLike` which takes no arguments and returns `true` if the tweet has zero
  likes, false otherwise.
- `firstMention` which takes no arguments and returns a `String` containing the
  substring between the _first_ appearance of the `@` character in the
  `contents` and the first space character after that.

## Open-Ended 1 (manual)

Consider the following statements about Java programs:

1. In Java, two different classes can define a field with the same name and
type.
2. In Java, one class can define two fields with the same name as long as they
have different types.

For each, write a small Java program that demonstrates whether it is true or
false. Put them in the files `Open1.java` and `Open2.java`.

To show that a statement is true, write a Java program that matches the
statement and doesn't produce an error when run.

To show that a statement is false, write a Java program that matches the
statement and produces an error when run, demonstrating that Java programs
cannot do what the property says.

Include both the program and a screenshot of running the program without error
as your submission; the template has space for both of these.


