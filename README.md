# Dracula Hugo

Clean and minimal personal blog and portfolio theme for Hugo (forked from Ezhil's Hugo theme).

![Screenshot](images/screenshot)

## Features

* Clean and minimal
* Clean Dracula colorscheme
* Responsive
* Supports tags
* Social media links
* Syntax highlighting
* Hugo RSS feeds

## Installation

From your Hugo site run the following.

```sh
cd themes
git clone https://github.com/dek1ber/draculaHugo.git
```

For more information read the [official setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Configuration

```toml
baseURL = "http://example.org/"
languageCode = "en-us"
title = "My personal blog"
theme = "draculaHugo"

copyright = "© Copyright notice"

# Enable syntax highlighting.
pygmentsstyle = "solarized-dark"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true

# Number of posts to show in recent posts list (Optional). Defaults to 10.
paginate = 10

[params]
    # Blog subtitle which appears below blog title. Supports markdown.
    subtitle = "Clean and minimal personal [blog theme for Hugo](https://github.com/vividvilla/ezhil)"

    # Specify favicon (icons/i.png maps to static/icons/i.png). No favicon if not defined.
    favicon = "icons/myicon.png"

# Main menu which appears below site header.
[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4

# Social media links which shows up on site header.
# Uses feather icons for icons. You can [search icon names from here](https://feathericons.com/).
[[params.social]]
name = "Github"
icon = "github"
url = "https://github.com/vividvilla/ezhil"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://twitter.com/gohugoio"

# Enable tags.
[taxonomies]
   tag = "tags"
```

## Content layout

You can specify content type with field `type` in your content. For example static pages can be set as type `page` which are excluded from recent posts and all posts page. You can use site params `mainSections` and `disableDisqusTypes` to control which page types are excluded from recent posts and Disqus comments respectively.

```md
---
title: "About"
date: 2019-04-19T21:37:58+05:30
description: "description"
tags: ["tags"]
---

This is some static page where you can write about yourself.
```


## Credits

* [Feather Icons](https://feathericons.com/)
* [Zen habits](https://zenhabits.net/) for demo content
* [Ezhil](https://github.com/vividvilla/ezhil) for not only inspiration but the actual theme fork as well
