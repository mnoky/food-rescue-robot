set :default_env, { 
  'TIME_ZONE' => 'Eastern Time (US & Canada)',
  'ASSET_HOST' => 'http://robot.friendshipdonations.org',
  'DOMAIN_NAME' => 'robot.friendshipdonations.org',
  'MAILER_ADDRESS' => 'smtp.sendgrid.com',
  'SENDGRID_USERNAME' => 'test',
  'SENDGRID_PASSWORD' => 'test',
  'FORCE_SSL' => 'false',
  'EXCEPTION_SENDER_ADDRESS' => '%{"FDN Robot" <do-not-reply@friendshipdonations.org>},',
  'EXCEPTION_EMAIL_PREFIX' => '[FDN ROBOT ERROR] ',
  'EXCEPTION_EMAIL_RECIPIENTS' => '%w{admin@friendshipdonations.org noky@noky.net}',
  'AWS_ACCESS_KEY_ID' => 'foo',
  'AWS_SECRET_ACCESS_KEY' => 'foo',
  'AWS_REGION' => 'us-east-1'
}

# Load DSL and Setup Up Stages
require 'capistrano/setup'
require 'capistrano/deploy'

require 'capistrano/rails'
require 'capistrano/bundler'
require 'capistrano/rvm'
require 'capistrano/puma'

# Loads custom tasks from `lib/capistrano/tasks' if you have any defined.
Dir.glob('lib/capistrano/tasks/*.rake').each { |r| import r }

