---
name: vim
category: reverse
points: 726
solves: 8
---

{% ignore %}
[Go to rendered GitBook version](https://sasdf.cf/ctf/)
{% endignore %}

> A vim challenge written with [kakoune](https://kakoune.org/).


# Overview, Concept and Design Criteria
I was trying to create reverse challenge with some strange languages. (or even not a language).
This is one of them.

## Design criteria
When writing a reverse challenge,
it's not too hard to create a huge amount of 💩 which is impossible to solve,
and I want to avoid that.

To make the code reasonable,
I use adopt some common pattern in asm here.

For example, there are many inlined function calls, and they have prologue/epilogue to save registers.

The whole program is built from many functions, so the pattern of each function can be easily detected.


# Solution
Will be released 72 hours after the end of competition.
