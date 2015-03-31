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

- Lorem ipsum
- Dolor
- Sit amet

```javascript
!(function() {
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
})();
```

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
