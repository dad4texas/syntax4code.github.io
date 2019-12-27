---
layout: post
title:      "Adventures in CLI Gem Scraping"
date:       2019-12-27 18:21:25 +0000
permalink:  adventures_in_cli_gem_scraping
---


I just finished my CLI Data Gem Portfolio Project and thought I might offer some insight to my fellow students that have yet to embark on this journey, or perhaps you have begun, but are having difficulty moving forward. 
I’ll have to admit the project at first was a bit intimidating, but it didn’t have to be. There are some steps I took that I shouldn’t have taken, and there were steps that I took that led to huge successes. To start out, I found the best web sites for scraping were sports sites, but there are other good sights for scraping as well.
1.	When choosing a sight, choose a subject matter you are interested in, it will make the project much more fun. I chose to scrape from a website called: https://www.fantasypros.com/nfl/reports/leaders/. This site had a list of the nfl players listed by rank. It offered basic information about each player and provided a link to gain access to more information about each player which fulfills the requirement of getting two layers of web page material.  It also had very well organized css selectors which is very important when you are trying to scrape very targeted information.

2.	I recommend using a couple of chrome extensions.
a.	The “Wappalyzer” Chrome extension is very useful for showing what programing languages are used on the sight. You will want to avoid scraping sights that use Angular, React and other java script frameworks.
b.	I also recommend using the “Selector Gadget” Chrome extension. This little app is amazingly useful when you are trying to get the correct css selections for the elements you want to scrape.
c.	Having a great text editor with some useful tools is helpful as well. I personally prefer using Microsoft’s “VS Code” on my Windows 10 desktop and on my Ubuntu Linux laptop. VS Code has tons of extensions and keyboard shortcuts that aid in the scripting and editing process.

3.	Once you have decided on a great site to scrape, it’s a good idea to create a flow chart of how you want the program to initiate the scraping, what information is going to be scraped, and how the program ends. 
For this I created a dialogue that guides the user based on their input. If the user wants to initiate the scraper, y is typed into the CLI prompt and the program takes off. If the user mistypes, an error message is given. If they type an x, the program is exited.  After the initial scrape, the user is prompted again, but this time they are asked if they would like more information about a player, if so, they type the player’s rank number into the CLI, and more information including latest news is provided to the user. Or they can type x again to exit the program.

4.	Using Flatiron’s video resources and looking at some of the scraper projects was very helpful. I would suggest looking at the “Student Scraper” and the “Worlds Best Restaurant” gem which can be found on github at: https://github.com/cjbrock/worlds-best-restaurants-cli-gem . Don’t get bogged down on making your gem exactly like the videos you watch because it is too hard to duplicate if you are trying to do the same thing on a different website. I was able to model my gem similar to the “Student Scraper”, but there was no way I would be able to duplicate it because my chosen site was so much more different and more complex. Also, if you get stuck, don’t flounder for hours and days, get help from you cohort. My cohort, was very instrumental in helping me with all sorts of issues, and they are happy to help.

5.	Finally, don’t get stressed out about the project, even though it can be very difficult at times, have fun with it. I kept a set of notes while on the project, and at the end of the day, I would notate where I left off with some details about what was accomplished and what I need to avoid. This helped me to stay on task and not go down to many unnecessary, time consuming  rabbit trails. Also, included in the notes were suggestions and resources that I could lookup in the preceding day, that might help the flow of the project. 

I must admit, now that my CLI Data GEM works seamlessly and the project is coming to a close, I am proud of what I have accomplished. However, the project is not the only accomplishment that has benefited me throughout this process. I have learned so much from being so immersed in it, and all the mistakes, and triumphs have catapulted my skill as a rubyist to a much higher level.  It has boosted my confidence and has made coding much more fun.

