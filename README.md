# twitterfeeddisplayonjekyllsite
in order to host this locally, do:

bundle update
bundle exec jekyll build
bundle exec jekyll serve

this should download and install the necessary plugins and dependencies from the associated Gemfile. Gemfile can be modified to add more plugins. 
Should this not work, delete the Gemfile, create your own Gemfile. (on terminal: touch Gemfile) (or create newfile and name the file Gemfile (no extension))
and add the following into your Gemfile:

source 'https://rubygems.org'
group :jekyll_plugins do
    gem 'github-pages'
    gem 'jekyll-twitter-plugin'
end

Save the file and do:

bundle update
bundle exec jekyll build
bundle exec jekyll serve
