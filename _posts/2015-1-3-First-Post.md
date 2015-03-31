---
layout: post
title: My first blog post
permalink: my-first-blog-post
category: Software development
tags: Ruby on Rails, AngularJS, GULP, Webpack
---

Just starting **new blog** powered by *[Jekyll](http://www.jekyllrb.com)* and so
far it seems awesome! I especially like the fact that I can write everything in
*Markdown*.

I want to try out some styles so I'll go ahead and add some elements to this
page.

## What will be the blog about?

Software development! Web development to be more concrete. I enjoy working on
both: client side as well as server side of the applications. I will cover topics
mainly about:
	- Ruby and Ruby on Rails
	- Javascript
	- Various JS frameworks
	..- AngularJS
	..- React
	..- Backbone
	- My favorite JS tools
	.. - GULP
	.. - Webpack

## How does the code looks like here?

Let's try some Ruby:
```ruby
class User
	attr_accessor :username, :email, zipcode
	attr_writer :password_confirmation

	def address
		{ city: City.find_by_zipcode(zipcode) }
	end

	# TODO: Create actual method to get user's phone number
	def phone_number
		'0987 123 432 943'
	end
end
```

And now some Javascript goodnes:
```javascript
!(function) {
	module.exports = function(ngModule) {
		ngModule.controller('UsersListCtrl', UsersListCtrl);

		function UsersListCtrl(UsersModel) {
			var vm = this;

			UsersModel.getUsers()
				.then(function(result) {
					vm.users = result;
				});
		};
	};
}();
```

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
