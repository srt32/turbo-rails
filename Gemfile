source 'https://rubygems.org'

gemspec

rails_version = ENV.fetch("RAILS_VERSION", "7.0")

if rails_version == "main"
  rails_constraint = { github: "rails/rails" }
  gem "sprockets-rails"
else
  rails_constraint = "7.0.0.alpha2"
end

gem "rails", rails_constraint

gem 'rake'
gem 'byebug'
gem 'puma'

group :development, :test do
  gem 'importmap-rails'
end

group :test do
  gem 'capybara'
  gem 'rexml'
  gem 'selenium-webdriver'
  gem 'webdrivers'
  gem 'sqlite3'
end
