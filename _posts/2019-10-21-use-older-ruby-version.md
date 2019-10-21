---
layout: post
title: Use older Ruby version
tags: [linux,ruby]
comments: true
---
While playing around with Jekyll, sometimes I was facing issues, which could be related to the Ruby version. [Here](https://linuxize.com/post/how-to-install-ruby-on-ubuntu-18-04/) is a good guide how to install Ruby.

This is how you switch between versions:
~~~
source ~/.rvm/scripts/rvm
rvm use 2.3 --default
ruby -v
~~~

