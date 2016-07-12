# Extras: Sinatra Front-End Assets

## Why do we need to learn this?

Sinatra does a lot of abstracting for us. We don't see the code in our file system that is executed by many gems. In this case, there's a `:public_folder` declared for '/static' resources by default.

## What's the trick?

It's pretty simple, actually. Just create a `/public` folder in the root directory of your project and place all your assets there. You must name this folder 'public' with a lower-case 'p'. If you create separate directories for stylesheets and javascripts, which is recommended, then the path from your `layout.erb` might look like this (but feel free to change the names of the folders and files):

```html
<link rel="stylesheet" type="text/css" href="/css/reset.css">
<link rel="stylesheet" type="text/css" href="/css/style.css">

<script type="text/javascipt" src="/js/scripts.js"></script>

```

You can see a sample of this [here](https://github.com/sf-wdi-29/sinatra-relationships-lab/blob/master/solution-code/songs-app/views/layout.erb#l5-9).


## I hate the word 'public'. Why can't I rename it???

[You can!](http://www.sinatrarb.com/intro#Static%20Files)


## "But Doctor, what about SASS?"

* Option 1:  Just run SASS from the command line and link your CSS file the old-fashioned way.
* Option 2:  Try [Compass](http://thesassway.com/beginner/getting-started-with-sass-and-compass), which does the same thing as Option 1, a little cleaner.
* Option 3:  Find a gem that does things the Rails way, such as the [Sinatra Asset Pipeline](https://github.com/kalasjocke/sinatra-asset-pipeline)


## Licensing
All content is licensed under a CC­BY­NC­SA 4.0 license.
All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.