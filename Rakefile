$LOAD_PATH.unshift File.expand_path(File.dirname(__FILE__) + '/lib')
require "mg"

MG.new("mg.gemspec")

require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/*_test.rb'
  test.verbose = false
end

task :default => :test
