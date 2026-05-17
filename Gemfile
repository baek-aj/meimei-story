# Created: 2026-05-17 22:01
source "https://rubygems.org"

gem "jekyll", "~> 4.3"
gem "jekyll-theme-chirpy", "~> 7.0"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", platforms: %i[mingw x64_mingw mswin]
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
