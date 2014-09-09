# Global Substitution

## Intro

Abbreviated to `.gsub()`, this method is a handy ruby tool that allows you to `globally substitute` one or more words, or character for another. Let's take a look at how that works.

We have a fact about a bug assigned to a variable `wrong_fact`:

```ruby
wrong_fact = "Ladybugs can taste with their feet."
```

But wait, that's not a fact about ladybugs, but butterflies! Let's swap out the word "Ladybugs" for "Butterflies" using .gsub. The method `.gsub` takes two `parameters`, the first one the word you want to replace, and the second one is the word you want to replace it with:

```ruby
right_fact = wrong_fact.gsub("Ladybugs", "Butterflies")
```

The `return value` (aka, what this action produces when it's called) will be "Butterflies can taste with their feet." Then, if we type `right_fact` into our console, we'll see the fact correctly printed.

## Chaining

What if you have a sentence that you want to substitute more than one word in? We can do that by calling `.gsub` more than once on the same line, through a process called `method chaining`. Take a look:

```ruby
wrong_fact = "Cats fail to recover about 50 percent of the nuts they bury."
true_fact = wrong_fact.gsub("Cats", "Squirrels").gsub("50", "74")

```
