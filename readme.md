# cmx.js - a library for authoring [xkcd-style](http://xkcd.com) comixes

### Please visit [cmx.io](http://cmx.io) for a live example.

<a href="http://cmx.io"><img src="http://cmx.io/img/cmx-preview.png" width="800px"/></a>

Note: Source for this comix strip is in [app/sample.html](app/sample.html).

### Read more about the markup [on the wiki](https://github.com/darwin/cmx.js/wiki)

## Development

Most of the files were generated by Yeoman. Actual cmx.js sources are located in [app/lib](app/lib).

#### Dependencies

* [yeoman](http://yeoman.io)

#### Initial setup

    git clone git://github.com/darwin/cmx.js.git
    cd cmx.js

#### Hacking

    cd cmx.js
    yeoman server
    => yeoman will open browser with editor and sample.html (http://localhost:3501)

#### Deploy

* ruby+rake must be available
* npm install exec-sync
* cmx.io repository checkout is expected at same directory level as cmx.js
* ask for push rights to [darwin/cmx.io](https://github.com/darwin/cmx.io) or just keep forked version and let me pull your changes

Initial setup:

    git clone git://github.com/darwin/cmx.io.git
    cd cmx.io
    git checkout gh-pages
    cd ..

My workflow:

    cd cmx.js
    rake build
    cd ../cmx.io
    git commit -m "published a new version!"
    git push -u origin gh-pages

    => http://cmx.io should reflect the changes in a few minutes

## Acknowledgements

* [Randall Munroe](http://xkcd.com) - [xkcd.com](http://xkcd.com)
* [Dan Foreman-Mackey](http://dan.iel.fm) - [xkcd plot drawing](http://dan.iel.fm/xkcd)
* [Jeremy Ashkenas](http://ashkenas.com) - [coffescript](http://coffeescript.org), [underscore.js](http://underscorejs.org)
* [Mike Bostock](http://bost.ocks.org) - [d3.js](http://d3js.org)
* [Michael Ciuffo](http://ch00ftech.com) - [humor-sans.ttf font](http://xkcdsucks.blogspot.cz/2009/03/xkcdsucks-is-proud-to-present-humor.html)
* [Cloud9 guys](http://c9.io) - [Ace Editor](http://ace.ajax.org)
* and many others making the web awesome

## License: [MIT](license.txt)
