---
layout: post
title:  "执行`rake test`没有响应"
date:   2014-12-19 17:00:00
categories: exception
tags: rake
author: "木卯溪"
---

## 执行rake test 没有响应
Since 2.0 minitest-rails does not add minitest rake tasks. The default rails test rake tasks are used. See the section on running tests in the README.

Also, if you are including the minitest-rails Railtie in your config/application.rb, then you shouldn't place the dependency in the :test group in your Gemfile.

## 相关

* [rake test](http://stackoverflow.com/questions/27559993/input-command-rake-test-but-can-not-get-a-response/27560782#27560782)
