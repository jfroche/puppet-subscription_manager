source "https://rubygems.org"

group :test do
gem "rake"
gem "listen","2.1.0"
gem "puppet", ENV['PUPPET_VERSION'] || '~> 4.5.0'
gem "rspec-puppet", :git => 'https://github.com/rodjek/rspec-puppet.git'
gem "puppetlabs_spec_helper"
gem 'rspec-puppet-utils', :git => 'https://github.com/Accuity/rspec-puppet-utils.git'
gem 'hiera-puppet-helper', :git => 'https://github.com/bobtfish/hiera-puppet-helper.git'
# there seems to be a bug with puppet-blacksmith and metadata-json-lint
# removing metadata for now
gem "metadata-json-lint"
gem 'puppet-syntax'
gem 'puppet-lint'
gem 'codeclimate-test-reporter', :require => false
gem 'serverspec',                    :require => false
gem 'beaker-puppet_install_helper',  :require => false
gem 'master_manipulator',            :require => false
gem 'beaker-hostgenerator'

if RUBY_VERSION < '2.2.5'
# lock beaker version
gem 'beaker', '~> 2.0'
gem 'beaker-rspec', '~> 5.6'
# lock nokogirii
gem 'nokogiri', '1.6.8'
else
gem 'beaker-rspec'
gem 'nokogiri'
end

end

group :development do
gem "travis"
gem "travis-lint"
gem "puppet-blacksmith"
gem "guard-rake"
end
