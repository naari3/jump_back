source "https://rubygems.org"

# Declare your gem's dependencies in jump_back.gemspec.
# Bundler will treat runtime dependencies like base dependencies, and
# development dependencies will be added by default to the :development group.
gemspec

rails_version = ENV["RAILS_VERSION"] || "default"

rails = case rails_version
when "master"
  {github: "rails/rails"}
when "default"
  ">= 4.0.0"
else
  "~> #{rails_version}"
end

gem "rails", rails