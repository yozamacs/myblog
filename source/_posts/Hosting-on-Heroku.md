title: "Hosting on Heroku"
date: 2015-03-13 18:11:42
tags:
- Heroku
- Spring
- Java
---
 was finally able to connect to the heroku database after a lot of errors. I added a line in my mapper file to create a table if there wasn’t one. I’m not sure if that’s the correct way to go about it. There is also an option to migrate your local database to heroku’s database.

I had a lot of trouble with 404 errors. I wasn’t getting any information about why they were happening from the page or from the logs.

It was really confusing because everything was working locally, but would not work on heroku. It turns out that I needed an index.jsp file that the servers serves up upon opening

I also had a lot of trouble with the links. For a reason that I have not yet figured out, I have to use the .html appendix when linking between pages even though I have the .jsp declared in the spring beans. I’m going to do some more hunting around that.

I tried to declare mappings to any appendix in the web.xml file, but that didn’t work either. I ended up using the html links and also leaving my jsp files in the root of the web app folder.

I don’t like any of that, so my next task will be to figure that out.

In the meantime, the application is finally up and running! [Check it out](http://maryum.heroku.com/). I have a lot more I want to do with it. You can look at the source code [here](https://github.com/yozamacs/technicalList).
