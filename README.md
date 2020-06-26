visit the [SCI Knowledge Base homepage](https://visualengineers.github.io/sci-knowledge-base/)

## Documentation

Whenever committing to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages. Jekyll uses the Liquid templating language to process templates, providing a number of useful Liquid additions to build the site (e.g. filters and tags). See the official [Liquid Documentation](https://shopify.github.io/liquid/basics/introduction/) to learn more.

### Jekyll Theme

The name of the theme is stored in the Jekyll `_config.yml` configuration file. You can either choose from one of the supported themes or use a remote-theme. To enable a theme:

`theme: theme-name` OR `remote_theme: "author/theme-name"`

The current theme is the remote theme `vsoch/docsy-jekyll`. Custom modifications to the remote theme include the sidebar and navigation functionality, additional layout templates and includes, custom styling as well as data storage and queries.

### Markdown

Markdown makes it easy to style your writing, including conventions for 

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

![Images](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSG5V-M6OvkJBvdLyY-zUSFBii4qqR9f5O7HWq4GAygHFZ5sjxm)

[Links](url) 

If you stumble upon a **broken link**, it is very likely you forgot to prepend the baseurl of the site (which is not automatically rendered). You can check the baseurl settings in the `_config.yml` configuration file. Fix: 

`{{ site.baseurl }}/your-link` or `{{ site.baseurl }}/{{ custom-page.url }}` or `{{ custom-page.url | prepend: site.baseurl }}`

More fancy markdown: [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Kramdown

Not yet satisfied? Kramdown is the default Markdown renderer for Jekyll, offering you additional options for styling. Add for example `{:.my-css-class}` to tell Kramdown you want to apply your fancy custom CSS.

### Inserting new content

## References & Links

Create a new entry in `data > references.yml` or `data > links.yml`. 

## Pages, Terms & Concepts

Create a new markdown file (.md) in `pages`, `terms > [first letter of entry]` or `concepts` analogous to the existing entries to make sure all styles are applied.

## Images

You can upload the image into `assets > img` or reference external urls. 
To add a full-width banner image (for best practice or concept) specify the source with "image: /path-to-image or external-url". The image will be inserted automatically at the top of a page and used as preview image.

## Linking shortcodes

Reference
`[[title]](({{ site.baseurl }}/resources/#references)`

Link
`[[title]](({{ site.baseurl }}/resources/#links)`

Page
`[title]({{ site.baseurl }}/[filename-goes-here])`

Term
`[title]({{ site.baseurl }}/terms/[filename-goes-here])`

Concept
`[title]({{ site.baseurl }}/concepts/[filename-goes-here])`

Video on Vimeo 
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>`

Video on YouTube
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`

Image
`![title](source){:.responsive-media}`


### Support

 [Github Pages documentation](https://help.github.com/categories/github-pages-basics/)
 [testing your site locally](https://kbroman.org/simple_site/pages/local_test.html)
