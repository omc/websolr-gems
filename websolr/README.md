# Websolr

[Websolr](https://www.websolr.com/) is a hosted [Solr](https://lucene.apache.org/solr/) platform offering Search as a Service. Websolr provides a number of features and additional architecture around Solr (TLS/SSL, authentication, redundancy, queuing, and more). Websolr is agnostic about clients, and supports a wide array of languages and frameworks.

The standard Ruby gem for communicating with a Solr instance is the fantastic [RSolr gem](https://github.com/rsolr/rsolr). Many other gems are built on top of RSolr, including the extremely popular [Sunspot gem](https://github.com/sunspot/sunspot).

Making the best use of Websolr's advanced features requires overriding some of the default behaviors of these libraries. This can be a complicated and time-consuming process for developers who just want to get up and running fast, with minimal configuration.

This gem automates those changes, so that all a developer needs to do is install the gem itself, and everything else will be taken care of automatically. Behaviors can be modified through environment variables and YAML configuration files.

## Installation

To use these gems, simply add the following to your project's Gemfile:

```ruby
gem 'websolr'
gem 'websolr-sunspot' # Only if you're using Sunspot
```

Then run `bundle install` to install the gem(s).

That's it!
