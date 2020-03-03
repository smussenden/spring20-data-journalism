# Session 07 Instructor Notes

### Announcements
* Keys posted for lab and last class.

### Class reading baltimore sun
MY NOTES: 
* MAIN FINDING: When people are shot in baltimore, they are more likely to die.  For every 3 people shot, 1 dies.  
* MAIN ANALYSIS: Pretty simple analysis: they divided the number of shootings by the number of shooting deaths -- 937/300.
* FRAMING IT/IS THIS NEWS: Is it getting worse? Yes, it used to be worse.  HAVE THINGS CHANGED frame for NEWS.   
* FRAMING IT/IS THIS NEWS: Is that a lot or a little?  Context: compared it to other cities. In Baltimore, New Orleans and Washington, it's worse than anywhere else. IS IT WORSE OR BETTER here FRAME for news.
* MOVING BEYOND MAIN FINDING TO EXPLAIN WHY? head shots going up as are multiple shots (40 percent gun death head shot in 2000, 62 percent in 2015).  Guns more lethal. This despite the fact that medical care is improving.
* Bringing it to life: Holy shit the story top and this quote. “If I shoot you in the leg, I know what I'm going to get,” said Quinzell Covington, who is serving a 25-year sentence for murder. “If I shoot you in the stomach, I know what I'm going to get. If I shoot you in the head, I definitely know what I'm going to get. I'm going to get your demise.”  A STORY CAN EXIST IN THE DATA, in your R markdown file, but does it check out in the real world.  ARE PEOPLE ACTUALLY SHOOTING IN THE HEAD?  YES.
* THEN THE NUTGRAF: Covington's evolution into a killer encapsulates a trend driving gun violence around the country: Increasingly, people are shooting to kill...In many places, if you get shot, you are more likely to die than ever before.
* THEN THE DATA IN PLAIN LANGUAGE: In Baltimore, one of every three people struck by gunfire dies, up from one death in every four shootings the previous decade. It ranks as one of the most lethal of America's largest cities, according to a Baltimore Sun analysis. Two other cities — Washington and New Orleans — shared the brutal distinction of one in three shootings ending in a homicide in 2015. Like Baltimore, several cities have seen the death grip tighten. In Chicago, one in 10 people died after being shot in 2000; now one in six perishes. Last year, the odds for gunshot victims worsened in at least 10 of the nation's largest cities, The Sun found.
* DATA COMPARISON FLAWS: DC tracks Washington, D.C., counts non-fatal shootings as any time a person is shot at; the other cities count when victims are struck by gunfire.
* WHY NOT SHOW WORK? Would have liked to have seen data behind analysis.  Release these Markdown files.

### Review of difference between sum(dosage_unit) and n()
* Pull up last lab to show this for final question.
* When you are operationalizing the question, make sure you know what is what.
* The error many of you got would have been WRONG and would have required a correction.  This isn't some little "oh i misspelled a city name error", which, while problematic.  If you had been using this as the foundation of a news story, if it was the intellectual CENTER of the story, that's a HUGE deal.

### Review of Joins
* Joins allow us to take data in two unrelated tables and put them together.  
* There are lots of reasons for joins.
* Probably the most common reason is so that you can build efficient databases.  Joins allow you to avoid repeating the same information, as we'll see in a second.  Repeating information can lead to errors. We often get databases provided to us, which generally means multiple related tables.  So we have to know this to work with them.
* But the exciting reason for learning joins is what we call ENTERPRISE joins.
* It allows us to put together two seemingly unrelated data sets and use them to find something new.
  * One example: Enterprise joins allowed the Howard Center and NPR to determine that, in Baltimore and cities around the country, the hottest neighborhoods tended to have the fewest trees and highest ambient temperatures.  We joined neighborhood level tree-cover percentage and median afternoon temperature with a dataset of poverty rates from teh census.
* walk through, inner, outer, left and right joins
* Show a table with students in one table and grades in class in another table.  
  * Start with 4 students in one table and four grades in another class.  
  * Table 1: student id, student name.  Four rows: including one not in table 2.  
  * Table 2: student id, class name, grade. Four rows: including one not in table 1.
* Show inner join, left join, right join, full outer join.
* Then, modify table 1 and table 2 student id column to have different names.  Explain that join still works, just need to specify in r that this column with this name should be matched with this column with a different names.  What MATTERS is that the values in it mean the same thing.  You could see how this could cause you trouble if they don't mean the same thing.  Cause the match would execute.
* Then, modify table 2 to have grades from multiple classes.  And show how you get the one-to-many match.  Ask: can anyone see how this could cause problems if we tried to COUNT the number of students by doing a count here?
