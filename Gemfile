source 'https://rubygems.org'

gem 'rake'

group :docs do
    gem 'yard'
    gem 'redcarpet'
end

group :spec do
    gem 'simplecov', require: false, group: :test

    gem 'rspec', '2.99'
    gem 'faker'

    gem 'puma' if !Gem.win_platform? || RUBY_PLATFORM == 'java'

    gem 'sinatra'
    gem 'sinatra-contrib'
end

group :prof do
    gem 'stackprof'
end

if RbConfig::CONFIG['host_os'].include? 'darwin'
    gem 'arachni-rpc', path: File.dirname( __FILE__ ) + '/../arachni-rpc-v0.2'
else
    gem 'arachni-rpc', path: '/home/zapotek/workspace/arachni-rpc-v0.2'
end

gemspec

