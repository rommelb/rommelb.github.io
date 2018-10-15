# Beautiful-Jekyll Theme (beautiful-jekyll-theme gem)

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/daattali/20)
[![Gem Version](https://badge.fury.io/rb/beautiful-jekyll-theme.svg)](https://badge.fury.io/rb/beautiful-jekyll-theme)

<<<<<<< HEAD
> *Copyright 2016 [Dean Attali](http://deanattali.com)*

**Beautiful-Jekyll** is a ready-to-use Jekyll theme to help you create an awesome website quickly. Perfect for personal blogs or simple project websites, with a focus on responsive and clean design. You can look at [my personal website](http://deanattali.com) to see it in use, or see examples of websites other people created using this theme [here](https://github.com/daattali/beautiful-jekyll#showcased-users-success-stories).

**This theme was developed for non-commerical purposes. For commerical usage, or if you enjoy this theme, please consider [supporting me](https://www.paypal.me/daattali/20) for the development and continuous maintenance of this template.**
=======
> *Copyright 2018 [Dean Attali](https://deanattali.com)*

**Beautiful Jekyll** is a ready-to-use template to help you create an awesome website quickly. Perfect for personal sites, blogs, or simple project websites.  [Check out a demo](https://deanattali.com/beautiful-jekyll) of what you'll get after just two minutes.  You can also look at [my personal website](https://deanattali.com) to see it in use, or see examples of websites other people created using this theme [here](#showcased-users-success-stories).

**If you enjoy this theme, please consider [supporting me](https://www.paypal.me/daattali/20) for developing and maintaining this template.**
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

<p align="center">
  <a href="https://www.paypal.me/daattali">
    <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" />
  </a>
</p>

<<<<<<< HEAD
![Screenshot](./screenshot.png)

## Prerequisites

To use this theme's gem, you need to first have a functioning Jekyll website. If you don't, there are many resources online for how to set up a Jekyll site. Here are the basic commands to get a minimal Jekyll site set up in Ubuntu:
=======
### Table of contents

- [Prerequisites](#prerequisites)
- [Build your website in 3 steps](#build-your-website-in-3-steps)
- [Add your own content](#add-your-own-content)
- [Last important thing: YAML front matter ("parameters" for a page)](#last-important-thing-yaml-front-matter-parameters-for-a-page)
- [Features](#features)
- [Creating a User Page vs a Project Page](#creating-a-user-page-vs-a-project-page)
- [Showcased users (success stories!)](#showcased-users-success-stories)
- [Advanced: local development](#advanced-local-development-using-docker)
- [FAQ and support](#faq-and-support)
- [Credits and contributions](#credits)

## Prerequisites

- You need to have a GitHub account. If you don't have one, [sign up here](https://github.com/join) - it takes one minute. This is where your website will live - if you sign up with username `johnsmith` then your website will be `https://johnsmith.github.io`.
- It would be helpful to understand what Markdown is and how to write it. Markdown is just a way to take a piece of text and format it to look a little nicer.  For example, this whole instruction set that you're reading is written in markdown - it's just text with some words being bold/larger/italicized/etc. I recommend taking 5 minutes to learn markdown [with this amazingly easy yet useful tutorial](https://markdowntutorial.com/).

## Build your website in 3 steps

Getting started is *literally* as easy as 1-2-3 :smile:
Scroll down to see the steps involved, but here is a 40-second video just as a reference as you work through the steps.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

```
$ sudo apt-get update
$ sudo apt-get install ruby ruby-dev make gcc
$ sudo gem install jekyll bundler
$ jekyll new ~/mysite
```

## Installation

To use the Beautiful-Jekyll theme, add this line to your Jekyll site's `Gemfile`:

```ruby
gem "beautiful-jekyll-theme", "1.1.1"
```

<<<<<<< HEAD
Then add this line to your Jekyll site's `_config.yml`:
=======
This will create a GitHub User page ready with the **Beautiful Jekyll** template that will be available at `https://<yourusername>.github.io` within a couple minutes.  To do this, click on *Settings* at the top (the cog icon) and there you'll have an option to rename.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

```yaml
theme: beautiful-jekyll-theme
```

And finally execute:

<<<<<<< HEAD
```
$ bundle
```

To preview your site, run `bundle exec jekyll serve` (optionally with the `--host 0.0.0.0` flag if needed) and open your browser at `http://localhost:4000`.

## Usage
=======
Another way to edit the config file (or any other file) is to use [prose.io](https://prose.io/), which is just a simple interface to allow you to more intuitively edit files or add new files to your project.

After you save your changes to the config file (by clicking on *Commit changes* as the video tutorial shows), your website should be ready in a minute or two at `https://<yourusername>.github.io`. Every time you make a change to any file, your website will get rebuilt and should be updated in about a minute or so.

You can now visit your shiny new website, which will be seeded with several sample blog posts and a couple other pages. Your website is at `https://<yourusername>.github.io` (replace `<yourusername>` with your user name). Do not add `www` to the URL - it will not work!
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

Using Beautiful-Jekyll is very simple, but you should take a few minutes to read through the features it supports to learn how to use it.

### Adding content

<<<<<<< HEAD
You can now start adding pages to your site. Beautiful-Jekyll supports three layouts: `post`, `page`, and `minimal`. In order to use Beautiful-Jekyll's template, a page must have its `layout` parameter set to one of these options in the YAML.
=======
To add pages to your site, you can either write a markdown file (`.md`) or you can write an HTML file directly.  It is much easier to write markdown than HTML, so I suggest you do that (use the [tutorial I mentioned above](https://markdowntutorial.com/) if you need to learn markdown). You can look at some files on this site to get an idea of how to write markdown. To look at existing files, click on any file that ends in `.md`, for example [`aboutme.md`](./aboutme.md). On the next page you can see some nicely formatted text (there is a word in bold, a link, bullet points), and if you click on the pencil icon to edit the file, you will see the markdown that generated the pretty text. Very easy!
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

Any blog posts (pages under the `_posts` directory) should use the `post` layout, while most other pages should use the `page` layout. You can use the `minimal` layout if you want a page with minimal styling, without the bulky navigation bar and footer.

Instead of remembering to manually add the layout parameter to every page's YAML, I recommend you add the following lines to your `_config.yml` so that all blog posts will automatically have layout `post` and all other pages will have layout `page`:

<<<<<<< HEAD
```yaml
defaults:
  -
    scope:
      path: ""
      type: "posts"
    values:
      layout: "post"
  -
    scope:
      path: ""
    values:
      layout: "page"
```
=======
As mentioned previously, you can use [prose.io](https://prose.io/) to add or edit files instead of doing it directly on GitHub, it can be a little easier that way.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

### Adding an index page

<<<<<<< HEAD
Feel free to create the index page (homepage) of your site however you'd like. If you want to have an index page similar to the one at [deanattali.com](http://deanattali.com), then create `index.html` as follows: 
=======
In order to have your new pages use this template and not just be plain pages, you need to add [YAML front matter](https://jekyllrb.com/docs/front-matter/) to the top of each page. This is where you'll give each page some parameters that I made available, such as a title and subtitle. I'll go into more detail about what parameters are available later. If you don't want to use any parameters on your new page (this also means having no title), then use the empty YAML front matter:
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

```html
---
layout: page
title: My Website
subtitle: Some short description of my site
---

<div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url }}">
      <h2 class="post-title">{{ post.title }}</h2>
        {% if post.subtitle %}
          <h3 class="post-subtitle">{{ post.subtitle }}</h3>
        {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry">
      {{ post.excerpt | strip_html | xml_escape | truncatewords: 50 }}
      {% assign excerpt_word_count = post.excerpt | number_of_words %}
      {% if post.content != post.excerpt or excerpt_word_count > 50 %}
        <a href="{{ post.url }}" class="post-read-more">[Read&nbsp;More]</a>
      {% endif %}
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {{ post.tags | join: ", " }}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}
```

You'll also need to add these lines to your `_config.yml` because the code above uses pagination:

```yaml
paginate: 5
gems:
  - jekyll-paginate
```

<<<<<<< HEAD
Make sure there is no `index.md` file (if there is one, then delete it).
=======
Many personalization settings in `_config.yml`, such as setting your name and site's description, changing the background colour/image, setting your avatar to add a little image in the navigation bar, customizing the links in the menus, customizing what social media links to show in the footer, etc.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

### Creating a navigation bar

<<<<<<< HEAD
Add these lines to your `_config.yml` file to get a demo navigation bar:   

```yaml
navbar-links:
  Home: ""
  About Me: "aboutme"
  Resources:
    - Beautiful Jekyll: "http://deanattali.com/beautiful-jekyll/"
    - Learn markdown: "http://www.markdowntutorial.com/"
    - GitHub Pages: "https://pages.github.com/"
  Author's home: "http://deanattali.com"
```
=======
If you want to enable comments on your site, Beautiful Jekyll supports either the [Disqus](https://disqus.com/) comments plugin or [Facebook](https://developers.facebook.com/docs/plugins/comments) comments.

To use Disqus, simply sign up to [Disqus](https://disqus.com/) and add your Disqus shortname to the `disqus` parameter in the `_config.yml` file.

To use Facebook comments, create a Facebook app using [Facebook developers](https://developers.facebook.com/docs/apps/register), and add the Facebook App ID to the `fb_comment_id` parameter in `_config.yml`.

If either `disqus` or `fb_comment_id` parameters are set in the configuration file, then all blog posts will have comments turned on by default. To turn off comments on a particular blog post, add `comments: false` to the YAML front matter. If you want to add comments on the bottom of a non-blog page, add `comments: true` to the YAML front matter.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

Change these values to match the pages on your site. Each menu item is composed of a `key:value` pair, where the `key` is the text that shows up in the navigation bar, and `value` is the URL to link to. The URL can either be the name of a page on your site (eg. `""` will go to your homepage, `aboutme` will go to a page called `aboutme` on your site), or a URL to an external site beginning in `http`. If you want to define sub-menus, use the format that the `Resources` menu is using in the sample code above.

<<<<<<< HEAD
#### Displaying an image in the navigation bar
=======
Beautiful Jekyll lets you easily add Google Analytics to all your pages. This will let you track all sorts of information about visits to your website, such as how many times each page is viewed and where (geographically) your users come from.  To add Google Analytics, simply sign up to [Google Analytics](https://www.google.com/analytics/) to obtain your Google Tracking ID, and add this tracking ID to the `google_analytics` parameter in `_config.yml`.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

You can add an image to the middle of the navigation bar by defining the `avatar` parameter in `_config.yml`. The image should be a square (width = height). This image will disappear once the user scrolls down in the page.

```yaml
avatar: "/path/to/image.png"
```

You can also place an image in the top-left corner of the navigation bar instead of your website's title. This is done with the `title-img` parameter in `_config.yml`:

```yaml
title-img: "/path/to/image.png"
```

### Add your name/email/social media links to the footer

You can add contact information and social media links in the footer. They will be displayed as nice little logos, to give the footer a clean feel. Add the following to your `_config.yml` file:

```yaml
author:
  name: Some Person
  email: "youremail@domain.com"
  facebook: yourname  # eg. daattali
  github: yourname    # eg. daattali
  twitter: yourname   # eg. daattali
  telephone: yourphone     # eg. +14159998888
  reddit: yourname    # eg. daattali
  google-plus: +yourname   # eg. +DeanAttali or 109424658772469020925
  linkedin: yourname  # eg. daattali
  xing: yourname      # eg. daattali
  stackoverflow: yourlink  # eg. "3943160/daattali"
  snapchat: yourname  # eg. daattali
  instagram: yourname # eg. daattali
  youtube: yourlink   # eg. user/daattali or channel/daattali
  spotify: yourname   # eg. daattali
```

Remove the lines that you don't want to display in the footer, and change `yourname` to the correct values in the links you want to keep.

#### Add an RSS feed link to the footer

You can add an icon that will link to an RSS feed of your blog by including the following parameter in `_config.yml`:

<<<<<<< HEAD
```yaml
rss-footer: true
```
=======
Parameter   | Description
----------- | -----------
title       | Page or blog post title
subtitle    | Short description of page or blog post that goes under the title
tags        | List of tags to categorize the post. Separate the tags with commas and place them inside square brackets. Example: `[personal, self help, finance]`
bigimg      | Include a large full-width image at the top of the page.  You can either give the path to a single image, or provide a list of images to cycle through (see [my personal website](https://deanattali.com/) as an example).
comments    | If you want do add Disqus comments to a specific page, use `comments: true`. Comments are automatically enabled on blog posts; to turn comments off for a specific post, use `comments: false`. Comments only work if you set your Disqus id in the `_config.yml` file.
show-avatar | If you have an avatar configured in the `_config.yml` but you want to turn it off on a specific page, use `show-avatar: false`. If you want to turn it off by default, locate the line `show-avatar: true` in the file `_config.yml` and change the `true` to `false`; then you can selectively turn it on in specific pages using `show-avatar: true`.
image       | If you want to add a personalized image to your blog post that will show up next to the post's excerpt and on the post itself, use `image: /path/to/img`.
share-img   | If you want to specify an image to use when sharing the page on Facebook or Twitter, then provide the image's full URL here.
social-share | If you don't want to show buttons to share a blog post on social media, use `social-share: false` (this feature is turned on by default).
use-site-title | If you want to use the site title rather than page title as HTML document title (ie. browser tab title), use `use-site-title: true`. When set, the document title will take the format `Site Title - Site Description` (eg. `My website - A virtual proof that name is awesome!`). By default, it will use `Page Title` if it exists, or `Site Title` otherwise.
layout      | What type of page this is (default is `post` for blog posts and `page` for other pages. You can use `minimal` if you don't want a header and footer)
js          | List of local JavaScript files to include in the page (eg. `/js/mypage.js`)
ext-js      | List of external JavaScript files to include in the page (eg. `//cdnjs.cloudflare.com/ajax/libs/underscore.js/1.8.2/underscore-min.js`). External JavaScript files that support [Subresource Integrity (SRI)](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity) can be specified using the `href` and `sri` parameters eg.<br/>`href: "//code.jquery.com/jquery-3.1.1.min.js"`<br/>`sri: "sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8="`
css         | List of local CSS files to include in the page
ext-css      | List of external CSS files to include in the page. External CSS files using SRI (see `ext-js` parameter) are also supported.
googlefonts | List of Google fonts to include in the page (eg. `["Monoton", "Lobster"]`)
gh-repo   | If you want to show GitHub buttons at the top of a post, this sets the GitHub repo name (eg. `daattali/beautiful-jekyll`). You must also use the `gh-badge` parameter to specify what buttons to show.
gh-badge  | Select which GitHub buttons to display, available options are: [star, watch, fork, follow]. You must also use the `gh-repo` parameter to specify the GitHub repo.

### Advanced features (including how to use a custom URL address for your site)

I wrote [a blog post](https://deanattali.com/2015/03/12/beautiful-jekyll-how-to-build-a-site-in-minutes/) describing some more advanced features that I used in my website that are applicable to any Jekyll site.  It describes how I used a custom URL for my site (deanattali.com instead of daattali.github.io), how to add a Google-powered search into your site, and provides a few more details about having an RSS feed.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

#### Add your website's name to the footer

After all the contact info links, you can also add the name of your website by defining the `url-pretty` parameter in `_config.yml`:

```yaml
url-pretty: "MyWebsite.com"
```

### Buttons for sharing blog posts on social media

By default, every blog post will have buttons at the bottom for sharing the page on Twitter, Facebook, LinkedIn, and Google+. If you want to disable these buttons, add these lines to your `_config.yml`:

```yaml
share-links-active:
  twitter: false
  facebook: false
  google: false
  linkedin: false
```

These settings will remove all four buttons. You can use `true` instead of `false` for any buttons that you want to keep.

<<<<<<< HEAD
### Allowing users to leave comments
=======
Want your website featured here? [Contact me](https://deanattali.com/aboutme#contact) to let me know about your website.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

If you want to enable comments on your site, Beautiful-Jekyll supports the [Disqus](https://disqus.com/) comments plugin.  To use it, simply sign up to Disqus and add your Disqus shortname (**not** the userid) to the `disqus` parameter in `_config.yml`:

<<<<<<< HEAD
```yaml
disqus: yourshortname
```
=======
| Website | Description |
| :------ |:----------- |
| [repidemicsconsortium.org/](https://www.repidemicsconsortium.org/) | R Epidemics Consortium |
| [vaccineimpact.org](https://www.vaccineimpact.org/) | Vaccine Impact Modelling Consortium |
| [derekogle.com/fishR](http://derekogle.com/fishR/) | Using R for Fisheries Analyses |
| [bigdata.juju.solutions](http://bigdata.juju.solutions) | Creating Big Data solutions Juju Solutions |
| [joecks.github.io/clipboard-actions](http://joecks.github.io/clipboard-actions/) | Clipboard Actions - an Android app |
| [deanattali.com/shinyjs](http://deanattali.com/shinyjs/) | shinyjs - an R package |
| [blabel.github.io](http://blabel.github.io) | Library for canonicalising blank node labels in RDF graphs |
| [reactionic.github.io](http://reactionic.github.io) | Create iOS and Android apps with React and Ionic |
| [ja2-stracciatella.github.io](http://ja2-stracciatella.github.io) | Jagged Alliance 2 Stracciatella |
| [ddocent.com](http://ddocent.com/) | RADSeq Bioinformatics and Beyond |
| [guitarlessons.org](https://www.guitarlessons.org/) | Free online guitar lessons for all |
| [terremotocentroitalia.info](https://www.terremotocentroitalia.info/) | Information about the 2016 Italy earthquake |

>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

### Adding Google Analytics to track page views

<<<<<<< HEAD
Beautiful-Jekyll lets you easily add Google Analytics to all your pages. This will allow you to track all sorts of information about visits to your website, such as how many times each page is viewed and where (geographically) your users come from.  To add Google Analytics, simply sign up to [Google Analytics](http://www.google.com/analytics/) to obtain your Google Tracking ID, and add this tracking ID to the `google_analytics` parameter in `_config.yml`:

```yaml
google_analytics: yourid
```
=======
| Website | Who | What |
| :------ |:--- | :--- |
| [deanattali.com](https://deanattali.com) | Dean Attali | Creator of Beautiful Jekyll |
| [ouzor.github.io](http://ouzor.github.io) | Juuso Parkkinen | Data scientist |
| [derekogle.com](http://derekogle.com/) | Derek Ogle | Professor of Mathematical Sciences and Natural Resources |
| [melyanna.github.io](http://melyanna.github.io/) | Melyanna | Shows off her nice art |
| [chauff.github.io](http://chauff.github.io/) | Claudia Hauff | Professor at Delft University of Technology |
| [kootenpv.github.io](http://kootenpv.github.io/) | Pascal van Kooten | Data analytics |
| [sjackman.ca](http://sjackman.ca) | Shaun Jackman | PhD candidate in bioinformatics |
| [anudit.in](http://www.anudit.in/) | Anudit Verma | Engineering student |
| [sharepointoscar.github.io](http://sharepointoscar.github.io) | Oscar Medina | Independent Hacker |
| [ocram85.com](https://ocram85.com) | Marco Blessing | A personal blog about PowerShell and automation |
| [khanna.cc](https://khanna.cc/) | Harry Khanna | Law and software |
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

### YAML parameter you can use to personalize each page

<<<<<<< HEAD
These are all the parameters you can place inside a page's YAML front matter that Beautiful-Jekyll supports.

Parameter   | Description
----------- | -----------
layout      | What type of page this is (default is `blog` for blog posts and `page` for other pages. You can use `minimal` if you don't want a header and footer).
title       | Page or blog post title.
subtitle    | Short description of page or blog post that goes under the title.
bigimg      | Include a large full-width image at the top of the page.  You can either give the path to a single image, or provide a list of images to cycle through (see [my personal website](http://deanattali.com/) as an example).
comments    | Only applicable if the `disqus` parameter is set in the `_config.yml` file. All blog posts automatically have comments enabled. To enable comments on a specific page, use `comments: true`; to turn comments off for a specific blog post, use `comments: false`.
social-share | If you don't want to show buttons to share a blog post on social media, use `social-share: false` (this feature is turned on by default).
share-img   | If you want to specify an image to use when sharing the page on Facebook or Twitter, then provide the image's full URL here.
image       | If you want to add a personalized image to your blog post that will show up next to the post's excerpt and on the post itself, use `image: /path/to/img.png`.
js          | List of local JavaScript files to include in the page (eg. `/js/mypage.js`)
ext-js      | List of external JavaScript files to include in the page (eg. `//cdnjs.cloudflare.com/ajax/libs/underscore.js/1.8.2/underscore-min.js`)
css         | List of local CSS files to include in the page
ex-css      | List of external CSS files to include in the page
googlefonts | List of Google fonts to include in the page (eg. `["Monoton", "Lobster"]`)

## Contributions

If you find anything wrong or would like to contribute in any way, feel free to submit a pull request/open an issue [on GitHub](https://github.com/daattali/beautiful-jekyll), or [send me a message](http://deanattali.com/contact).

Thank you to [all contributors](https://github.com/daattali/beautiful-jekyll/graphs/contributors). Special thanks to the following people with non-trivial contributions (in chronological order): [@hristoyankov](https://github.com/hristoyankov), [@jamesonzimmer](https://github.com/jamesonzimmer), [@XNerv](https://github.com/XNerv), [@epwalsh](https://github.com/epwalsh), [@rtlee9](https://github.com/rtlee9).
=======
Beautiful Jekyll is meant to be so simple to use that you can do it all within the browser. However, if you'd like to develop locally on your own machine, that's possible too if you're comfortable with command line. Follow these simple steps set that up with Docker:

1. Make sure you have [Docker](https://www.docker.com/) installed.

2. Clone your repository locally.

    ```bash
    git clone https://github.com/<your_username>/<your_username>.github.io.git
    ```

3. Run the following shell commands to build the docker image and start the container for the first time:

    ```bash
    cd <repository_folder>
    docker build -t beautiful-jekyll "$PWD"
    docker run -d -p 4000:4000 --name beautiful-jekyll -v "$PWD":/srv/jekyll beautiful-jekyll
    ```


Now that Docker is set up, you do not need to run the above steps again. You can now view your website at http://localhost:4000/. You can start the container again in the future with:

```bash
docker start beautiful-jekyll
```

And you can stop the server with:

```bash
docker stop beautiful-jekyll
```

Whenever you make any changes to `_config.yml`, you must stop and re-start the server for the new config settings to take effect.

Disclaimer: I personally am NOT using local development so I don't know much about running Jekyll locally. If you follow this route, please don't ask me questions because unfortunately I honestly won't be able to help!

## FAQ and support

If you need any help, I suggest heading over to the [Jekyll support forum](https://talk.jekyllrb.com/).

Beautiful Jekyll is actively used by thousands of people with wildly varying degrees of competency, so it's impossible to answer all the questions that may arise. Below are answers to a few very common questions. Most questions that I get asked are not directly related to this theme, and instead are more general questions about Jekyll or web development. Many such questions can be answered by reading the [Jekyll documentation](https://jekyllrb.com/) or with Google.

#### How do I change the number of posts per page OR the colour of the navigation bar OR the image in the navigation bar OR ...?

Beautiful Jekyll is built to be very customizable, and as such, many questions about "how do I change ..." can be answered by looking at the `_config.yml` file. The configuration file has many adjustable parameters to customize your site.

#### How do I add a favicon to my site?

Easy! Just place a valid `favicon.ico` (or another valid favicon image) in the root directory of your project. And then wait! It can take a while to update.

#### How do I move the blog to another page instead of having it on the home page?

The default style of Beautiful Jekyll is to feature the blog feed on the front page. But for many sites that's not the ideal structure, and you may want to have a separate dedicated page for the blog posts. To have the blog hosted on a different URL (for example at `<mysite.com>/blog`), copy the `index.html` file into a folder with the same name as the desired page (for example, to `blog/index.html`), and in the `_config.yml` file you need to add a parameter `paginate_path: "/<page name>/page:num/"` (for example `paginate_path: "/blog/page:num/"`).

#### What size do you recommend using for the `bigimg` photos?

Unfortunately, this is a no-answer! There isn't a one-size-fits-all solution to this, because every person will view your site on a different browser with different dimensions. Some browsers will have very wide aspect ratio, some will be narrower, some will be vertical (such as phones), different phones have different screens, etc. The image will always be centered, so the only tip I can give is that you should make sure the important part of the image is in the middle so that it'll always show. Other than that, every browser will show a different clipping of the image.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a

## Credits

This template was not made entirely from scratch. I would like to give special thanks to:
- [Barry Clark](https://github.com/barryclark) and his project [Jekyll Now](https://github.com/barryclark/jekyll-now), from whom I've taken several ideas and code snippets, as well as some documenation tips.
- [Iron Summit Media](https://github.com/IronSummitMedia) and their project [Bootstrap Clean Blog](https://github.com/IronSummitMedia/startbootstrap-clean-blog), from which I've used some design ideas and some of the templating code for posts and pagination.

<<<<<<< HEAD
I'd also like to thank [Dr. Jekyll's Themes](http://drjekyllthemes.github.io/), [Jekyll Themes](http://jekyllthemes.org/), and another [Jekyll Themes](http://jekyllrc.github.io/jekyllthemes/) for featuring Beautiful Jekyll in their Jekyll theme directories.
=======
I'd also like to thank [Dr. Jekyll's Themes](https://drjekyllthemes.github.io/), [Jekyll Themes](http://jekyllthemes.org/), and another [Jekyll Themes](http://jekyllrc.github.io/jekyllthemes/) for featuring Beautiful Jekyll in their Jekyll theme directories.

## Contributions

If you find anything wrong or would like to contribute in any way, feel free to create a pull request/open an issue/send me a message.  Any comments are welcome!

Thank you to [all contributors](https://github.com/daattali/beautiful-jekyll/graphs/contributors). Special thanks to  [@OCram85](https://github.com/OCram85) for contributing multiple times as well as helping with discussions.

If you do fork or clone this project to use as a template for your site, I would appreciate if you keep the link in the footer to this project.  I've noticed that several people who forked this repo removed the attribution and I would prefer to get the recognition if you do use this :)

## Known limitations

- If you have a project page and you want a custom 404 page, you must have a custom domain.  See https://help.github.com/articles/custom-404-pages/.  This means that if you have a regular User Page you can use the 404 page from this theme, but if it's a website for a specific repository, the 404 page will not be used.
>>>>>>> fdaf2eaa003374991bdea2290f2cc10ddd7c2e6a
