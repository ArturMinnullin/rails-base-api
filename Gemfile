source 'https://rubygems.org'

ruby '2.1.1'

gem 'rails', '4.1.4'

# https://github.com/rails-api/rails-api/issues/135
gem 'rails-api', git: 'https://github.com/fs/rails-api.git'

gem 'pg'
gem 'thin'
gem 'decent_exposure'
gem 'active_model_serializers'
gem 'interactor-rails'
gem 'seedbank'
gem 'dotenv-rails'
gem 'devise'

group :development do
  gem 'letter_opener'
  gem 'foreman'
  gem 'bullet'

  gem 'guard-rspec'
  gem 'rb-fsevent', require: false
  gem 'zeus'
end

group :development, :test do
  # FIXME: Required for fixing warning
  # https://github.com/rspec/rspec-rails/pull/772
  # Going to be fixed in rspec > 2.99
  #
  gem 'minitest'
  gem 'byebug'
  gem 'rspec-rails'
  gem 'mail_safe'

  gem 'rails_best_practices'
  gem 'brakeman'
  gem 'rubocop'
  gem 'bundler-audit'
end

group :test do
  gem 'simplecov', require: false
  gem 'webmock', require: false

  gem 'database_cleaner'
  gem 'email_spec'
  gem 'shoulda-matchers'
  gem 'json_spec'
end

group :development, :test, :staging do
  gem 'faker'
  gem 'factory_girl_rails'
  gem 'rspec_api_documentation'
  gem 'apitome'
end

group :staging, :production do
  gem 'rollbar'
  gem 'rails_12factor'
end
