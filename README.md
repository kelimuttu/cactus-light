# Cactus Light

A responsive, light and simple [Hexo](http://hexo.io) theme for a personal website.

:cactus: [Demo](https://kelimuttu.github.io/cactus-light/)

![cactus-light](https://pageshot.net/images/e8179e0b-cad7-402b-a6a2-6ef1ea7443e5.png)

## Summary

- [General](#general)
- [Features](#features)
- [Install](#install)
- [Configuration](#configuration)
- [License](#license)

## General

- **Version** : 2.0
- **Compatibility** : Hexo 3 or later

## Features

- Fully responsive
- Disqus
- Googe analytics
- Font Awesome icons
- Pick your own code highlighting scheme
- Configurable navigation menu
- Projects list
- Simplicity

## Install
1. In the `root` directory:

    ```git
    $ git clone https://github.com/kelimuttu/cactus-light.git themes/cactus-light
    $ npm install hexo-pagination --save
    ```

2. Change the `theme` property in the `config.yml` file.

    ```yml
    # theme: landscape
    theme: cactus-light
    ```

3. Run: `hexo generate` and `hexo server`

## Configuration

### Navigation

Setup the navigation menu in the theme's `_config.yml`:

  ```
  nav:
    Home: /
    About: /about/
    Articles: /archives/
    Contact: /contact/
    LINK_NAME: URL
  ```

### RSS

Set the `rss` field in the theme's `_config.yml` to one of the following values:

1. `rss: false` will totally disable rss (default).
2. `rss: atom.xml` sets a specific feed link.
3. `rss:`leave empty to use the [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed) plugin. 

### Analytics

Add you Google Analytics `tracking_id` to the theme's `_config.yml`.

  ```
  plugins:
      gooogle_analytics: 'UA-49627206-1'            # Format: UA-xxxxxx-xx
  ```

### Comments

First, create a site on Disqus: [https://disqus.com/admin/create/](http://disqus.com/admin/create/).

Next, update the theme's `_config.yml` file:

  ```
  plugins:
      disqus_shortname: SITENAME
  ```

where `SITENAME` is the name you gave your site on Disqus.

### Code Highlighting

Pick one of [the available colorschemes](https://github.com/probberechts/cactus-dark/tree/master/source/css/_highlight) and add it to the theme's `_config.yml`:

  ```
  customize:
      highlight: COLORSCHEME_NAME
  ```

## License
MIT
