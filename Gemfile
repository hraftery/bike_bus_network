source "https://rubygems.org"
gem "jekyll", "~> 4.4.1"
# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
# gem "github-pages", group: :jekyll_plugins
# If you have any plugins, put them here!
group :jekyll_plugins do
end

# Note jekyll-remote-theme currently requires jekyll-sass-converter 3.0.0. You may want to
# uninstall 3.1.0 so you can run `jekyll` instead of `bundle exec jekyll`. But once this
# issue is resolved we might not need it at all: https://github.com/raviriley/agency-jekyll-theme/issues/103
#gem 'jekyll-remote-theme', '~> 0.4.3'
gem 'jekyll-agency', git: 'https://github.com/hraftery/agency-jekyll-theme.git', tag: '1.2.1'

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:windows]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]

# Prevent warning about logger not being a default gem in the future.
gem "logger", "~> 1.6.4"
