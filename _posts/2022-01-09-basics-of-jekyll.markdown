---
layout: single
title:  "Basics of starting your Jekyll Blog"
date:   2022-01-09 10:12:48 +0800
categories: jekyll
---
Preface: This blog contains basic codes to maintain a Jekyll Blog :)

Reference: [https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)

Content: 

1. Build A New Blog
2. Start A New Post
3. Watch Out the Font
5. Push Your Post to GitHub
5. The Use of Chinese Language



### Build A New Blog

- Build A New Blog 

  ```
  jekyll new LYCBlog
  ```

- Change Your Directory

  ```bash
  cd LYCBlog
  ```

- Start Your Project

  ```bash
  bundle exec jekyll serve
  ```



### Start A New Post

When comes to generate a new post, come to ==_posts== file, and build a new markdown file. Note that the name of markdown files should be `yy-mm-dd-filename.markdown` format.

A recommended Front Matter Defaults seem like:

```css
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: true
      read_time: true
      comments: true
      share: true
      related: true
```



### Watch Out the Font

According to the [reference website](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/), the _sass file have a structure as:

```css
minimal-mistakes
├── _sass
|  └── minimal-mistakes
|     ├── vendor               # vendor SCSS partials
|     |   ├── breakpoint       # media query mixins
|     |   ├── magnific-popup   # Magnific Popup lightbox
|     |   └── susy             # Susy grid system
|     ├── _animations.scss     # animations
|     ├── _archive.scss        # archives (list, grid, feature views)
|     ├── _base.scss           # base HTML elements
|     ├── _buttons.scss        # buttons
|     ├── _footer.scss         # footer
|     ├── _masthead.scss       # masthead
|     ├── _mixins.scss         # mixins (em function, clearfix)
|     ├── _navigation.scss     # nav links (breadcrumb, priority+, toc, pagination, etc.)
|     ├── _notices.scss        # notices
|     ├── _page.scss           # pages
|     ├── _print.scss          # print styles
|     ├── _reset.scss          # reset
|     ├── _sidebar.scss        # sidebar
|     ├── _syntax.scss         # syntax highlighting
|     ├── _tables.scss         # tables
|     ├── _utilities.scss      # utility classes (text/image alignment)
|     └── _variables.scss      # theme defaults (fonts, colors, etc.)
├── assets
|  ├── css
|  |  └── main.scss            # main stylesheet, loads SCSS partials in _sass
```

What you need to do is to open the file `_variables.scss`, and then locate the codes here:

```html
/* serif typefaces */
$georgia: Georgia, serif !default;
$times: Times, serif !default;
$bodoni: "Bodoni MT", serif !default;
$calisto: "Calisto MT", serif !default;
$garamond: Garamond, serif !default;

$global-font-family: Times;
$header-font-family: Georgia;
$caption-font-family: Georgia;

```

Change the content in `XXX-font-family`, then you can change the font here.

### Push Your Post to GitHub

```bash
git pull
git add .
git commit -m "submit your comment"
git push origin master
```



### The Use of Chinese Language

See this [page](https://y-c-li.github.io/lyc.github.io/jekyll/Try-a-Chinese-Post/).