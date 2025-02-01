source "https://rubygems.org"

# Use Jekyll with GitHub Pages constraints
gem "jekyll", "~> 3.9"

# Minimal Mistakes theme (Gem-based method)
gem "minimal-mistakes-jekyll"

# GitHub Pages (Locks dependencies for compatibility)
gem "github-pages", group: :jekyll_plugins

# Required Plugins
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-include-cache" # Enables caching to optimize performance
  gem "jekyll-remote-theme" # Allows using remote themes like Minimal Mistakes
end

# Performance booster for Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

gem "faraday-retry", "~> 2.2"
