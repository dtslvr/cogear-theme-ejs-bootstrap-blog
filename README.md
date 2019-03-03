# Cogear.JS blog theme with bootstrap in ejs

Theme with blog posts on the home page.

Simple responsive design based on Bootstrap v4. Posts tags support and pagination.

# Installation

You need to install [`cogear-plugin-blog`](https://github.com/codemotion/cogear-plugin-blog) to use this theme.

Go to the site folder and install theme with command:
```bash
yarn add cogear-theme-ejs-bootstrap-blog
# or
npm install cogear-theme-ejs-bootstrap-blog
```

After that, you need to edit your site `config.yaml` to set up installed theme.

```yaml
theme: ejs-bootstrap-blog
```

# Configuration

Use `cogear-plugin-blog` options in `./config.yaml`:
``` yaml
title: Blog | Cogear.JS – modern static websites generator
description:
keywords:
theme: ejs-bootstrap-blog
blog:
  index: "" # Provide posts to index page
  regex: "^p/"
  tagUri: "tag"
  perPage: 5
pages:
  ^p/:
    layout: post
    author:
     login: User
     avatar: "https://www.gravatar.com/avatar/400caf343d3bab57ab93f63e21a12be7?s=24"
     link: https://cogearjs.org
```

# Docs

More info: [https://cogearjs.org/docs/themes](https://cogearjs.org/docs/themes)
