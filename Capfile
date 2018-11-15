# Load DSL and Setup Up Stages
require 'capistrano/setup'
require 'capistrano/deploy'

require 'capistrano/rails'
require 'capistrano/bundler'
require 'capistrano/rvm'
require 'capistrano/puma'
require 'capistrano/sidekiq'

install_plugin Capistrano::Puma

Dir.glob('lib/capistrano/tasks/*.cap').each { |r| import r }

require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

