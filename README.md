# Linters and code style guides

Here we define our code style guides.

Repo is on:

<https://github.com/trkin/linters_and_code_style_guides>

## Ruby Style Guides

For Ruby we are following

* <https://github.com/thoughtbot/guides/tree/main/ruby>
* <https://github.com/Shopify/ruby-style-guide>
* <https://github.com/airbnb/ruby>

## Standard

For automated way of controlling code styles we use
[Standard](https://github.com/testdouble/standard) which uses Rubocop underneath
and it is installed with those commands:
```
bundle add standard

cat > .rubocop.yml <<HERE_DOC
# https://github.com/trkin/linters_and_code_style_guides/blob/main/.rubocop.yml
require: standard

inherit_gem:
  standard: config/base.yml
HERE_DOC

cat > .standard.yml <<HERE_DOC
# https://github.com/trkin/linters_and_code_style_guides/blob/main/.standard.yml
ignore:
  - "**/*":
    # It's OK to put comma after each line {a:1,}
    - Style/TrailingCommaInHashLiteral
HERE_DOC
```

## Erb lint

TODO: https://github.com/Shopify/erb-lint

# General text syntax

* labels on buttons, titles,...  should be upper case with no period: `This Job
Is Paused`
* sentences on error messages, flash messages...  should have period at the end:
`Job has been copied successfully.`

## Commit message

<https://github.com/GsActions/commit-message-checker>

```
```
