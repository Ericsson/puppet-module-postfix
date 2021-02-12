source ENV['GEM_SOURCE'] || 'https://rubygems.org'

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end

gem 'facter', '~> 1.0'   if ENV['PUPPET_GEM_VERSION'] < '~> 3.5.0'
gem 'facter', '>= 2.2.0' if ENV['PUPPET_GEM_VERSION'] >= '~> 3.5.0'

gem 'puppet-lint', '~> 2.0'
gem 'puppet-lint-absolute_classname-check'
gem 'puppet-lint-alias-check'
gem 'puppet-lint-empty_string-check'
gem 'puppet-lint-file_ensure-check'
gem 'puppet-lint-file_source_rights-check'
gem 'puppet-lint-leading_zero-check'
gem 'puppet-lint-spaceship_operator_without_tag-check'
gem 'puppet-lint-trailing_comma-check'
gem 'puppet-lint-undef_in_function-check'
gem 'puppet-lint-unquoted_string-check'
gem 'puppet-lint-variable_contains_upcase'

gem 'rspec-puppet',       '~> 2.7.0' if RUBY_VERSION < '2.0.0'
gem 'json',               '<= 1.8'   if RUBY_VERSION < '2.0.0'
gem 'json_pure',          '<= 2.0.1' if RUBY_VERSION < '2.0.0'
gem 'metadata-json-lint', '0.0.11'   if RUBY_VERSION <= '1.9.3'
gem 'metadata-json-lint'             if RUBY_VERSION > '1.9.3'
gem 'public_suffix',      '~> 1.1.0' if RUBY_VERSION < '2.1.1' && RUBY_VERSION >= '1.9'
gem 'public_suffix',      '1.3.0'    if RUBY_VERSION < '1.9'

gem 'puppetlabs_spec_helper', '~> 2.7',   :require => false if RUBY_VERSION >= '1.9'
gem 'parallel_tests',         '<= 2.9.0', :require => false if RUBY_VERSION < '2.0.0' && RUBY_VERSION >= '1.9'
gem 'parallel_tests',         '1.0.9',    :require => false if RUBY_VERSION < '1.9'
gem 'parallel',               '1.3.3.1',  :require => false if RUBY_VERSION < '1.9'

if puppetversion && puppetversion < '5.0' && RUBY_VERSION >= '2.1.9'
  gem 'semantic_puppet', :require => false
end
