---
day: '107'
title: Hugo/ Netlify Blog
date: 2018-01-21T10:04:46.351Z
tags:
  - 100daysofcode
  - hugo
  - netlify-cms
  - javascript
  - html
  - css
categories: code
weight: 0
---
# Day 107

## Today's Progress

Worked on my blog some more. Couldn't figure out how to add to site variables from CMS.

## Thoughts

I posted a question on [SO](https://stackoverflow.com/questions/48365670/add-to-site-variables-from-cms) and [Hugo forums](https://discourse.gohugo.io/t/add-to-site-variables-from-cms/10111):  

> I'm using the [Forty Theme](https://github.com/MarcusVirg/forty) and the `config.toml` file has a Tiles section as follows:
>
> ```
> # Tiles Section
> [params.tiles]
> enable = true
>
>  # Display your showcases here.
>   [[params.tiles.showcase]]
>   title = 
>   subtitle = 
>   image = 
>   url = 
> ```
>
> I want to be able to add entries to the tiles section from CMS. How do I add variables to `params.tiles.showcase` from CMS? Here's a snippet from my `config.yml`
>
> ```
> collections:
>   - name: "blog"
>     label: "Blog post"
>     folder: "post/"
>     create: true
>     fields:
>       - { label: "Title", name: "title" }
>       - { label: "Publish Date", name: "date", widget: "datetime" }
>       - { label: "Description", name: "description", widget: > "markdown", required: false }
>       - { label: "Featured Image", name: "image", widget: "image", > required: false }
>       - { label: "Body", name: "body", widget: "markdown", required: false }
> ```

## Links

* [Add to site variables from CMS (Stack Overflow)](https://stackoverflow.com/questions/48365670/add-to-site-variables-from-cms)
* [Add to site variables from CMS (Hugo Forums)](https://discourse.gohugo.io/t/add-to-site-variables-from-cms/10111)
