# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies
         sudo emacs /var/lib/gems/2.5.0/gems/activerecord-5.2.2.1/lib/active_record/connection_adapters/sqlite3_adapter.rb
  12 -	 #gem "sqlite3", "~> 1.3.6"
  13 +     gem "sqlite3", ">= 1.3.6"
  ##
  #
  /var/lib/gems/2.5.0/gems/bundler-2.0.1/lib/bundler/rubygems_integration.rb:408:in `block (2 levels) in replace_gem': Error loading the 'sqlite3' Active Record adapter. Missing a gem it depends on? can't activate sqlite3 (~> 1.3.6), already activated sqlite3-1.4.0. Make sure all dependencies are added to Gemfile. (LoadError)
	from /var/lib/gems/2.5.0/gems/activerecord-5.2.2.1/lib/active_record/connection_adapters/sqlite3_adapter.rb:12:in `<main>'
  ######
  #   sqlite3 1.4.0  2018/02
  #  sqlite3自体の最新versionは1.4.x代
  #  上記の後方互換性の指定'~> 1.3.6'は1.4.0未満を指定しているので、
  #  Railsがサポートしているsqlite3versionの範囲で後方互換性を留められる。
  ###

[sudo] condorsan のパスワード: 

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
