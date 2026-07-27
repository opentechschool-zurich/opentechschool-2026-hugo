# A Hugo Static Website for the OpenTechSchool Zurich

## Setup

- Add the Congo theme to the `theme/` folder.

### The template

We are using the "Congo" template.

- https://jpanther.github.io/congo/docs/configuration/

## Specific features


### Listing all recent articles

We have a custom _partial_ for the _recent articles_ that shows all recent articles, regardless of their language.

## Map

I've created a shortcode for embedding a map from OpenStreetMap:

- The shortcode inspired by https://raw.githubusercontent.com/hanzei/hugo-component-osm/

Usage:

- In <https://openstreetmap.org> look for the coordinates of place you to have at the center of the map
 - If you have a location in the search result, it's location (`latitude, longitute`)
 - Otherwise, right click on the point you want at the center of the map, pick "Center map here" and copy the values at the end of the url (`latitude/longitute`)

Possible improvements:

- Add a paremeter for moving the marker off the center
- Add some Javascript to support relative (100% ...) widths or heights

## Learning Hugo

## The first steps

- For the first steps, it's worth just using an existing templates with a good support for the latest Hugo version.

## Customizing the template

- Override parts of the templates, buy creating overrides.

## Learning the template language

- https://gohugo.io/templates/introduction/
- It (mostly) uses a ["prefix" notation](https://en.wikipedia.org/wiki/Polish_notation).
- The documentation sections: https://gohugo.io/documentation/
- Casting from strings: https://gohugo.io/functions/cast/
- Doing math: https://gohugo.io/functions/math/


## Creating custom shortcodes

Shortcodes can be used to add _custom_ items in the markdown pages.

- https://gohugo.io/templates/shortcode/

## TODO

- [x] Show the list of all posts in the german posts page
- [ ] Fill the content
