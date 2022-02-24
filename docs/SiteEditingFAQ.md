---
title: FAQ for site editing 
has_children: true
nav_order: 1000
---

# FAQ for site editing 

You can use the [editor on GitHub](https://github.com/KahunaDev/kahunadev.github.io/edit/main/docs/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

## Site content editing examples

You can find a few short guideline on site editing:
- [Markdown syntax](./site/editing/MarkdownTextEditingGuidelines.md)
- [Mermaid syntax](./site/editing/MermaidDiagramEditingGuidelines.md)


## Jekyll Themes
Currently the doucmentation is generated using the following Jekyll theme:
```
remote_theme: pmarsceill/just-the-docs
```

Reasons:
- pretty :)
- generates a TOC sidebar based on YML frontmatter added to the very beginning of files


##  Pages configuration in _config.yml
Among other things, the name of this theme is saved in the Jekyll `_config.yml` configuration file:
````yml
remote_theme: pmarsceill/just-the-docs
title: KahunaDev.io test Pages served from GitHub
description: Description: KahunaDev.io test Pages served from GitHub
````

