<h1>
  <img src="images/ruby-banner.png">
</h1>

<br>
<br>

<p align="center">
	<b>✨ Becoming a Ruby and Ruby on Rails developer for people who already know some developery things. A loving guide continually a work-in-progress ✨</b>
</p>

<br>

<hr>

### The Best Way to Learn Rails

The best way to learn Ruby on Rails if you have some experience in web development, but not necessarily programming or computer science, is through *project based learning*. Building practical app examples will help you understand how things work and what you can do with the knowledge you obtain. Yes, learning the fundamentals of a programming language, like variables, loops, conditionals, and all that other stuff, *is* good, but there is still a disconnect between the fundamentals and practical implementation. Plus, you will start learning the fundamentals as you build real world apps.

1. **Project based learning.** Choose classes and courses that focus on building practical apps.
2. **Repetition.** Build a whole bunch of things! Starting off, opt for project based courses that build small apps and build a bunch. Doing so may seem repetitive (because it is) but will teach you the fundamentals of how any Ruby on Rails app is built from the ground up.
    * Tip: our suggestion is not to take some of the courses provided by the big name code schools. Not because they are not any good, but because the projects are HUGE and really extensive and overwhelming for a beginner. An example would be don't take a class that clones a big app like Facebook.
    * Also, as a beginner Ruby on Rails developer, you are going to mess up *a lot*. And Rails errors can be really cryptic and frustrating for beginners. That's why you **must** build small apps, because at some point you will hit a roadblock and you don't know how to continue. Would you prefer that to be on a course that takes 2 hours to complete? Or a course that clones Facebook and takes 12 hours? (speaking from experience over here!)
3. **Stick to the tutorial.** Yeah, yeah, we know you are excited building a project based app following along with a tutorial, and you have some great ideas of how you can deviate from the tutorial and build something else, or modify this, or modify that, but... for the time being, don't. Stick to the tutorial verbatim. At least for the first go round.
    * Dream: dreaming is great, and you really should dream big! Then go build a Rails Idea Logger app and keep track of all your ideas :)
    * Stick in the mud: stick to the tutorials verbatim in the beginning. Why? Because learning this stuff is hard! And you *will mess stuff up* and if you deviate from tutorial you won't know how to get back on track. So, at least for the first few project based apps you build, follow it to a T.

### If you know nothing about web development this is not for you (no offense)

This guide is for people who know some things already. If you're brand new to web development, check out [Interneting Is Hard](https://internetingishard.com/) and then check out [Codecademy's beginner classes](https://www.codecademy.com/) before diving into Ruby on Rails.

## Getting Started with Rails

1. Setup your Ruby on Rails environment
    * [Rails Girls Environment Setup](http://guides.railsgirls.com/install)
    * [Jumpstart's Environment Setup Guide](http://tutorials.jumpstartlab.com/topics/environment/environment.html)
1. Start with the official [Ruby on Rails Guide Tutorial](http://guides.rubyonrails.org/getting_started.html)
1. [Create a simple app with Leo Trieu](https://code4startup.com/projects/hero-learn-ruby-on-rails-and-wistia-apis-by-cloning-code4startup-version-newbies)
1. Build a few [Rails apps with Mackenzie Child](https://medium.com/ruby-on-rails/how-i-finally-learned-rails-95e9b832675b#.xkwboov9j)

## Tutorials

- https://medium.com/ruby-on-rails/how-i-finally-learned-rails-95e9b832675b#.3cf9c5l69
- http://curriculum.railsbridge.org/ruby/
- http://guides.railsgirls.com/
- https://www.codementor.io/learn-ruby-on-rails-online?utm_source=bestprogramminglanguagefor&utm_medium=side-projects&utm_campaign=bestprogramminglanguagefor
- http://tutorials.jumpstartlab.com/
- http://rubyonrailstutor.github.io/
- https://code4startup.com/projects
- https://thinkster.io/
- http://www.opensourcerails.com/
- https://hackr.io/
- http://www.lugolabs.com/
- http://www.tutset.com/
- https://gorails.com/
- http://baserails.com
- http://www.schneems.com/ut-rails/
- [Reddit on Rails](https://github.com/schneems/reddit_on_rails)

## Just Ruby

- [Why's (Poignant) Guide to Ruby](http://poignant.guide/book/)
- [Learn Ruby the Hard Way](https://learnrubythehardway.org/book/)
- [RubyMonk](https://rubymonk.com/)

## Rails Tasks & Features

- [Creating Static Pages](http://blog.teamtreehouse.com/static-pages-ruby-rails)

## Lists of Rails Things
- https://github.com/dreikanter/ruby-bookmarks
- https://github.com/hothero/awesome-rails-gem
- https://github.com/sindresorhus/awesome
- [Real World Rails](https://github.com/eliotsykes/real-world-rails)
- [RubyTapas](https://www.rubytapas.com/)

## Examples of Open Source Apps Built with Rails
- https://github.com/ekremkaraca/awesome-rails

## Podcasts
- [Rails5 Podcast](https://ruby5.codeschool.com/)

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

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Spacetime](http://heyspacetime.com) has waived all copyright and related or neighboring rights to this work.
