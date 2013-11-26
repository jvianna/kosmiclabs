require 'rubygems'
require 'rake'
require 'rdoc'
require 'date'
require 'yaml'
require 'tmpdir'
require 'jekyll'

desc "Generate files"
task :generate do
    Jekyll::Site.new(Jekyll.configuration({
        "source"        => ".",
        "destination"   => "_site",
        "config"        => "_config-prod.yml"
    })).process
end

task :default => :generate