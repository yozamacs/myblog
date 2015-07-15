title: "Open Source Adventures"
date: 2015-05-13 18:12:46
tags:
- Open Source
- Java
---

Open source software is something that I’ve always wanted to get involved in. To me, it’s the coolest thing about software development. The ability to create software with people all over the world that also has the ability to make the world better.

Up until now, I’ve just browsed various open source repos looking at something that I think can help. But I was pretty intimidated by a lot of the open issues that I saw in a lot of the repos. Fortunately, my coach directed me towards a pretty cool android project that is the android client for openMRS.

OpenMRS is a Java-based, web-based electronic medical record. You can find out more about it [here](https://wiki.openmrs.org/display/docs/Introduction+to+OpenMRS)  The project I am looking at is an android [client](https://wiki.openmrs.org/display/projects/OpenMRS+2.x+Android+Client) for OpenMRS.

So far I have forked the code. I had some trouble running the tests. As a part of their build they have code review tools that checked for unused variables and unused imports. My code wouldn’t build because I hadn’t finished writing my tests. Eventually, we got the project to build after commenting our my half written test.

I also had problems with IntelliJ not recognizing the android code, but it turns out I had my project language set to Java 8 and not Android. I am still having trouble getting the emulator to work, to run the tests. My emulator is just hanging, with the Android logo refreshing over and over. It did load once, but I can’t recreate that at the moment. Looking forward to finishing the tests I’m writing and seeing them run on the emulator.
