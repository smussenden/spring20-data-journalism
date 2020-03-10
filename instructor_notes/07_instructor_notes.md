## 07_instructor_notes

## Announcements
* Keys posted
* Data Acquisition: Everyone right now look at comments.  Did I say I needed to talk to you?  Raise hand, I'll write on board.  
* Assignment due dates
  * Spring Break is next week.  Everything is due this SUNDAY. Not SUNDAY just before we return.  This SUNDAY.
* Contingency plans
  * If you are sick, go home please.  
  * Nothing decided.  But we've been asked to think about how we might teach classes if restrictions are put in place (i.e. campus closing, meeting sizes limited).
  * I hope to continue this class as is, if we can't meet in person.
  * Class will continue to meet at same time via Webex or Zoom.  Study sessions at same time.  
  * It may require an adjustment on our part, but I'm pretty sure this will work okay.
  * As soon as I know something, I'll post to ELMS.
  * Questions?  

## What's an API?

* What's an API?
  * An "Application programming interface" allows you to pull data from a third-party database directly into your environment.  
  * An alternative to loading files locally.  Have to follow specific rules or methods to get the data as determined by owner of the data. There is generally a guide/reference/documentation telling you what you can get and how to get it.
  * [Twitter API](https://developer.twitter.com/en/docs/tweets/search/api-reference/get-search-tweets) and [RTweet R Package](https://rtweet.info/)
  * [ARCOS raw data download](https://github.com/wpinvestigative/arcos#download-the-raw-data) and [ARCOS R package](https://wpinvestigative.github.io/arcos/)
  * [Census Data](https://data.census.gov/cedsci/) and [Tidycensus R Package](https://data.census.gov/cedsci/)

### Chicago Tribune Reading

* Philip and Laina presenting

First story: pharmacists ignoring drug pairs.
* More straightforward analysis method.
* Key notes: They BUILT a database. tested 255 pharmacies to see how often stores would diagnose dangerous drug pairs.  
* The analysis was then simple: majority = more than half.
* WHY HAPPENING? Data couldn't answer.  Reporting through interviews found: speed and market forces.
* Got results: CVS, Walgreens, Wal Mart also changed policies to stop.
* Show the harm: missed opportunity to incorporate patients into this story.
* "Pharmacies miss half of dangerous drug combinations" highlights a major problem: 52% of pharmacies sold potentially dangerous medication combinations without warning patients ("They failed to catch combinations that could trigger a stroke, result in kidney failure, deprive the body of oxygen or lead to unexpected pregnancy with a risk of birth defects"), a huge issue considering that the rate of patients taking 5+ prescription drugs has doubled since 1994.
* Independent pharmacies (72% failure rate) were more likely to fail to warn patients than chains (49% overall failure rate), but some larger chains still had failure rates above 60%. One culprit: emphasis on filling prescriptions quickly – one Walmart pharmacist mentioned filling a prescription every 2.7 minutes.

Second story: identifying dangerous drug pairs.  
* VERY complex. Used machine learning classifier to predict whether a particular drug combo was problematic.  A form of machine learning: code that you can teach.  Parse through a bunch of data, and learns. Well beyond scope of this class.   
* I have a data science masters degree, and I wouldn't feel comfortable doing this work on my own.
* Tribune partnered with researchers, who did this work.  They published an academic paper! https://link.springer.com/article/10.1007/s40264-016-0393-1#Sec2
* One takeaway: doing something even a little complex, working with experts and helping develop methods and results is KEY.   https://www.cjr.org/first_person/could_collaborating_with_scientists_be_the_next_step_for_investigative_reporting.php

Why this matters?
* One in five Americans takes three or more prescription drugs, and one in 10 take at least five or more.

Q: should journalists do this kind of work?

* ONe side: We're not social science researchers.  We should leave that to people with real expertiese.  Use data to identify SIMPLE patterns and trends, and use it to find evidence, characters, places.
* Other side: yes.  If done carefully, can lead to newsworthy results that researchers MAY not be inclined to do for various reasons.
* Me: I come down in the middle.  Do it in partnership with researchers.  


### IN CLASS LAB
