FED
===

Documentation for the front-end codebase

## Requirements

* Node >=0.10.0 (http://nodejs.org/)
* Ruby >=1.9 (http://www.ruby-lang.org/en/)

You'll need these installed before anything else will work.

## Tools and Frameworks

This is a brief explanation of some of the tools and frameworks we're using. These are the higher level
tools that are unlikely to change any time soon.

### [Node](http://nodejs.org/)

> Node.js is a platform built on Chrome's JavaScript runtime for easily building fast, scalable network applications.

We use node for all of our front-end tooling. Our entire build system is written in node. Seeing as it's just 
JavaScript and it's the build for the front-end developers, it's a perfect fit.

Node uses the CommonJS module system which is the same module system we're using for our client-side JavaScript.
This keeps things consistent and opens up the possibility of re-using code on both the front and back-end.

### [Ruby](http://www.ruby-lang.org/en/)

> A dynamic, open source programming language with a focus on simplicity and productivity.

We use Ruby primarily for building our Sass files into CSS files for the browser. Don't be afraid.

### [Sass](http://sass-lang.com/)

> Sass makes CSS fun again. Sass is an extension of CSS3, adding nested rules, variables, mixins, selector inheritance, and more.

We're using Sass to write most of our CSS. It allows us to write better CSS faster. Instead of writing `.css` files
you instead create `.scss` files that compile into plain old CSS. This is done for you in the build (which is explained
later on) so you shouldn't need to worry about getting your hands dirty with Ruby.

```
$ gem install sass
```

### [Grunt](http://gruntjs.com)

Grunt is the build tool we use for all of the front-end code. It is written in node and has an extremely simple
plugin system. There are thousands of plugins available for Grunt already allowing us to leverage an amazing
eco-system.

Grunt handles everything from minification, code analysis, test running, copy files, building files and more.
If there's anything we want automated on the front-end we use Grunt. The plugins are just JavaScript and they
are extremely easy to write.

We have a [number of custom Grunt tasks available in Stash](http://ntlvmbld01:7990/projects/GT)

## Getting Started

Once you've got Node and Ruby, the first thing you'll need to do is install the global tools. First, Sass.

```
$ gem install sass
```


## Grunt Build

### Custom Grunt Tasks

## Available Components

### Styles

### Scripts
