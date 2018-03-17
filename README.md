# README

WIN7:

https://www.coderhold.com/install-ruby-rails-windows-7-8-10-step-step.html

Install node.js https://nodejs.org/en/

rails new techsisters_forum

add devise to Gemfile

add bootstrap to Gemfile

add jquery-rails to Gemfile

add gem 'bcrypt', git: 'https://github.com/codahale/bcrypt-ruby.git', :require => 'bcrypt'

bundle

change application css to scss and @import 'bootstrap';

//= require jquery3, popper, bootstrap to application.js

rails s

http://localhost:3000

rails generate scaffold User username:string

rails db:migrate

routes.rb -> root 'welcome#index'

rails g controller Welcome index

bundle

rails g devise:install

rails g devise:controllers users

rails g devise:views

rails g devise user

add username field to registrations/new

add login/logout links to views/layouts/application.html.erb based on user_logged_in?

rails g scaffold Post user:belongs_to title:string content:string

rails db:migrate

application.html.erb nav, container, alerts

devise views

move posts to partial, add @posts = Post.all to welcome controller. List group, 

add all posts link to to views/layouts/application.html.erb is user_logged_in?

rails g scaffold Comment post:belongs_to user:belongs_to content:string

rails db:migrate

Add new comment link to posts

move comments under posts in routes

move new comment inside post show view

...

vagrant halt