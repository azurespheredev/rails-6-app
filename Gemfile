source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "2.7.2"

# Use Rails without ActionCable to avoid websocket-driver if not needed
gem "rails", "~> 6.1.7", require: [
                           "active_record/railtie",
                           "action_controller/railtie",
                           "action_view/railtie",
                           "active_job/railtie",
                           "sprockets/railtie",
                         ]

# Use PostgreSQL as the database
gem "pg", "~> 1.4" # use 1.4+ for better Windows support

# Use Puma as the app server
gem "puma", "~> 5.0"

# Use SCSS for stylesheets
gem "sass-rails", ">= 6"

# Webpacker for frontend assets
gem "webpacker", "~> 5.0"

# JSON APIs
gem "jbuilder", "~> 2.7"

# Compatibility patch for racc compilation issues
gem "racc", "< 1.6.0"

group :development, :test do
  gem "byebug", platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  gem "web-console", ">= 4.1.0"
  gem "rack-mini-profiler", "~> 2.0"
end

gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby]
