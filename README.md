Heroku Buildpack libqt4-dev Cedar 14
===========================

Use the latest version of libqt4-dev inside Heroku  _Cedar 14_.

This buildpack downloads and installs the [libqt4-dev
packages](http://packages.ubuntu.com/precise/libqt4-dev)
manually.

## Usage

This buildpack is built to be used through
[heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi),
so in your app you need to:
```
heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi
```

Then, create a `.buildpacks` file inside your app:
```
https://github.com/gnagel/heroku-buildpack-libqt4-dev-cedar-14
https://github.com/heroku/heroku-buildpack-nodejs
```

This example was based on the nodejs buildpack, but it can be used with
any other.
If it is not working with yours, please report a bug.

## Thanks

Thanks to the creator and contributors of the original
[heroku-buildpack-image-magick](https://github.com/mcollina/heroku-buildpack-libqt4-dev)
for many of the ideas used here

## Contributing to heroku-buildpack-libqt4-dev-cedar-14

* Check out the latest master to make sure the feature hasn't been
  implemented or the bug hasn't been fixed yet
* Check out the issue tracker to make sure someone already hasn't
  requested it and/or contributed it
* Fork the project
* Start a feature/bugfix branch
* Commit and push until you are happy with your contribution
* Please try not to mess with the configs.sh. If you
  want to have your own version, or is otherwise necessary, that is
  fine, but please isolate to its own commit so I can cherry-pick around
  it.

## LICENSE - "MIT License"

Copyright (c) 2015 Glenn Nagel, https://github.com/gnagel
Copyright (C) 2015 Heroku, Inc.

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.
