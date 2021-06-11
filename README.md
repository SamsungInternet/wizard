Samsung Internet Security Wizard
================================

The goal of this is to provide a guide to help people browse the Web Securely.

Some of the features are Samsung Specific.

## Testing locally

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
