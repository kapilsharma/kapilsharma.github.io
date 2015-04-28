---
layout: post
title:  "Publish with Jekyll"
date:   2015-04-28 14:54:46
categories: jekyll update
---

I was looking to utilize github sites as blog since long. However could not finish it due to some issue or other.

# Prerequisite

We need Ruby, ruby gems and node js installed.

## Ruby

``` bash
sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
git clone git://github.com/sstephenson/rbenv.git .rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
less .bashrc
exec $SHELL
git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
git clone https://github.com/sstephenson/rbenv-gem-rehash.git ~/.rbenv/plugins/rbenv-gem-rehash
rbenv install 2.2.1
rbenv global 2.2.1
ruby -v
echo "gem: --no-ri --no-rdoc" > ~/.gemrc
gem install bundler
```

## Node JS

``` bash
sudo apt-get install nodejs
```

## info

http://24ways.org/2013/get-started-with-github-pages/

Ruby

https://gorails.com/setup/ubuntu/14.04

http://stackoverflow.com/questions/8648390/syntax-highlighting-markdown-code-blocks-in-jekyll-without-using-liquid-tags
