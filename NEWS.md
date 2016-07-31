NEWS
====


# janitor 0.1.0.9000

## Features

### Major
* `crosstab()` can be called in a `%>%` pipeline, e.g., `mtcars %>% crosstab(cyl, gear)`.  Thanks to [@chrishaid](https://github.com/chrishaid) [(#34)](https://github.com/sfirke/janitor/pull/34)
* `tabyl()` can also be called in a `%>%` pipeline, e.g., `mtcars %>% tabyl(cyl)` [(#35)](https://github.com/sfirke/janitor/issues/35)
* added `use_first_valid_of()` function [(#32)](https://github.com/sfirke/janitor/issues/32)

### Minor

* `crosstab()` returns 0 instead of NA when there are no instances of a variable combination.
* A call like `tabyl(df$vecname)` retains the more-descriptive `$` symbol in the column name of the result - if you want a legal R name in the result, call it as `df %>% tabyl(vecname)`
* Single and double quotation marks are handled by `clean_names()`

## Bug fixes

*

## Package management

* Added codecov to measure test coverage
* Added Travis-CI for continuous integration

# janitor 0.1 (Release date: 2016-04-17)

* Initial draft of skeleton package on GitHub