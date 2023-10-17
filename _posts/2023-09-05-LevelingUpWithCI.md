---
layout: post
title: Leveling up with CI
image:_posts/PowerBI_LevellingUp.png
tags: [PowerBI, Microsoft Forms, SharePoint, Data Analysis]
---
![Leveling up with CI](https://github.com/metzma/metzma.github.io/assets/101017804/9eb707fd-0774-4f78-a154-81b3087b5161)

In this project, our Continous Improvement team was looking for a solution that could help generate additonal interest from IT associates to particpate in identifying and implementing technology solutions or workflows to improve current processes and contribute to cost reduction savings to the IT department.

# Table of contents

- [00. Project Overview](#overview-main)
    - [Context](#overview-context)
    - [Components](#overview-actions)
    - [How it was built](#overview-results)

___

# Project Overview  <a name="overview-main"></a>

### Context <a name="overview-context"></a>

In this project, our Continous Improvement team was looking for a solution that could help generate additonal interest from IT associates to particpate in identifying and implementing technology solutions or workflows to improve current processes and contribute to cost reduction savings to the IT department.  An subcommittee was formed by members of the CI team.  This group had the idea to gamify the process.  We came up with badges to help individuals increase their standings within CI activities.  
Badges were based on the CI mascot of Yoda and utilized a Star Wars theme. Badge levels include: Wookie, Beginner, Intermediate, Advanced, and Expert. The colors of the badges coincide with the colors of the Lean Six Sigma belts. A Microsoft SharePoint page was adding the to CI SharePoint site to have a landing page for this initiative. 

<br>
<br>
### Components <a name="overview-actions"></a>

The subcommittee wanted to be able to have participants be able to do the following things:
* Learn more about how to participate
* Self-report their CI activities
* View their progress on a leaderboard

Technology used:
* Microsoft SharePoint
* Microsoft Forms 
* Microsoft OneDrive
* Microsoft PowerBI

### How it was built <a name="overview-results"></a>

The CI team already had an existing SharePoint site. I was able to add a SharePoint page to the site.  A Quick Link was added to the primary landing page of the CI SharePoint site.  From there, a graphic was added a header image.  

The team wanted a text block added for displaying points to the specific badge levels.  The following badge levels are: Wookie, Beginner, Intermediate, Advanced, and Expert. The team also wanted a way to indicate the number of points earned per activity which was displayed in a text box. 

A Microsoft Form was added to the page.  The Micorsoft Form was added to my OneDrive account, by utilizing "Forms for Excel" within the new button inside OneDrive.  By adding the form through "Forms for Excel", this allows your forms to write to an Excel Online spreadsheet that does not need to be downloaded in order to view the most recent responses.  Responses can then be tracked in real-time.
Then within PowerBI, I added a connection to my Excel Online source within my OneDrive account.  This allowed for every refresh to pick up any new forms entries based on participants submissions.

Within PowerBI, I added 4 KPI cards with custom icons to represent the following metrics via DAX measures:
* Participant Count
* Submission Count (All time)
* Number of Points Submitted
* Submission Count (Last 30 days)

A table visual was added to the report that contains the following columns:
* Rank
* Partcipant Name
* Total Points
* Badge Level

This model consists of 3 tables:
* Submissions
* BadgeLevels
* ActivityPoints

Rank was dynamically calculated via a DAX measure.  The BadgeLevels table contained an upper and lower bounds for each level, which was then correlated back to the total points for a given user. 

<br>
<br>

