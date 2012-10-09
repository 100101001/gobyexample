## Go by Example

Source for the [Go by Example](https://gobyexample.com)
site.


### Overview

This repo contains:

* `src`: Go and Bash source code for the site
* `meta`: metadata used to generate the site
* `tool`: toolchain used to generate the site
* `style`: CSS for the site

The site is built by extracting the code & comments from
the `.go` and `.sh` source files in `src` and rendering
that data according to `meta` and `templates` via programs
in `tool`.


### Usage

To validate the source, generate the site, and open the
home page in your browser:

```console
$ tool/build
$ open site/index.html
```

To build continuously in a loop:

```console
$ tool/build-loop
```

Generation requires the [`pygmentize`](http://pygments.org/)
binary for syntax highlighting.


### License

This work is licensed under a [Creative Commons Attribution 3.0 Unported License](http://creativecommons.org/licenses/by/3.0/).
