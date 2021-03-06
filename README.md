[![Documentation Status](https://readthedocs.org/projects/polkadot-wiki/badge/?version=latest)](https://polkadot-wiki.readthedocs.io/en/latest/?badge=latest)
[![Build Status](https://travis-ci.org/w3f/polkadot-wiki.svg?branch=master)](https://travis-ci.org/w3f/polkadot-wiki)

# Polkadot Wiki

This repository contains the source files for the [Polkadot wiki](https://wiki.polkadot.network).

## Running locally

Clone the repository to your local file system.

```bash
git clone https://github.com/w3f/Polkadot-wiki.git
```

Install `mkdocs` by using the `pip` package manager.

```bash
pip install mkdocs --user
```

Run `mkdocs serve` from the repository root to spawn a hot reloading development server and navigate to `localhost:8000` in a web browser.

## Publishing

The wiki is hosted on [Read the Docs](https://readthedocs.org) and is built on each published commit to the master branch on the GitHub repository.

## Styling

[Mkdocs-Material](https://squidfunk.github.io/mkdocs-material/) is used to give the wiki its sleek theme.

## Contributing

Please read over the rules for contribution at the [CONTRIBUTING](CONTRIBUTING.md) document. 

### Contributor set-up

As a contributor, you will need to run `npm i` in the local copy of your repository after your bring it down.

### Adding a new page

If you add a page please ensure that you give it the correct placement in the navigation by manually inputting it in the `mkdocs.yml` under the `nav` field. It is done in this way in order to have more control in how pages are displayed on the UI and give better organization to topics. 

### Spellchecking

We set [`husky`](https://github.com/typicode/husky) hooks up to catch spelling errors. If you are being prevented from committing, just run `npm run spellcheck:interactive` to use the interactive debugger and fix your spelling.
