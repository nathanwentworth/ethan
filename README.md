# Ethan Thibault's Website

## Introduction

This is a pretty straightforward Jekyll theme, all customization is in `/css/app.scss` and `_config.yml`. 

## Configuration

Editing your `_config.yml` should be your first step. This contains global variables such as the site title, tagline, portrait image, contact info, etc. `textlinks` and `imagelinks` are both key/value pair arrays that populate the header and footer links. Try to keep them both in the same format they are currently. `imagelinks` pulls the images from the `/img/social/` folder, so place images in there to use them. 

The `app.scss` file in `/css/` will be what you use to edit things about the appearance itself. `$primary-color` is the main theme color used for titles, links, underlines, highlight, etc. `$secondary-color` is what is used for link hover. `$background-color` is for the background color. `$max-width` sets the maximum width of the site (I don't entirely recommend changing that one. Not much should be negatively affected, but I think the design works best at 960px). `$border-radius` isn't used for much anymore, but it currently sets the corner radius of the "Read More" buttons. If you want to put in any css overrides, simply put them below `@import "main";`. Anything under that will override the site styles. 

## Posts/Entries

Each post or entry is in one of three folders, and therefore collections: _interactive, _writing, or _other. Each title is relatively self-explanitory, interactive being for interactive projects, writing being for externally hosted writing pieces, and other being for anything you might want featured, but not fitting either category. Interactive is the only thing that generates pages, writing and other both do not generate html pages. 

### Variables

There are a few key variables that are required, or at least heavily encouraged for each entry. 

#### Required Variables

* title: "Here is the title"
  - The title of the post. This is displayed on gallery/home pages, as well on the generated html of interactive pages.
* ext_url: "https://website.com"
  - This is *not* required for interactive projects, but this is what you are linking to for things like writing and other, which don't generate pages.

#### Optional Variables

* image: "AfJ4lN7CIAA2oGY.jpg"
  - The key image of the post. Just like the title, this is displayed on the gallery/home pages, as well on the generated html of interactive pages.
* excerpt: "An excerpt"
  - This overrides the default excerpt variable, which is pulled from the first paragraph of content of the post. This can be useful for interactive projects. Keep in mind, this does not allow for markdown parsing.
* featured: true
  - This is what puts a project on the front page. You can either set it to false or just remove it to remove the post from the front page. 
* no_year: true
  - Use this if you don't want to display the year next to the title
* hide_title: true
  - Use this if you don't want to display the title at all. 


