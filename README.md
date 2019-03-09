# Bootstrap Blog Theme in ejs for Cogear.JS

This is a simple theme with blog posts on the home page and a responsive design based on [Bootstrap](https://getbootstrap.com) v4. Tags support and pagination.

![screenshot](https://github.com/dtslvr/cogear-theme-ejs-bootstrap-blog/raw/master/screenshot.png)

# Installation

## Preset

There is a ready to use blog preset for the `ejs-bootstrap-blog` theme. Just clone the [repository](https://github.com/dtslvr/cogear-preset-ejs-bootstrap-blog), install the dependencies and run the project.

## Manual Installation

Install [`cogear-plugin-blog`](https://github.com/codemotion/cogear-plugin-blog) first to use this theme.

Go to the site folder and install the theme:
```bash
npm install cogear-theme-ejs-bootstrap-blog
```

or

```bash
yarn add cogear-theme-ejs-bootstrap-blog
```

After that, edit your site's `./config.yaml` to set up the installed theme.

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
  index: ""
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

# Further reading

Find more information in the official [Cogear.JS](https://cogearjs.org) documentation: https://cogearjs.org/docs
