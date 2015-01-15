# nuklei.io

[![Build Status][build-status-image]][build-status]
[![Issue Stats][pull-requests-image]][pull-requests]
[![Issue Stats][issues-closed-image]][issues-closed]

[build-status-image]: https://travis-ci.org/nuklei-io/nuklei-io.github.io.svg?branch=develop
[build-status]: https://travis-ci.org/nuklei-io/nuklei-io.github.io
[pull-requests-image]: http://www.issuestats.com/github/nuklei-io/nuklei-io.github.io/badge/pr
[pull-requests]: http://www.issuestats.com/github/nuklei-io/nuklei-io.github.io
[issues-closed-image]: http://www.issuestats.com/github/nuklei-io/nuklei-io.github.io/badge/issue
[issues-closed]: http://www.issuestats.com/github/nuklei-io/nuklei-io.github.io

Install Jekyll
==============

```bash
$ sudo gem install bundler
... gems installed
```
Note: requires ruby 1.9.2 or higher.

```bash
$ bundle install
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
...
Your bundle is complete!
Use `bundle show [gemname]` to see where a bundled gem is installed.

$ bundle show jekyll
/Library/Ruby/Gems/2.0.0/gems/jekyll-2.4.0

$ jekyll --version
jekyll 2.4.0
```
Note: requires XCode command line tools, will fail at command line with instructions if necessary.

Note: If you get an error like the following when you run Jekyll, then run ```$ gem uninstall jekyll```, which will prompt you to choose a version to uninstall.

```bash
WARN: Unresolved specs during Gem::Specification.reset:
redcarpet (~> 3.1)
WARN: Clearing out unresolved specs.
Please report a bug if this causes problems.
/Library/Ruby/Gems/2.0.0/gems/jekyll-2.5.1/bin/jekyll:21:in `block in <top (required)>': cannot load such file -- jekyll/version (LoadError)
from /Library/Ruby/Gems/2.0.0/gems/mercenary-0.3.5/lib/mercenary.rb:18:in `program'
from /Library/Ruby/Gems/2.0.0/gems/jekyll-2.5.1/bin/jekyll:20:in `<top (required)>'
from /usr/bin/jekyll:23:in `load'
from /usr/bin/jekyll:23:in `<main>'
```

Preview Site Locally
====================

```bash
$ jekyll serve --watch
...
  Server address: http://0.0.0.0:4000/
  Server running... press ctrl-c to stop.
```
Browse to http://localhost:4000/ to preview site.

Modifications to local files cause Jekyll to automatically rebuild, so a browser refresh is sufficient to see changes.

If you have multiple Jekyll sites running at the same time, you can start one of them on a different port. This can be useful if you're comparing the master repository with your forked copy, for example:

```bash
$ jekyll serve --watch --port 4001
...
  Server address: http://0.0.0.0:4001/
  Server running... press ctrl-c to stop.
```
