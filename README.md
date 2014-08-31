The Goldilocks Approach in Sass
===============================

I really like [The Goldilocks Approach](http://goldilocksapproach.com/) for making responsive designs in CSS. I also really like [SASS](http://sass-lang.com/). As such, this project is a straight port from CSS to both SASS and SCSS. I've packaged the whole thing as a basic [Compass](http://compass-style.org/) project.

Installation
------------

I'm assuming if you're using this, you have SASS and Compass and all that installed on your computer. If so, you can just clone the repo and get started.

Usage
-----

The Goldilocks approach makes use of a couple of things available in [Bourbon Sass](http://bourbon.io) but not in the base SASS mix.

In the file `_bear_defaults.scss`, I've included some commented lines that can replace the longer contexts. With Bourbon installed, the file looks like:

```
$baby_bear_max_width: 30em;
$mummy_bear_max_width: 30em;
$daddy_bear_max_width: 60em;

$leading: golden-ratio(1em, 1);
$body_font_family: $georgia;

@mixin cf {
	@include clearfix;
}
```

But, obviously only use that if you've already installed Bourbon.