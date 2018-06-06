# Pristine

A clean and elegant theme for [Hugo](https://gohugo.io/)

### Things you need to put on your config.toml

```
baseURL = "http://yourwebsite.com/"
languageCode = "en-us"
title = "My Awesome Site"
canonifyURLs = true
enableEmoji = true
googleAnalytics = "UA-XXXXXX-1"
```

Replace that `googleAnalytics` variable with one of your own.

Then clone the this repo in your themes directory:

```
cd themes
git clone https://github.com/sakibccr/pristine.git
```

Then set the `theme` variable in your config file:

```
theme = "pristine"
```

You must put an image in a directory called `img` inside your static directory. Then you must put the path of that image in the `portrait` variable like so:

```
[params]
    portrait = "img/portrait.jpg"
```

You can set up your main menu. You must create a `_index.md` file in your `content` directory. Then you can make other directories inside the `content` directory and set your menu url accordingly.

Example:

```
[[menu.main]]
  name = "Home"
  url = "/"
  weight = 1

[[menu.main]]
  name = "All Articles"
  url = "/all/"
  weight = 2
```

In the above case, you must create a directory called `all` inside `content` and create a `_index.md` there. That will then show all of your posts in one page.

Then there is a menu called *Projects*. You can create it like bellow:

```
[[menu.projects]]
  name = "My awesome project"
  url = "https://myawesomeproject.com"
  weight = 1
```

Another last thing is you can set your social profiles links in the config and they will show up in your site. You can do that like this:

```
[[params.social]]
    title = "Email"
    url = "mailto:john@doe.com"
[[params.social]]
    title = "Follow @johndoe"
    url = "https://twitter.com/johndoe"
[[params.social]]
    title = "Github"
    url = "https://github.com/johndoe"
[[params.social]]
    title = "Facebook"
    url = "https://facebook.com/johndoe"
```

*PRs and issues are welcome* :thumbsup: :pizza:
