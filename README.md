# Ruby on Rails Tutorial: sample application

This is the sample application for
the [*Ruby on Rails Tutorial*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).
###############################################
加入guard和spork支持后，运行
time bundle exec rspec spec/requests/static_pages_spec.rb --drb
报错如下：
-------------------------------------------------
Exception encountered: #<ActiveRecord::ConnectionNotEstablished: ActiveRecord::ConnectionNotEstablished>
backtrace:
/Users/yufanbai/.rvm/gems/ruby-2.0.0-p353/gems/activerecord-4.0.2/lib/active_record/connection_adapters/abstract/connection_pool.rb:546:in `retrieve_connection'
/Users/yufanbai/.rvm/gems/ruby-2.0.0-p353/gems/activerecord-4.0.2/lib/active_record/connection_handling.rb:79:in `retrieve_connection'
-------------------------------------------------

执行如下命令解决
1.gem uninstall guard-spork
2.gem uninstall spork
3.bundle install
###############################################