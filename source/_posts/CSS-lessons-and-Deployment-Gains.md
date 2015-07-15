title: "CSS lessons and Deployment Gains"
date: 2015-05-12 11:50:43
tags:
- Spring
- Java
- CSS
---
Lessons learned:

CSS Files
If you want a certain CSS file to override another (for example, if you’re using a theme from someone else and you want to override portions of their styles with your own) then place your CSS file at the bottom. The bottommost file overwrites any conflicts from the previous ones. It took me a lot of google searches to find that!

Tomcat Spring local deployment
I am working on my goal project right now, and to deploy it to Tomcat and view it on local host, I was calling mvm install to create a war file and then manually copying it to the web apps folder in the tomcat folder on my computer (via terminal). However, after starting the process of deploying my app to Heroku, I saw a no sweat way of deploying my app locally. You just type:

java -jar target/dependency/webapp-runner.jar target/*.war

You can see the reference [here](https://devcenter.heroku.com/articles/java-webapp-runner).

I wish I could say my simple local deployment has gone as simply as my heroku deployment, but it has not. I am getting errors that seem to be related to dependencies not matching up. Hopefully I will be up and running soon.
