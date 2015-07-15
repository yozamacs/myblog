layout: hosting
title: "Hosting an angular seed app on Heroku"
date: 2015-07-14 22:53:54
tags:
- Heroku
- hosting
- tutorials
---
I created an angular app for practice that visualizes some data sets from [Sunlight API](https://sunlightlabs.github.io/datacommons/index.html)  Creating the app itself was pretty straightforward once I watched some angular tutorials and some start to finish apps being built from code school. I definitely recommend the soup to bits videos on code school, those were definitely the most helpful resources I came across.

However when it came time to host my app on Heroku so that I could share it with others, I ran into an entire load of issues. Strangely enough, the angular-seed app doesn’t come with it’s own server, but that might be because there are a lot of options for serving up angular. I saw people use flask and rails as deployment servers. I chose to use [Express](http://expressjs.com/), a lightweight node framework for web.

I followed this [tutorial](http://linqed.eu/2014/10/07/deploying-angular-seed-to-heroku/) specifically about deploying an angular seed app on heroku. One of the initial problems that I had was that I cloned the angular seed with a depth of -1 so that I didn’t have all of the commits from the angular-seed repository. But that causes problems with heroku, so I undid that with the git fetch —unshallow. I kept getting the CANNOT GET / after deploying to heroku.

It turns out that  this line `app.use(express.static(__dirname + '/app'));`
was not showing the pages from my app. We ended up removing the
 `+ ‘/app’` and adding an express redirect
 ```javascript
 app.get('/', function(request, response) {
  response.redirect('/app/views');
});
```
 and that served up the index of my angular app. Go checkout my [app](https://journeyinlearning.herokuapp.com/)!
