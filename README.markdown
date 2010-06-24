smushit-php
=========

A PHP wrapper around Yahoo!'s [Smush.it image compression web service](http://www.smushit.com/ysmush.it/).

Given a URL to an image or a local image filename, this class will losslessly compress the image using Yahoo!'s Smush.it service and return the URL to the smushed image along with its meta information. It can optionally overwrite the local image file.

Much love to the Yahoo! [Exceptional Performance group](http://tech.groups.yahoo.com/group/exceptional-performance/) for a wonderful service :-)

EXAMPLES
--------

    $img = new SmushIt('http://some-domain.com/image.jpg');
    print_r($img); // Will output...
    // SmushIt Object
	// (
	//     [filename] => 
	//     [url] => http://some-domain.com/image.jpg
	//     [compressedUrl] => http://smushit.zenfs.com/results/dcd75d06/smush/image.jpg
	//     [size] => 42517
	//     [compressedSize] => 23063
	//     [savings] => 45.76
	//     [error] => 
	// )

UPDATES
-------

Code is hosted at GitHub: [http://github.com/tylerhall/smushit-php](http://github.com/tylerhall/smushit-php)

LICENSE
-------

The MIT License

Copyright (c) 2009 Tyler Hall <tylerhall AT gmail DOT com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.