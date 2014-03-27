# BlogJS


## Description

BlogJS is a simple blog application built with AngularJS, Node.js and MongoDB. Creates your article and shares them in a beautiful minimalistic template.

## Features

- [x] Create Article
- [x] Edit Article
- [x] Delete Article
- [x] Add tags to Article
- [x] Add Authentication to the administration
- [ ] Add snapshot for Google Crawling bot

## Installation

Get the sources with `git clone https://github.com/kdelemme/blogjs.git`

## Run

### Build

The build result is already available, but if you want to build it yourself, install bulp: 

Under blogjs/ directory:

Install gulp globally: `npm install gulp gulp-concat`

Make sure you have a package.json and install gulp in your project dependencies: `npm install --save-dev gulp`

Run gulp: `gulp`

### Back-end

Go to the api folder and install the dependencies: `npm install bcrypt express mongoose express-jwt jsonwebtoken`

Edit api/blog.js and replace the value of Access-Control-Allow-Origin to match your server configuration.

Edit api/route/users.js and replace `user.username = "YOUR_USERNAME";` and `user.password = "YOUR_PASSWORD";` with your username and password. After the first launch, delete those lines and restart the nodejs application.

Run the application: `node blog.js`

### Front-end

Edit app/js/app.js and replace the value of `options.api.base_url` to match your server configuration.

You can now open your browser: `http://localhost/blogjs/app`

To access the Administration, go to `http://localhost/blogjs/app/#/admin/login`

## Stack

* AngularJS
* Bootstrap
* MongoDB
* Node.js

## Licence
The MIT License (MIT)

Copyright (c) 2014 Kevin Delemme (kdelemme@gmail.com)

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


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/kdelemme/blogjs/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

