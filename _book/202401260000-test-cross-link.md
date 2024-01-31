# test cross-link

## link and reference

\@ref(nice-label)

[link to partition][partition]

[partition] [#partition] (\@ref(partition)) \@ref(#partition)

[equivalence class] [#equivalence class] (\@ref(equivalence class)) \@ref(#equivalence class)

[equivalence-class] [#equivalence-class] (\@ref(equivalence-class)) \@ref(#equivalence-class)

[equivalence-class.html] [equivalence-class.html#equivalence-class] (\@ref(equivalence-class.html)) \@ref(equivalence-class.html#equivalence-class)

[equivalence relation] [#equivalence relation] (\@ref(equivalence relation)) \@ref(#equivalence relation)

[equivalence-relation] [#equivalence-relation] (\@ref(equivalence-relation)) \@ref(#equivalence-relation)

[equivalence-relation.html] [equivalence-relation.html#equivalence-relation] (\@ref(equivalence-relation.html)) \@ref(equivalence-relation.html#equivalence-relation)

## footnote

noun[^202401260000-test-cross-link-1]

[^202401260000-test-cross-link-1]: This is a footnote.

## citation

https://stackoverflow.com/questions/48965247/use-csl-file-for-pdf-output-in-bookdown/49145699#49145699

citation 1[@noauthor_bookdown_2019] citation 2 @noauthor_bookdown_2019

citation 3[@ccjou2009] citation 4 @ccjou2009

## bookdown environment for definition, theorem, proof

https://bookdown.org/yihui/rmarkdown/bookdown-markdown.html

::: {.theorem #label name="Theorem Name"}
Here is my theorem.
:::

::: {.proof name="Proof Name"}
Here is my proof.
:::

::: {.theorem #pyth name="Pythagorean theorem"}
For a right triangle, if $c$ denotes the length of the hypotenuse
and $a$ and $b$ denote the lengths of the other two sides, we have

$$a^2 + b^2 = c^2$$
:::

::: {.definition #unnamed-chunk-2 name="Definition Name"}
Here is my definition.
:::
