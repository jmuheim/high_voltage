# encoding: utf-8

require 'rubygems'
require 'bundler/setup'
require 'bundler/gem_tasks'

require 'rake'
require 'rspec/core/rake_task'
require 'appraisal'

RSpec::Core::RakeTask.new(:spec)

desc 'Default'
task :default => [:all]

desc 'Test the engine under all supported Rails versions'
task :all do |t|
  exec 'appraisal install && appraisal rake spec'
end
