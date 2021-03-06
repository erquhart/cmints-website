---
title: Pages
description: Learn about pages structure and how to create pages in <fix>CMintS</fix> using <fix>Markdown</fix>, <fix>ejs</fix> and <fix>HTML</fix>.
navTitleId: nav-doc-title-overview
topicTitle: nav-doc-title-pages
showDocNav: true
showTOC: true
showEdit: documentation/pages/index.md
showTranslate: 150
---

{pages-p[Paragraph in 'Pages' section]
Actual content of the website goes to the <fix>**src/pages**</fix> directory. Content can be
written using Markdown(default), EJS(Complex pages) and HTML. The folder
structure inside of the pages directory reflect actual path when the page is
requested, so for example if you consider the structure below and would like to
request src/pages/about/team.md page you would request it through <fix>**/about/team**</fix>
path, if for example you host your website at example.com domain, that would be
<fix>`https://example.com/about/team`</fix>:
}

```bash
├── about
│   └── team.md
├── about.md
├── documentation
│   ├── getting-started
│   │   ├── configuration.md
│   │   ├── index.md
│   │   └── structure.md
│   └── i18n
│       ├── index.md
│       └── markdown.md
├── index.ejs
└── news.md
```

## Markdown

{markdown-p[Paragraph in 'Markdown' section]
In order to write page content using Markdown, just assign <fix>`.md`</fix>
extension to the file. <fix>CMintS</fix> uses <a href="http://commonmark.org/"
target="_blank" rel="noopener">CommonMark</a> in order to support Markdown pages. CommonMark is
a a strongly defined, highly compatible specification of Markdown, basically
speaking it's a Markdown, but specified. You can learn more about writing
CommonMark <a href="http://commonmark.org/help/" target="_blank" rel="noopener">here</a>.
}

## ejs

{ejs-p[Paragraph in 'ejs' section]
ejs pages are used for more complex pages, in most of the cases you probably
would prefer writing your actual content using markdown without having to
include HTML tags that will require you also managing them and not forgetting to
close when required, but when it comes to some complex landing pages sometimes
Markdown is useless. EJS is a simple templating language that lets you generate
HTML markup with plain JavaScript. You can learn more about EJS <a
href="http://ejs.co/" target="_blank" rel="noopener">here</a>. In order to create EJS page just
assign <fix>`.ejs`</fix> extension to the file.
}

## HTML

{html-p[Paragraph in 'HTML' section]
If you are reading this page you probably already familiar with HTML and you
most probably used it for your website or you might be familiar with some common
tags and terms. You should mostly cover your needs by Markdown and EJS for the
complex pages, but sometimes you might have a ready HTML page which you would
like to include as a page content in that case just assign <fix>`.html`</fix>
extension to the file.
}
