# Paths4All
A strength and balance mobile app for people in care homes or suffering from dementia.

Link to logos, fonts and brand guidelines:
https://pathsforall-my.sharepoint.com/:f:/g/personal/carlg_pathsforall_org_uk/EtMTihASdghHsxrH9GDw7-wBI6TTJ3X1nhECuhPnppgiOg?e=D9lOGh

Hex colour codes for strength and balance artwork:
Orange – #EB6012
Brown – #281A08
Light Brown – #9F662D
Cream – #F3F0E3

Link to artwork for strength and balance graphics:
https://pathsforall-my.sharepoint.com/:f:/g/personal/carlg_pathsforall_org_uk/Eq7lhFCD52NGnz4UOm1AGmsBpqPucXLVh7Y_RofgyXp2BQ?e=wKV40I

Strength and Balance app - Technical briefProject Brief:

PFA’s Strength and Balance programme consists of 8 simple exercises that can improvestrength and balance and reduce the risk of falls in older adults. The exercises are promotedas part of our work with walking groups, care homes and online through a series of videos.They are made available through staff and volunteer training and a suite of resourceincluding leaflets and interpretation panels that have been installed in care homes.We would like to create an app that could be used by a range of groups to guide themthrough each of the eight exercises. As well as the general public, Paths for All wouldpromote this specifically to:

Care home and sheltered housing residents
People receiving care and support after a hospital admission
Participants in our programme of health walks
Health and social care professionals to use with clients and patients

Below are some suggestions for the core functionality of the app:
Android and iOS versions
Mobile and tablet friendly
Free to download
Uses existing dementia friendly strength and balance graphics and copy
Home screen with start tab
8 x strength and balance exercises with the following functionality:
  Overview of exercise programme and start tab
  Beginner, intermediate and advanced levels
  Intro and start button
  Exercise screen with timer and pause option
  Arrows to go back to previous exercise and skip to next one
  Animated exercise instruction
  Congratulations on completing the exercise routine
  Ability to tailor sets/ timings for each exercise – could be set by the user ora health professional e.g. physiotherapist
Calendar overview of activity – each record has number of exercises and time
taken
Reminder with motivational message – ability to toggle on and off and set time
Info page on exercises and signposting to PFA
About and contact
Delete data
Share
Privacy statement

First iteration MVP:
As a user, I’d like to be able to use the app on both IOS and Android, and the appshould be responsive on both phones and larger tablets.
As a user, I’d like to be greeted with a Home/Start page upon opening the app
As a user, I want to be able to start the set of exercises
After clicking on start, I want to be able to see the first exercise’s first stepdisplayed with the helping text
Swiping or clicking on the image should switch to the next step of the exercise(optionally it can switch to the next step after a set amount of time (8-10seconds?))
(Later iteration can replace this with a proper animation)
As a user, I’d like to see 5 circles and a timer at the bottom of the app, touching acircle should mark it as done for a set of exercises, restarting the timer
After all 5 circles are marked, a new button should appear to progress to the nextexercise, with a message congratulating the user before the next exercise starts
As a user, I’d like to navigate between the exercises with arrows

Progress as you see fit, a recommended starting workflow would be as such:
1.Create an app in Firebase, using a new google account
2.Create the Firestore Realtime Database that’s seeded with a structured objectcontaining the necessary instructions for the exercises, and URLs for the relatedimages
3.Either after or meanwhile, create front-end to the application - get a basic Hello Worldup and running with both Android/IOS/Web App.
4.Create a standard landing page, with clickable start icon to kickstart the app

Tech stack with tutorials:
Mobile app - using ReactJS○React Native tutorial: https://facebook.github.io/react-native/docs/tutorial
Very lengthy (5+ hours) crash course for free on YouTube:https://www.youtube.com/watch?v=qSRrxpdMpVctr
Styling of React Native apps
https://blog.bitsrc.io/styling-in-react-native-c48caddfbe47○Quick 
intro to styling in ReactNative:
https://www.reactnative.guide/8-styling/8.0-intro.html○Great 
blogpost on responsiveness with ReactNative:
https://medium.com/react-native-training/build-responsive-react-native-views-for-any-device-and-support-orientation-change-1c8beba5bc23
Back end -Firebase (use it to store the images, text, and later the animations in Firestore Realtime Database
Firebase resources:○https://www.youtube.com/watch?v=e1Cm-jj0CG4
video tutorial onFirebase’s Realtime database
https://firebase.google.com/docs/database/?authuser=0
- Firebase documents on Realtime database
No need for authentication for the time being

Technical challenges:
Responsiveness is key - app must be usable on different sized screens and ondifferent platforms. Make sure the app is responsive on all apps
User needs and end user group is very specific - check with the client constantly tomake sure requirements are met

Styling/wireframes:
TBD with client, see document for branding guidelines.Inspiration:
Plank app:https://play.google.com/store/apps/details?id=fat.burnning.plank.fitness.loseweight&amp;hl=en
For the timer/5 counters at the bottom:https://play.google.com/store/apps/details?id=com.stronglifts.app
Notes: Make sure to properly document everything with the app — how to start the app, how tofind any credentials you might use, what tools to install (potentially creating a script to install tools)
Good README templates:
https://github.com/othneildrew/Best-README-Templatehttps://gist.github.com/PurpleBooth/109311bb0361f32d87a2
List of good README examples:
https://github.com/matiassingers/awesome-readme
Remember: Leave a README/documentation/Diary for the upcoming cohort that you’dlike to get when you start!
