---
layout: page
title: Bootstrap 4 Github Pages
---

A [Bootstrap 4](https://getbootstrap.com/) start up project for [Github Pages](https://pages.github.com/) and [Jekyll](https://jekyllrb.com/).

<div class="alert alert-primary" role="alert">
  A simple primary alert—check it out!
</div>
<div class="alert alert-secondary" role="alert">
  A simple secondary alert—check it out!
</div>
<div class="alert alert-success" role="alert">
  A simple success alert—check it out!
</div>
<div class="alert alert-danger" role="alert">
  A simple danger alert—check it out!
</div>
<div class="alert alert-warning" role="alert">
  A simple warning alert—check it out!
</div>
<div class="alert alert-info" role="alert">
  A simple info alert—check it out!
</div>


But if you don't know where to start I can recommend you to import a starting theme from [Bootswatch](https://bootswatch.com/).

* Go on [Bootswatch](https://bootswatch.com/) and choose a theme that you like.
* Using the top bar, download its `_variables.scss` and `_bootswatch.scss` files.
* Copy the content of `_variables.scss` in `_sass/_variables.scss`.
* Copy the content of `_bootswatch.scss` in `_sass/_bootstrap_customization.scss`.

That's it, you now have a totally different appearance compared to a vanilla Bootstrap 4.

### Modify the content

You probably don't want the present guide to be the front page of your website, so you should edit the `index.md` file. You probably also want to edit or delete the `CONTRIBUTING.md`, `README.md` and `LICENSE.md` files.

Aside from that you can of course create new pages and posts like with any Jekyll website by refering to the [Jekyll documentation](https://jekyllrb.com/).

### Run Jekyll on your computer to speed up testing

Editing your website's content or theme directly on Github is completely possible but, due to the time Github Pages takes to update your website, it will probably be much more effective to work using a local Jekyll installation.

To do so:

* Install the [requirements for Jekyll](https://jekyllrb.com/docs/installation/).
* Type `bundle install` at the root of your project to install the necessary Ruby dependencies.
* Type `bundle exec jekyll serve` to launch the test Jekyll web server that will re-compile your work if you edit it.
* You can then open `http://localhost:4000` in your web browser to see your work-in-progress website.

Please note that, to ensure maximum compatibility with Github Pages, the `Gemfile` of this project references the `github-pages` gem, not Jekyll directly. This implies some differences in behavior compared to the official documentation of Jekyll.

## Known issues

* Bootstrap 4 should normally be post-processed using [Autoprefixer](https://github.com/postcss/autoprefixer). Even if it is possible to use autoprefixer with Jekyll, it is not possible with a classic Github Pages installation without adding some kind of pre-processing before publication. Since this project mostly aims compatibility with Github Pages I prefer to keep it that way. The consequences of this choice is that some Bootstrap features could not work as expected on older browsers.

## Websites using Bootstrap 4 Github Pages

* [My personal blog](https://nicolas-van.github.io/)
