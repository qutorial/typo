env = ENV["RAILS_ENV"] || 'development'
dbfile = File.expand_path("../config/database.yml", __FILE__)

#unless File.exists?(dbfile)
#  raise "You need to configure config/database.yml first"
#else
#  conf = YAML.load(File.read(dbfile))
#  adapter = conf[env]['adapter']
#  raise "You need define an adapter in your database.yml" if adapter == '' || adapter.nil?
#  case adapter
#  when 'sqlite3'
#    gem 'sqlite3'
#  when 'postgresql'
#    gem 'pg'
#  when 'mysql'
#    gem 'sam-mysql-ruby'
#  else
#    raise "Don't know what gem to use for adapter #{adapter}"
#  end
#end

group :production do
  gem 'pg'
end

source 'https://rubygems.org'
ruby "1.9.3"

gem 'thin', '>= 1.5.1'
gem 'rails', '~> 7.0.8', '>= 7.0.8.1'
gem 'require_relative'
gem 'htmlentities'
gem 'json'
gem 'bluecloth', '~> 2.1'
gem 'coderay', '~> 0.9'
gem 'kaminari', '>= 0.15.0'
gem 'RedCloth', '~> 4.2.8'
gem 'addressable', '~> 2.1', :require => 'addressable/uri'
gem 'mini_magick', '~> 1.3.3', :require => 'mini_magick'
gem 'uuidtools', '~> 2.1.1'
gem 'flickraw-cached'
gem 'rubypants', '~> 0.2.0'
gem 'rake', '~> 0.9.2'
gem 'acts_as_list'
gem 'acts_as_tree_rails3'
gem 'recaptcha', :require => 'recaptcha/rails', :branch => 'rails3'

group :development, :test do
  gem 'ruby-debug19'
  gem 'factory_girl', '~> 2.2'
  gem 'webrat'
  gem 'rspec-rails', '~> 2.11', '>= 2.11.4'
  gem 'simplecov', :require => false
  gem 'sqlite3'
  gem 'cucumber'
  gem 'cucumber-rails', '>= 1.3.1', :require => false
  gem 'cucumber-rails-training-wheels'
  gem 'database_cleaner'
  gem 'capybara', '>= 1.1.3'
end
