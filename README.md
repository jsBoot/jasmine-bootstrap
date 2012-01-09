JASMINE-BOOTSTRAP
=================

Do you like writing jasmine specs, but find the TrivialReporter underwhelming to look at? I took the standalone runner at http://github.com/fnando/jasmine-standalone and Twitter's bootstrap css at http://twitter.github.com/bootstrap to create jasmine-bootstrap. Here's what it looks like:

![BootstrapReporter](url)

Here's what the default jasmine-html.js looks like for comparison:

![TrivialReporter](url)

I kept all the TrivialReporter's css classes and most all of its html structure intact. That way jasmine-bootstrap should work with whatever ci you may have already built around the TrivialReporter.

* Does the jasmine-bootstrap reporter add any other enhancements? *
Not yet, but I'm working on a couple of other things that have always bothered me about the TrivialReporter, so we'll see.

Usage
-----

Grab everything in src/ and link to them in you html file:
``` html
<link rel="stylesheet" href="src/lib/bootstrap.css" type="text/css">
<link rel="stylesheet" href="src/jasmine-bootstrap.css" type="text/css">
<script type="text/javascript" src="src/jasmine-bootstrap.js"></script>
```
You could also grab the minified version of bootstrap.css from http://twitter.github.com/bootstrap if you want.

Starting the BootstrapReporter is just like starting the TrivialReporter:
``` html
<script type="text/javascript">
  jasmine.getEnv().addReporter(new jasmine.BootstrapReporter());
  jasmine.getEnv().execute();
</script>
```
Full example is in the test/ directory

Author
-------

**Sarah Brown**

+ http://twitter.com/esbie
+ http://github.com/esbie

License
---------------------

Copyright (c) 2011, Esbie

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.