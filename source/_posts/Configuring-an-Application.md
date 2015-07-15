title: "Configuring an Application"
date: 2015-04-12 11:48:13
tags:
- Java
- Spring
---
Lately I’ve been having trouble configuring a spring application to run on a server and connecting it to a database through spring. The latter, the database connection, I found tutorials about, but wasn’t sure if what I was doing was working, since I couldn’t see the application.

 Part of my confusion was due to working on this spring application in the IntelliJ pro edition, which deploys your application to a tomcat server automatically. When I made the switch to IntelliJ community edition, there was no support for launching in tomcat. Fortunately, I was able to work with my coach and we used maven to create a WAR file from the application code and put that in the tomcat web apps folder and launch the application manually.

There was an interesting [blog post](http://www.daedtech.com/faking-tomcat-support-in-intellij-idea-community-version) that had a ant build file that does all of the above. I don’t know much about ant. I just looked it up ant and saw that it was a command line tool used to build applications. Definitely something to add to the list of things to know.

After finally getting the app up and running on the tomcat server, we were able to address the database connection issues. There were numerous issues, including not having the spring jdbc library, needing both the mybatis and mybatis spring dependencies, and an outdated version of the javax servlet. With all of that out of the way, I still need to get the database aspect working. But I feel so much better after a lot of the configuration that has puzzled me for months.
