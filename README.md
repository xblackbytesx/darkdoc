# darkdoc

darkdoc is a small black and white theme for [Hugo](https://github.com/spf13/hugo) (a fast and modern static website engine).


### Dependencies

darkdoc needs at least version 0.14 of Hugo.


### Partials

There are a few partials that is of great interest to override


#### author

The author partial is added at the end of each single page (such as blog posts) and by default only prints the name of the author registered in the site params, e.g. in your `config.toml`

    [params]
        author = "Fabio"

In order to override and have your own markup appended to single pages, just create the file `layouts/partials/author.html` and roll your own.


### Shortcodes

darkdoc comes with these additional shortcodes:


#### gist

Include a Github gist using their JavaScript include.

    {{% gist e572b28c9a0eef0b2763 %}}

Where the first parameter is the gist id.


### Building

There is not much to build, but the theme CSS is minified using the node tool [clean-css](https://github.com/GoalSmashers/clean-css).

    cleancss -o static/css/darkdoc.min.css static/css/darkdoc.css

*Any change in styles needs to result in a minification!*


# License

darkdoc is released under the MIT license, see LICENSE for details.
