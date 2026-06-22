# frozen_string_literal: true

begin
  require 'voxpupuli/test/rake'
rescue LoadError
  require 'puppetlabs_spec_helper/rake_tasks'
end

begin
  require 'voxpupuli/acceptance/rake'
rescue LoadError
  # voxpupuli-acceptance not available
end

begin
  require 'puppet-strings/tasks'
rescue LoadError
  # puppet-strings not available
end
