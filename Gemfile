source "https://rubygems.org"

# Specify your gem's dependencies in rails_pulse.gemspec.
gemspec

gem "puma"

gem "sqlite3"
gem "pg"

# Load environment variables from .env file
gem "dotenv-rails", groups: [ :development, :test ]

# MySQL gem only added in CI via bundle install --with mysql
group :mysql do
  gem "mysql2"
end

# Omakase Ruby styling [https://github.com/rails/rubocop-rails-omakase/]
gem "rubocop-rails-omakase", require: false
gem "rubocop-minitest", require: false

gem "css-zero"
gem "groupdate", ">= 6.5.1"
gem "importmap-rails"
gem "rails_charts", github: "railspulse/rails_charts", branch: "chart-initialize-event"
gem "ransack"
gem "turbo-rails"
gem "pagy", "~> 43.0.0pre" 
gem "request_store"

# Testing dependencies
group :test do
  gem "appraisal"
  gem "capybara"
  gem "database_cleaner-active_record"
  gem "factory_bot_rails"
  gem "faker"
  gem "minitest-reporters"
  gem "mocha"
  gem "pry-byebug"
  gem "selenium-webdriver"
  gem "shoulda-matchers"
  gem "test-prof"
  gem "timecop"
end

group :development, :test do
  gem "debug"
end
