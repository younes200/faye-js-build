# About this repository

This repository was created in order to have an updated NPM package of the faye
Node.js module that can be defined as a dependency in `package.json`.

It can be referenced from your `package.json` file like this:

    "dependencies": {
      "faye": "git://github.com/muzzley/faye-js-build.git#master"
    }

# Faye

* Documentation: http://faye.jcoglan.com
* Mailing list: http://groups.google.com/group/faye-users
* Source code: http://github.com/faye/faye

Faye is a set of tools for simple publish-subscribe messaging between web
clients. It ships with easy-to-use message routing servers for Node.js and Rack
applications, and clients that can be used on the server and in the browser.


## Questions, issues, ideas

Please raise questions on the [mailing
list](http://groups.google.com/group/faye-users), and feel free to announce and
share ideas on Faye-related projects there too. I'd appreciate it if we only use
the GitHub issue tracker for bona fide bugs; You'll probably get better and
quicker answers to questions from the mailing list.


## Development

To hack on Faye, you'll need Node in order to build both the gem and the npm
package. There are also a few submodules we use for testing. The following
should get you up and running:

```bash
# Download the code from Git
git clone git://github.com/faye/faye.git
cd faye
git submodule update --init --recursive

# Install dependencies
bundle install
npm install

# Build Faye
npm run-script build

# Run tests
bundle exec rspec -c spec/
node spec/node.js
```


## License

(The MIT License)

Copyright (c) 2009-2013 James Coglan and contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the 'Software'), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

