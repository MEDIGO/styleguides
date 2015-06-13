# SCSS Style Guide

This is the MEDIGO SCSS Style Guide.

It is inspired in the [Github's Primer Guidelines](http://primercss.io/guidelines/)
and the [Google's HTML & CSS Style Guide](http://google.github.io/styleguide/htmlcssguide.xml)

## Table of Contents

1. [Comments](#comments)
1. [Naming](#naming)
1. [Nesting](#nesting)
1. [Properties](#properties)
1. [Specificity](#specificity)
1. [Values](#values)
1. [Whitespace](#whitespace)

## Comments

* Use // for comments.

```scss
// bad
/* this is an example */

// good
// this is an example
```

## Naming

* Use meaningful or generic names.

```scss
// bad
#yee-1901 {}
.button-green {}

// good
#gallery {}
.aux {}
```

* Use names that are as short as possible but as long as necessary.

```scss
// bad
#navigation {}
.atr {}

// good
#nav {}
.author {}
```

* Separate words in names by a hyphen.

```scss
// bad
#demoimg {}
.error_status {}

// good
#demo-img {}
.error-status {}
```

## Nesting

* Avoid unnecessary nesting.

```scss
// bad
.flash {
  padding: 15px;

  .flash-msg {
    margin-top: 15px;
  }
}

// good
.flash {
  padding: 15px;
}

.flash-msg {
  margin-top: 15px;
}
```

## Properties

* Alphabetize properties within rule declarations.

```scss
// bad
text-align: center;
text-indent: 2em;
color: black;
background: fuchsia;

// good
background: fuchsia;
color: black;
text-align: center;
text-indent: 2em;
```

* Use shorthand properties where possible.

```scss
// bad
padding-bottom: 2em;
padding-left: 1em;
padding-right: 1em;
padding-top: 0;

// good
padding: 0 1em 2em;
```

## Specificity

* Use IDs for elements that occur exactly once inside a page.

```scss
// bad
.signup-form {}

// good
#signup-form {}
```

## Values

* Omit unit specification after "0" values.

```scss
// bad
margin: 0px;

// good
margin: 0;
```

* Use lowercase hexadecimal color values.

```scss
// bad
color: #FFF;

// good
color: #fff;
```

* Use 3 character hexadecimal notation where possible.

```scss
// bad
color: #eebbcc;

// good
color: #ebc;
```

## Whitespace

* Use soft-tabs with a two space indent.

```scss
// bad
h1 {
∙∙∙∙color: black;
}

// good
h1 {
∙∙color: black;
}
```

* Put spaces after `:` in property declarations.

```scss
// bad
color:black;

// good
color: black;
```

* Put spaces before `{` in rule declarations.

```scss
// bad
h1{}

// good
h1 {}
```

* Put line breaks between rulesets.

```scss
// bad
h1 {
  color: black;
}
p {
  color: white;
}

// good
h1 {
  color: black;
}

p {
  color: white;
}

```

* When grouping selectors, keep individual selectors to a single line.

```scss
// bad
h1, h2, h3 {
  color: black;
}

// good
h1,
h2,
h3 {
  color: black;
}
```

* Each property declaration should appear on its own line for more accurate error reporting.

```scss
// bad
h1 {
  color: black; font-weight: normal;
}

// good
h1 {
  color: black;
  font-weight: normal;
}
```
