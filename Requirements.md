# Requirements

You'll need these installed before anything else will work.

## Node 

http://nodejs.org/

> Node.js is a platform built on Chrome's JavaScript runtime for easily building fast, scalable network applications.

We use node for all of our front-end tooling. Our entire build system is written in node. Seeing as it's just 
JavaScript and it's the build for the front-end developers, it's a perfect fit.

Node uses the CommonJS module system which is the same module system we're using for our client-side JavaScript.
This keeps things consistent and opens up the possibility of re-using code on both the front and back-end.

### Mac

```
brew install node
```

or use NVM (Node Version Manager)

```
curl https://raw.github.com/creationix/nvm/master/install.sh | sh
```

Then run to install the latest:

```
nvm install 0.10 && nvm use 0.10
```

### Windows

Get the [installer](http://nodejs.org/).

## Ruby

http://www.ruby-lang.org/en/

> A dynamic, open source programming language with a focus on simplicity and productivity.

We use Ruby primarily for building our Sass files into CSS files for the browser. Don't be afraid.

### Mac

Get rvm. It makes working with different versions of Ruby really simple. 

```
curl -L https://get.rvm.io | bash -s stable
```

Once you've got it run:

```
rvm install latest
```

### Windows

Get the [installer](http://www.ruby-lang.org/en/).

## Sass

http://sass-lang.com/

> Sass makes CSS fun again. Sass is an extension of CSS3, adding nested rules, variables, mixins, selector inheritance, and more.

We're using Sass to write most of our CSS. It allows us to write better CSS faster. Instead of writing `.css` files
you instead create `.scss` files that compile into plain old CSS. This is done for you in the build (which is explained
later on) so you shouldn't need to worry about getting your hands dirty with Ruby.

### Installation

```
gem install sass
```

## Grunt

http://gruntjs.com

Grunt is the build tool we use for all of the front-end code. It is written in node and has an extremely simple
plugin system. There are thousands of plugins available for Grunt already allowing us to leverage an amazing
eco-system.

Grunt handles everything from minification, code analysis, test running, copy files, building files and more.
If there's anything we want automated on the front-end we use Grunt. The plugins are just JavaScript and they
are extremely easy to write.

We have a [number of custom Grunt tasks available in Stash](http://ntlvmbld01:7990/projects/GT)

### Installation

```
npm install -g grunt-cli
```

## Component

http://github.com/component/component

Component is the package manager and code build tool we're using for all projects. It turns CommonJS modules into something the browser can use, turns templates into something JS can use, combines CSS and manages images and other assets.

This is run automatically in the Grunt build.

### Installation

```
npm install -g component
```

## Mocha

http://visionmedia.github.io/mocha/

Mocha is the tool we use for running JavaScript unit tests. Client-side tests are made up of a test runner HTML file
and the tests and other scripts are included like a normal, static web page.

### Installation

```
npm install -g mocha
```
