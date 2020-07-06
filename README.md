# Notice

All changes are directly pushed to the [Wintermute website](https://www.projekt-wintermute.de/)

# Editing

The folowing guidelines should be sufficient to edit the content of the page. The content can be written in mark down [Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) or plain html.

## Pages

All pages are located in the root directory as `<title>.md`. New pages can be added by copy/paste from an existing page. Please note that the permalink front matter has to be unique.

## Partners and Publications

All partners and publications are managed via data files, which are located in the *_data/* folder. To edit or to create a new entry simply extend the respective YAML file.

## Images

Images should be uploaded to */assets/img/*

# Setup for local testing

The following is only required if one wants to parse the site locally (the following is for Ubuntu). 

Install ruby:

    sudo apt-get install ruby-full build-essential zlib1g-dev

Set path:

    echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
    echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
    echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
    source ~/.bashrc

Install Jekyll:

    # Note: does not work for me, despite GEM_HOME it still tries to install in
    # /var/lib/gems/ on Ubuntu 18.04 and thus complains with permissions denied
    gem install jekyll bundler

Parse the site and create a local server:

    jekyll serve


Install and Serve - on Mint 19.3/bionic
    
    bundle install
    bundle exec jekyll serve

View the site:

http://127.0.0.1:4000/






