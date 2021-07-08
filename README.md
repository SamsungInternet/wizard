Samsung Internet Security Wizard
================================

The goal of this is to provide a guide to help people browse the Web Securely.

Some of the features are Samsung Specific.

## Folders

* Assets: Images and Videos, language specific assets should be in a sub folder represented by their i18n code e.g. `assets/es`, `assets/en`, `assets/kr`
* Pages: Pages are used to hold each page of content in the wizard. Each markdown file in the wizard is displayed in alphabetical order so keep the pages numbered e.g. `01 intro.md`

## Files

Each language file e.g. `/en.md` loads all the content from a particular folder and displays them as pages here is what these files should look like:

```markdown
---
title: Security and Privacy Wizard
layout: 'index'
pages: 'pages/en'
lang_label: 'English'
desc: 'This guide will help you make Samsung Internet be as secure as possible and explain how it protects you.'
---
```

* The `pages` field picks the folder from which the content should be loaded, they are loaded in alphabetical order
* The `title` and `desc` fields are used for SEO and social media.
* The `layout` field is to be left alone it just says that this uses the template called index
* the `lang_label` field should be the language of the page it is loaded according to the region it was loaded from so that people can find it in the language picker

## Building

This uses GitHub pages so there is no build step needed. Changing the files on GitHub will automatially
generate the web site.

## Testing locally

To test your changes locally before merging them you can install Jekyll locally which is what GitHub pages uses.

* Install ruby and [Install Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)
* Run with jekyll: `jekyll run serve`
* Open up localhost:4000 in your browser

## Adding a new language

Here are the steps for adding a new language:

Duplicate the folder language you want to translate from in `pages/` e.g. `pages/en/` to `pages/kr/`

For the files in the folder the filename is only used for the order of the pages, in alphabetical order, so rename however you want but keep the numbers at the start.

Duplicate `en.md` in the root of the repo. Rename it to the country code for your language. E.g. `kr.md`

In this file translate `title` and `desc` and set `pages` to the location of your new folder. E.g. `pages/kr/`

You are welcome to use the assets from another language but it may be better for your users if you reproduce the assets from a region & language correct device to ensure it makes sense for the readers.
