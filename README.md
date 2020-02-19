visit the [SCI Knowledge Base homepage](https://visualengineers.github.io/sci-knowledge-base/)

## Documentation

Whenever committing to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages. Jekyll uses the Liquid templating language to process templates, providing a number of useful Liquid additions to build the site (e.g. filters and tags). See the official [Liquid Documentation](https://shopify.github.io/liquid/basics/introduction/) to learn more.

### Markdown

Markdown makes it easy to style your writing. It includes conventions for

```markdown
Syntax highlighted code block
```

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

![Images](https://publicdomainvectors.org/photos/Placeholder.png =150x150 )
title and image ratio are optional

[Links](url) 

If you stumble upon a **broken link**, it it very likely you forgot to prepend the baseurl of the site (which is not automatically rendered).
Try `{{ site.baseurl }}/your-link` or `{{ site.baseurl }}/{{ custom-page.url }}` or `{{ custom-page.url | prepend: site.baseurl }}`
You can check the baseurl settings in the `_config.yml` configuration file.

More fancy markdown: [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Custom responsiveness shortcodes 

Vimeo (use media-wrapper class)
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>`

YouTube (use media-wrapper class)
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`

Images (use responsive-media class)
`![ title ]( src ){:.responsive-media}`

### Jekyll Themes

The name of the theme is stored in the Jekyll `_config.yml` configuration file. You can either choose from one of the supported themes or use a remote-theme. To enable a theme:

`theme: theme-name` OR `remote_theme: "author/theme-name"`

The current theme is the remote theme `vsoch/docsy-jekyll`. Custom modifications to the remote theme include the sidebar and navigation functionality, additional layout templates and includes, custom styling as well as data storage and queries.

### Jekyll Plugins

...

### Support

 [Github Pages documentation](https://help.github.com/categories/github-pages-basics/)
