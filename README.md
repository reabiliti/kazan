# Kazan [![Build Status](https://travis-ci.org/khusnetdinov/kazan.svg?branch=master)](https://travis-ci.org/khusnetdinov/kazan) [![Dependency Status](https://gemnasium.com/badges/github.com/khusnetdinov/kazan.svg)](https://gemnasium.com/github.com/khusnetdinov/kazan) [![Code Climate](https://codeclimate.com/github/khusnetdinov/kazan/badges/gpa.svg)](https://codeclimate.com/github/khusnetdinov/kazan)

Kazan creates rails project and setups predefined gems and tools.

![img](http://res.cloudinary.com/dtoqqxqjv/image/upload/c_scale,w_240/v1476011701/147601141068782_rgcl3z.png)

## Installation

Install gem:

    $ gem install kazan

## Usage

By default this rails application generator uses PostgreSQL as db and RSpec as test framework. Also it installs and setups a lot usefull gems, and you don't need waste time then you stat new project.

Just run:

    $ kazan projectname

This generator maps all flags to rails native generator, for example you can create api application:

    $ kazan projectname --api

See all gems that will be installed to project in [Gemfile](https://github.com/khusnetdinov/kazan/blob/master/templates/Gemfile.erb) for web application or for api [Gemfile.api](https://github.com/khusnetdinov/kazan/blob/master/templates/Gemfile.api.erb).

## Gems

It includes applications gems:

  - [Dotenv](https://github.com/bkeepers/dotenv) Shim to load environment variables from .env into ENV in development.
  - [I18n](https://github.com/svenfuchs/rails-i18n) is central point to collect locale data for use in Ruby on Rails.
  - [PostgreSQL](https://www.postgresql.org/) database with [PG](https://rubygems.org/gems/pg/versions/0.18.4) adapter is used by defaul.
  - [Puma](http://puma.io/) is a simple, fast, threaded, and highly concurrent HTTP 1.1 server for Ruby/Rack applications.
  - [Rack Canonical Host](https://github.com/tylerhunt/rack-canonical-host) is middleware that lets you define a single host name as the canonical host for your application. Requests for other host names will then be redirected to the canonical host.
  - [Rack Timeout](https://github.com/heroku/rack-timeout) aborts requests that are taking too long; an exception is raised.
  - [Recepient Interceptor](https://github.com/croaky/recipient_interceptor) never accidentally send emails to real people from your staging environment.
  - [Rails 5.0.0](http://rubyonrails.org/)
  - [Rails Config](https://github.com/railsconfig/config) helps you easily manage environment specific settings in an easy and usable manner.
  - [Simple From](https://github.com/plataformatec/simple_form) [API EXCLUDED] aims to be as flexible as possible while helping you with powerful components to create your forms.

It includes assets gems [API EXCLUDED]:

It includes development gems:

  - [Annotate](https://github.com/ctran/annotate_models) adds a comment summarizing the current schema.
  - [Awesome Print](https://github.com/awesome-print/awesome_print) prints pretty Ruby objects in full color exposing their internal structure with proper indentation.
  - [Better Errors](https://github.com/charliesome/better_errors) [API EXCLUDED] replaces the standard Rails error page with a much better and more useful error page.
  - [ByeBug](https://github.com/deivid-rodriguez/byebug) is a simple to use, feature rich debugger for Ruby 2.
  - [Bundler Audit](https://github.com/rubysec/bundler-audit) is patch-level verification for bundler.
  - [Bullet](https://github.com/flyerhzm/bullet) is designed to help you increase your application's performance by reducing the number of queries it makes.
  - [Foreman](https://github.com/ddollar/foreman) procfile-based applications.
  - [Letter Opener](https://github.com/ryanb/letter_opener) previews email in the default browser instead of sending it.
  - [Listen](https://github.com/guard/listen) listens to file modifications and notifies you about the changes.
  - [Pry](https://github.com/rweng/pry-rails) for interactively exploring objects.
  - [Rack Mini Profiler](https://github.com/MiniProfiler/rack-mini-profiler) [API EXCLUDED] displays speed badge for every html page.
  - [Spring](https://github.com/rails/spring) speeds up development by keeping your application running in the background.
  - [Web Console](https://github.com/rails/web-console) [API EXCLUDED] is a debugging tool for your Ruby on Rails applications.

It includes tests gems:
 - [Capybara](https://github.com/jnicklas/capybara) [API EXCLUDED] helps you test web applications by simulating how a real user would interact with your app.
 - [Database Cleaner](https://github.com/DatabaseCleaner/database_cleaner) is a set of strategies for cleaning your database in Ruby.
 - [Factory Girl](https://github.com/thoughtbot/factory_girl) is a fixtures replacement with a straightforward definition syntax.
 - [Faker](https://github.com/stympy/faker) a port of Perl's Data::Faker library that generates fake data.
 - [Formulaic](https://github.com/thoughtbot/formulaic) [API EXCLUDED] the tedium of formulaic form filling with Capybara.
 - [Launchy](https://github.com/copiousfreetime/launchy) [API EXCLUDED] helper class for launching cross-platform applications in a fire and forget manner.
 - [Rspec](https://github.com/rspec/rspec-rails) is a testing framework for Rails.
 - [Simplecov](https://github.com/colszowka/simplecov) is a code coverage analysis tool for Ruby.
 - [Shoulda Matchers](https://github.com/thoughtbot/shoulda-matchers) provides RSpec- and Minitest-compatible one-liners that test common Rails functionality.
 - [Timecop](https://github.com/travisjeffery/timecop) providing "time travel" and "time freezing" capabilities, making it dead simple to test time-dependent code.
 - [Web Mock](https://github.com/bblimke/webmock) for stubbing and setting expectations on HTTP requests in Ruby.

## Bonuses

  - TODO: The ./bin/setup convention for new developer setup
  - TODO: A few nice time formats set up for localization
  - t() and l() in specs without prefixing with I18n
  - TODO: Rack::Deflater to compress responses with Gzip
  - TODO: A low database connection pool limit
  - [Safe binstubs] (https://github.com/thoughtbot/suspenders/pull/282)

## Optional associate services

- TODO: Gitlab CI
- TODO: Gitlab Docker Registry

## Other

  TODO

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
