require "rake/testtask"
require "rake/clean"

begin
  require "jenkins/rake"
  Jenkins::Rake.install_tasks
  task :default => :package
rescue LoadError
end

begin
  require "rspec/core/rake_task"
  RSpec::Core::RakeTask.new(:spec)
rescue LoadError
end
