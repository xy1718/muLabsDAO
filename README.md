---
---
# muLabsDAO DNA - tech setup for the site

muLabsDAO DNA is a web site that describes how muLasbDAO works and why. The source lives on github.

Below are instructions for how to set up a local development environment. Useful for when you want to make many changes and test locally before pushing to github.

## 1. Install GIT

Here's [how to install GIT](http://git-scm.com/book/en/v2/Getting-Started-Installing-Git). 

## 2. Clone the repo

Tell git to download the muLabs dna source:

    git clone https://github.com/xy1718/muLabsDAO.git
	cd muLabsDAO

You should now have the whole thing, including the README.md file that you are reading right now!

The web site source files are under `_docs`, have a look! They are written using [markdown](https://guides.github.com/features/mastering-markdown/) (a simpler format than html). When you push to github, it will automatically convert the pages to static html and build the site. 

## 3. Install Jekyll and related tools

To test the site locally, you need to install jekyll (the tool that github uses to generate sites), which in turn relies on some Ruby stuff. But you can do all easily via Ruby bundler, like this:

First install Ruby if you don't already have it, for example via [homebrew](http://brew.sh).

    brew install ruby

Then install the Ruby Bundler gem, if you don't already have it.

    gem install bundler

Next, tell the bundler to install all the gems needed (jekyll, github-pages, etc). They are listed in Gemfile in case you are curious.

	bundle install	

If you are getting error messages, you may have old versions of some Gems installed. Try updating to the latest using:

	bundle update	

Congrats! You got the stuff you need. You should now be ready to....

## 4. Run the site locally!

Tell Jekyll to generate the site and serve it up:

    bundle exec jekyll serve

Or if you are lazy you can use the run script (which just does jekyll serve)

That's it, your local copy of the muLasbDAO DNA site should be up and running on
[http://localhost:4000](http://localhost:4000)

Every time you edit a source doc (under _docs) it will update the site automatically.


