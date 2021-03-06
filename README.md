This documentation explains the general setup of the [Shape-Changing Interfaces Knowledge Base](https://visualengineers.github.io/sci-knowledge-base/)(SCI-KB), which individual changes were made to the template and how you can participate.

## General Setup

Whenever committing to this repository, GitHub Pages will run the static site generator [Jekyll](https://jekyllrb.com/docs/) to rebuild the pages. Jekyll uses the [Liquid](https://shopify.github.io/liquid/basics/introduction/) templating language to process templates, providing a number of (really) useful Liquid additions to build the site such as filters to insert content automatically. 

**Themes**. You can either choose from one of the supported themes or use a remote-theme. Its name is stored in the Jekyll `_config.yml` configuration file via:

`theme: theme-name` OR `remote_theme: "author/theme-name"`

The current theme is the remote theme `vsoch/docsy-jekyll`. Custom modifications to the remote theme include the sidebar and navigation functionality, additional layout templates and includes, custom styling as well as data storage and queries.

**Markdown**. Unless you don't have any super special requests, Markdown makes it easy to style your writing. It includes conventions for syntax highlighted code blocks, headlines, lists, font styles and simplifies the insertion of images and links. 

If you stumble upon a **broken link** in SCI-KB, check if the baseurl of the site is prepended. (which is not automatically rendered). You can check the baseurl settings in the `_config.yml` configuration file. Quick fix: 

`{{ site.baseurl }}/your-link` or `{{ site.baseurl }}/{{ custom-page.url }}` or `{{ custom-page.url | prepend: site.baseurl }}`

More fancy markdown: [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

**Kramdown**. Not yet satisfied? Kramdown is the default Markdown renderer for Jekyll, offering you additional options for styling. Add for example `{:.my-css-class}` to tell Kramdown you want to apply your fancy custom CSS.

## SCI-KB Specials

These path specifications and reusable code snippets are special for the SCI-KB. They have been created to structure the knowledge base and facilitate the insertion of new content.

### Inserting Knowledge
We're glad you want to join in! What type of content do you want to insert?

- **References & Links** 
Create a new entry in `data > references.yml` or `data > links.yml`. The sorting will be in alphabetical order automatically.

- **Best Practices, Terms & Concepts and other pages**  
Create a new markdown file (.md) in `best-practices`, `terms` (place under first letter), `concepts` or `pages` by copying an existing page (to make sure all styles are applied). To enable users to search for content on specific topics, Best Practices, Terms and Concepts should be assigned to 1 of the 4 topics (design, society, technology, user experience). For example, to assign a knowledge item to User Experience, go to the top of the markdown file and type (downcase): `category: user experience`. It will then be tagged and shown in User Experience collections.

- **Images**  
Upload images into `assets > img`. 

### Linking To Knowledge
Do you want to reference your content or did you discover a missing link? You can link content in markdown pages with the following syntax.

- **Reference**    
`[[title]](({{ site.baseurl }}/resources/#references)`

- **Link**  
`[[title]](({{ site.baseurl }}/resources/#links)`

- **Page**    
`[title]({{ site.baseurl }}/[filename-goes-here])`

- **Term**    
`[title]({{ site.baseurl }}/terms/[filename-goes-here])`

- **Concept**    
`[title]({{ site.baseurl }}/concepts/[filename-goes-here])`

### Adding Media To A Page Like A Pro

These code snippets ensure that media content looks good everywhere. (Even if the photos look like crap...no, we're afraid not.)

- **Video on Vimeo**     
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>`

- **Video on YouTube**  
`<div class="media-wrapper"><iframe src="..." frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`

- **Image**  
`![title](source){:.responsive-media}` 

- **Banner Image**  
To add a full-width banner image (works for best practice & concept), you can specify the image source and credits at the page's head like this: `image: /path-to-image or external-url` and `image-credits: ...some markup or plain text...` The image will be inserted automatically at the top of a page and used as preview image in best practice / concept overview also. Have a look at an existing best practice or concept if you need an example.

### Other

- **Accordion**  
Who doesn't love accordions? Accordions will automatically be rendered in custom SCI-KB style. With `markdown="1"`, markdown can be rendered inside of our `<details>` html block level tag. Remove `open` if you would like the accordion to be closed by default.
`<details markdown="1" open>`  
`<summary><h3>Title</h3></summary>`  
`... content goes here ...`  
`</details>`

- **Quiz**
For any term, concept, or best practice, you can insert a quiz. To do so, place a .yml file inside the data/quizzes folder and insert one or more questions as shown in the example.yml. Name your file using the title of the page on which the quiz should appear (but downcased and hyphens instead of whitespaces, e.g. "3D Printing" becomes "3d-printing"). No further action needed, the quiz will be inserted automatically. 

### Support
Helpful links for all who have not yet enough or further questions.

- [Github Pages documentation](https://help.github.com/categories/github-pages-basics/)  
- [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/)  
- [Testing your site locally](https://kbroman.org/simple_site/pages/local_test.html)    
- [Jekyll Documentation](https://jekyllrb.com/docs/)     
- [Liquid Documentation](https://shopify.github.io/liquid/basics/introduction/)  
