# WORKING DRAFT INTENDED FOR FEEDBACK!!!!!

# After hearing a lot of feedback, I'll be adjusting this to be adding features to an existing application, rather than starting from scratch. Thanks.

# Internship at Hearken

## Introduction

[Hearken](http://www.wearehearken.com/) focuses on developing tools and processes to help newsrooms and other media outlets better engage with their audience in the pre-publication phase of a story, from idea inception through the reporting process. Our first offering is a set of tools, including embeddable modules, to gather questions from the audience and allow them to weigh in via voting on what story should be reported. We are a small team, consisting of our CEO, [Jennifer Brandel](https://twitter.com/JnnBrndl), our CTO, [Corey Haines](https://twitter.com/coreyhaines) (me), and our lead developer, [Sam Withrow](https://twitter.com/typwrtr).


We are looking for an beginner-level intern to join us for a 2- to 3-month contract, spending 30 hours per week working with us. While the internship will be focused on developing features for our tools, we look at this program as a learning opportunity for the participant. Work will be done under the guidance of senior-level developers with frequent discussions about simple design, testing and other development practices. We are intending to begin with a single intern, but hope to move to a cohort of 3 by the end of the year. Unfortunately we aren't in the position (yet) to hire someone full-time, but this internship can be a great stepping stone in your job search.

We are looking to start in August, 2015. Due to the nature of the internship and our capacity, we currently are only accepting applications from people who can be physically present with us in Chicago.

## Our technology

Our technology stack consists of a Ruby on Rails back-end server, with a backbone-based web front-end. We lean towards server-side logic and rendering with traditional AJAX techniques.

## What you get

During the course of the contract, you'll be working closely, in-person, with Corey. While our primary goal is to ship functionality for our customers, this internship has a strong learning component. You can expect regular code reviews, discussions about coding and a welcoming, non-judgmental atmosphere to ask questions when you don't know how to do something.

* 2- to 3-month contract internship working on a real-world, production application that is used by media outlets and newsrooms around the country.
* $20 / hour for 30 hours a week paid as a contractor.
* LinkedIn recommendation at the end of the contract.
* Regular code reviews (all work is merged in with pull requests, so there is room to discuss).
* Weekly 1-1s to talk about anything, not only code (want to talk about your career? we can talk about that. want some feedback on speaking? that's cool, too).
* Ad-hoc discussions of simple design, testing and rails best practices (example: why did you make a whole new controller just for that one action?).
* Free copy of Corey's book, [Understanding the 4 Rules of Simple Design](https://leanpub.com/4rulesofsimpledesign/).

## How to apply

In order to apply, a small application should be written and submitted. This application should be representative of your skills and techniques building a traditional Rails application. We're interested in seeing not just the end result, but also the steps along the way: please make a lot of commits with good comments as you develop to highlight your thought processes.

Submitting can be done with the following steps:
* Fork this repository
* Create a branch with your name
* Complete the challenge
* When finished, submit a pull request against this repository.

**Note:** We understand that there can be various reasons you might not be comfortably publicly submitting your code. If you have concerns, please email [corey.haines@wearehearken.com](mailto:corey.haines@wearehearken.com), and we will find an alternate method. Submitting your application in private will IN NO WAY affect your chances.

## Application requirements

I love cats! With the recent studies released that have definitively shown that looking at cat pictures is beneficial to your health, I have decided to save the world via a new web application called "ZOMG! CAT HEALTH!" This application consists of randomly showing two cat pictures. The user is presented with a button below each picture, one says "ZOMG! So Cute!" and the other says "Amazing! So Beautiful!" For each pair of pictures, the user selects one by pressing the button below it. After clicking the button, two more random pictures are shown, and the user is invited to select again. This process is repeated until the user closes the browser.

You can think of it this way:
* System should randomly show two pictures of cats with a button under each: one says "ZOMG! So Cute!"; the other says "Amazing! So Beautiful!"
* Visitor "chooses" a cat by pressing the associated button.
* After choosing one, the system presents the user with two more cats to choose from.

Of course, while this application is world-changing and will clearly be a hit just from a health perspective, we also want to do some data analysis on which cats are primarily "ZOMG! Cute!" and which are "Amazing! So Beautiful!" We'll also want the ability to add new images. So, we need to put together an administrative backend. There are a few functions that need to be built.

The administrative backend should be restricted behind a login. You don't need to worry about user registration, as we can manually create the users in the database. Please use Devise for the user authentication.

Once logged in, the user can do the following tasks.

Managing cat pictures will be done with standard CRUD (create-read-update-delete) functionality. A cat picture consists of a URL pointing to the picture (we don't want to worry about the complexity of self-hosting the pictures).

**Note:** You can find in this repository a file called "seed_cats.txt" containing a set of URLs of pictures of my cats, Zak, Pistachio and Squeaks. Please use this list to to seed the system.

Also behind the login should be a reporting page that shows the cats, as well as their current statistics for "ZOMG! Cute!" and "Amazing! So Beautiful!" votes. It is important to be able to see which cats are doing well in which category, so please make a way to do this.

I would also like the ability to download a CSV of all the votes that includes the following information: cat url, ip address of voter, which vote.

You can think of it this way:
* System has an administrative section protected by a login.
* Support standard CRUD (create-read-update-delete) function for a cat picture. A cat record consists of a URL to the image.
* Have a page to view top-ranking cats, based on the number of "ZOMG! Cute!" and "Amazing! So Beautiful!" votes they've received.
* Provide export functionality for all votes into a CSV: cat url, ip address of voter, which vote.

## What to focus on?

This challenge is about showing what we can expect if you join our internship. We understand that you are a beginner, so please do your best, but make it representative of your own work; we value solid, quality work, rather than the latest and fanciest technology.

Some aspects of what we are looking for:
* Maintainable code
* Testing
* Understandability of code

## Questions?

Feel free to email [corey.haines@wearehearken.com](mailto:corey.haines@wearehearken.com).
