# GDI Chicago Slides Template

These slides are built using Yeoman, with the Reveal generator. It will compile your Sass (located in `css/source`) automatically.

If you add a new Sass file that isn't a partial, you need to edit the Gruntfile. You'll see examples of where this change needs to be made.

# Getting started

Download a zip of the [tagged release](https://github.com/gdichicago/yeoman_reveal_template/releases) you want to use. I always recommend the most recent, but there may be different versions.

Unzip the file and place the contents in the Git repo of the class you're creating.

This repository includes a `.gitignore` that you should *really* keep. Its contents:

```
node_modules
*.log
.sass-cache
```

*Note*: the `bower_components` folder isn't ignored. This is commonly ignored, but this template is designed to be packaged and uploaded as-is without any special tweaks (other than creating slides).

You should have npm and Sass (Ruby gem) installed already.

```
$ npm install -g yeoman
$ npm install -g generator-reveal
$ npm install
```

And then you're ready.

# Usage

To add a new (HTML) slide:

```
$ yo reveal:slide "Slide name"
```

If you want to use Markdown:

```
$ yo reveal:slide "Slide Title" --markdown
```

To watch:

```
$ grunt server
```

To compile for distribution (`slideshow` folder):

```
$ grunt dist
```

# End result

You should have:

* a website in the `workshop` folder
* slides in the `slideshow` folder