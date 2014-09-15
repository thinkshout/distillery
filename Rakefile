require 'rubygems'
require 'rake'
require 'rdoc'
require 'date'
require 'yaml'
require 'tmpdir'
require 'jekyll'

task :default => :server

desc 'Build site with Jekyll'
task :build do
  jekyll 'build'
end

desc 'Build and start local server'
task :serve do
  jekyll 'serve -w --baseurl=""'
end

def jekyll(opts = '')
  system 'rm -rf _site'
  system 'bundle exec jekyll ' + opts
end
