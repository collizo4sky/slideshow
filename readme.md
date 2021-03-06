# Backbone UI: Slideshow

A simple slideshow feature using existing Backbone structures and CSS3 for lightweight rendering. 


## Install

Using bower: 
```
bower install backbone.ui.slideshow
```

## Dependencies

* [Backbone](http://backbonejs.org/)
* [Underscore](http://underscorejs.org/)
* [jQuery](http://jquery.com/) (or alternative event handler)

Note that the slideshow uses APP.View from [Backbone APP](http://github.com/makesites/backbone-app) if available, but falls back gracefully if you prefer using custom render logic. 


## Usage

In its most simple application, a model with the slides and an html fragment (either the markup or a url of the file containing it) should be enough to render the slideshow. 

```
var view = new Backbone.UI.Slideshow({
		el : "#slidehow", 
		collection : new Backbone.Collection(slides),
		url : "../html/slides.html"
});
view.render();
```
By default the html fragment will be parsed by the underscore's micro-template engine.  You are free to use any template engine by using the ```template``` option as described below. 


## Options

A more detailed list of all the available options. 

* ***collection***: the data for the slides
* ***url***: the url of an html fragment
* ***html***: the markup of the html fragment
* ***template***: A template method to parse the html fragment
* **draggable**: (Boolean) Allows the slideshow to be updated with a drag motion

## Examples 

* [Fullscreen Slideshow](http://rawgit.com/backbone-ui/slideshow/master/examples/fullscreen.html)
* [Style 01](http://rawgit.com/backbone-ui/slideshow/master/examples/style01.html)


## Credits

Created by Makis Tracend ( [@tracend](http://github.com/tracend) )

Distributed through [Makesites.org](http://makesites.org/)

Released under the [MIT license](http://makesites.org/licenses/MIT)

