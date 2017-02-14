# awesome-rails
Becoming a Ruby and Ruby on Rails developer for people who already know some backend and/or frontend stuff

https://medium.com/ruby-on-rails/how-i-finally-learned-rails-95e9b832675b#.3cf9c5l69
http://curriculum.railsbridge.org/ruby/
http://guides.railsgirls.com/
https://www.codementor.io/learn-ruby-on-rails-online?utm_source=bestprogramminglanguagefor&utm_medium=side-projects&utm_campaign=bestprogramminglanguagefor
http://tutorials.jumpstartlab.com/
http://rubyonrailstutor.github.io/
https://code4startup.com/projects
https://thinkster.io/
http://www.opensourcerails.com/
https://hackr.io/
http://www.lugolabs.com/
http://www.tutset.com/
https://gorails.com/
http://baserails.com

https://github.com/dreikanter/ruby-bookmarks
https://github.com/hothero/awesome-rails-gem
https://github.com/sindresorhus/awesome
https://github.com/ekremkaraca/awesome-rails


## Make a Resource

This is the lightweight way to create a Resource without generating via Scaffolding, which creates a whole bunch of files and code that are not all necessary.

1. In console, `rails g model {post} title:string description:text`
2. In console, `rake db:migrate`
3. Update `config/routes.db` add the new resource `resources :posts`
4. Add a `root 'posts#index'` to the `config/routes.rb` (or whatever root path you want)
5. Go to localhost:3000 and you will get an error. You need a Controller
6. In console, `rails g controller Posts`. Make sure the resource is capitalized and pluralized
7. Refresh localhost. Missing template.
8. Go to app/view/posts and create file index.html.erb
9. Add a link to create new resource `<%= link_to "New Post", new_post_path %>`
10. Create `new.html.erb` view for resource
11. Update all the resource Controller stuff
