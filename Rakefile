require 'bundler/gem_tasks'
require 'rspec/core/rake_task'
require 'rubocop/rake_task'

RSpec::Core::RakeTask.new
RuboCop::RakeTask.new(:rubocop)

desc 'Run Fasterer'
task :fasterer do
  sh('bundle exec fasterer')
end

task(default: [:spec, :rubocop, :fasterer])
