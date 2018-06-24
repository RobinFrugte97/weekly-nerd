# SCSS

[SCSS](https://sass-lang.com/documentation/file.SASS_REFERENCE.html) is a CSS extension. It exist for to the convenience of the developer. SCSS adds a lot of functionality to CSS. Everything you ever dreamed of; it's all possible with SCSS. You can declare variables for your convenience, make nesting a LOT easier and use Mixins so you can re-used defined styles throughout your project.

## Why SCSS?

As stated before, SCSS can make writing CSS a lot easier and faster. One alternative way to write easier CSS is SASS. While SCSS and SASS are virtually the same, I personally find SCSS to have a bit more clarity.

SCSS:
``` scss
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```

SASS:
``` sass
nav
  ul
    margin: 0
    padding: 0
    list-style: none

  li
    display: inline-block

  a
    display: block
    padding: 6px 12px
    text-decoration: none
```

SASS looks cleaner than SCSS, but when you just start off with a CSS extension, you might find SCSS to be easier as it resembles CSS more closely.

## Some features

### Variables

It's real easy to declare and use variables in SCSS. You use the `$` sign to declare the variable, like this:

``` scss
$primary-color: #333
```

In this case, `$primary-color` is ready to be used.

Variables are used like this:

``` scss
color: $primary-color
```

By using variables you only have to change your code in the declaration of the code.

### Nesting

In CSS you tend to get really long selectors. SCSS nesting can prevent that.

Instead of:

``` CSS
nav>ul {
  width: 5rem;
}
nav>ul>li {
  font-size: 1rem;
}
```

You can nest it:

``` scss
nav {
  ul{
    width: 5rem;

    li {
      font-size: 1rem;
    }
  }
}
```

This way you can keep your code real clean and easy to follow.
