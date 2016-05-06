# Reggie CLI

## Overview

Reggie CLI is a stripped down version of the node-reggie package by github user mbrevoort. Reggie is great,
but it is no longer working on new versions of node. We have old versions of the reggie server
running on some box, but we want to upgrade node on our dev environments and not get dtrace install
errors on the reggie CLI. This package simply aims to fix that aspect by splitting out the
reggie cli part of the reggie package.

### Publishing

If installed globally, from within the root directory of an NPM module:

```bash
$ reggie-cli -u http://<host:port> publish
$ reggie-cli -u http://127.0.0.1:8080 publish
```

The Reggie client just `npm packs` your module and `PUT`s it to `http://<host:post>/package/:name/:version`.

## Read More

https://github.com/mbrevoort/node-reggie

## License

Copyright (c) 2012-2013 Mike Brevoort

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
