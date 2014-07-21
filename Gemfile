source 'https://rubygems.org'

gemspec

require File.expand_path 'spec/support/detect_rails_version', File.dirname(__FILE__)

rails_version = detect_rails_version
gem 'rails', rails_version

gem 'arbre', github: 'gregbell/arbre' # until gregbell/arbre#16 makes it into an official release

# Optional dependencies
gem 'cancan'
gem 'devise'
gem 'draper'
gem 'pundit'
gem 'pry'

# Utility gems used in both development & test environments
gem 'rake', require: false
gem 'parallel_tests'

group :development do
  # Debugging
  gem 'pry'                # Easily debug from your console with `binding.pry`
  gem 'better_errors'      # Web UI to debug exceptions. Go to /__better_errors to access the latest one
  gem 'binding_of_caller'  # Retrieve the binding of a method's caller in MRI Ruby >= 1.9.2

  # Performance
  gem 'rack-mini-profiler' # Inline app profiler. See ?pp=help for options.
  gem 'flamegraph'         # Flamegraph visualiztion: ?pp=flamegraph

  # Documentation
  gem 'yard', github: 'lsegal/yard' # Documentation generator (until lsegal/yard#765 is in a release)
  gem 'redcarpet'          # Markdown implementation (for yard)
end

group :test do
  gem 'capybara'
  gem 'simplecov', require: false # Test coverage generator. Go to /coverage/ after running tests
  gem 'coveralls', require: false # Test coverage website. Go to https://coveralls.io
  gem 'cucumber-rails', require: false
  gem 'database_cleaner'
  gem 'guard-rspec'
  gem 'jasmine'
  gem 'jslint_on_rails'
  gem 'launchy'
  gem 'rails-i18n' # Provides default i18n for many languages
  gem 'rspec'
  gem 'rspec-rails'
  gem 'shoulda-matchers'
  gem 'sqlite3'
end
