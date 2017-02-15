SpreeGeocoding
================
Forked version of https://github.com/solidusio-contrib/solidus_geocoding for Spree 
Add geocoding to `Spree::Address`.

See https://github.com/alexreisner/geocoder

Installation
------------

Add spree_geocoding to your Gemfile:

```ruby
gem 'spree_geocoding'
```

Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g spree_geocoding:install
```

Testing
-------

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs, and [Rubocop](https://github.com/bbatsov/rubocop) static code analysis. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_geocoding/factories'
```

Copyright (c) 2016 [Taylor Scott], released under the New BSD License
