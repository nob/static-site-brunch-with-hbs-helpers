# static-site-brunch (with Handlebars helpers)

Static site support for [Brunch](http://brunch.io/).

This is a fork of [static-site-brunch](https://www.npmjs.com/package/static-site-brunch)

Only {#if_eq} helper is added, currently.

## Install

```
npm install --save static-site-brunch-with-hbs-helpers
```

## Usage

Add Handlebars templates to `app/templates` and they will be automatically
compiled and placed in your `public` directory.

Partials are automatically registered if they begin with an underscore, e.g.
`_hello.hbs`.

YAML front matter allows you to control the context passed to the template
during render.

## Example

```
---
people:
  - name: Devin
  - name: Kevin
---
{{#each people}}
  Hello {{name}}
{{/each}}
```
