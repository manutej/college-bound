## Problem Statement

 You are a part-time tutor who also dabbles in data science. You have several students who are struggling to understand what the future holds for them and how standardized tests fit into their life path. They are feeling overwhelmed with all the data around "acceptable test scores" for various schools and majors. They want a good education, but need some help narrowing down the choices for majors and schools, based on their target (or expected) SAT score range. Can you help them to make an informed decision in a time-sensitive situation before the application deadline?

The SAT and ACT - the disdain of many young High School Seniors. The process for preparing for this test and all the other bells and whistles of college applications, not to mention which colleges to choose for a critical next step in a student's education. At times, much of this can be overwhelming for students, and this has been my experience with talking to many young individuals who feel lost between the cracks through this process. are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university. Standardized tests are simply a way to allow colleges to distinguish "qualified" applicants across a large population where each school or state may have different standards, educational practices etc. Therefore the initial idea of the standardized test was to create a common comparison metric to measure academic performance across all backgrounds. 

Therefore, in order to help these students feeling overwhelmed, we need to provide them a new way of looking at their possible options and also to understand a little more clearly where they might stack up for a given college and for a given intended major. After all, it is important to go into this next phase of life with an informed outlook of the landscape. Often times, the resources (especially free resources) are among slim pickings to find the best options for an informed decision, planning, and preparation for this critical transition in a student's academic career. 



### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|intended_major|object|2019 SAT Scores by Intended College Major|The name of various majors and fields of interest for prospective college-bound applicants.| 
|test_takers_per_major|float|2019 SAT Scores by Intended College Major|The number of test takers who are interested in major| 
|percent_of_total_decimal|float|2019 SAT Scores by Intended College Major|Percent of total expressed as a decimal| 
|total_accepted|int|2019 SAT Scores by Intended College Major|Total number of students accepted for the intended major| 
|reading_writing_sat_score|int|2019 SAT Scores by Intended College Major|Score for the reading and writing SAT section| 
|math_sat_score|int|2019 SAT Scores by Intended College Major|Score for the reading and writing Math section| 


|Feature|Type|Dataset|Description|
|---|---|---|---|
|school_name|obj|Ranges of Accepted ACT & SAT Student Scores by Colleges|Name of the University or College |
|number_applicants|int|Ranges of Accepted ACT & SAT Student Scores by Colleges|Number of applicants for this college|
|acceptance_rate|float64|Ranges of Accepted ACT & SAT Student Scores by Colleges|Acceptance rate as a decimal|
|sat_quartile_range|object|Ranges of Accepted ACT & SAT Student Scores by Colleges|SAT Quartile range (as a string)|
|act_quartile_range|object|Ranges of Accepted ACT & SAT Student Scores by Colleges|ACT Quartile Range (as a string|
|sat_lower_quartile|float64|Ranges of Accepted ACT & SAT Student Scores by Colleges|SAT Score marking the lower quartile for the given college or university|
|sat_upper_quartile|float64|Ranges of Accepted ACT & SAT Student Scores by Colleges|SAT Score marking the upper quartile for the given college or university|

## Conclusions and Discussion
### Based on all this data, we can conclude that being able to look at the subscores and SAT Quartiles of scores that correspond to certain majors or colleges is a useful way to approach becoming informed about the process. By sorting our score values we were able to understand which were the majors that correspond to which of the top scores. For example, it helps to know that if I want to pursue an engineering degree, I will probably want to make sure to have a high math score, but also a high reading and writing score (as opposed to the conventional logic of just needing math). Furthermore, this project was a beginning entry point into the world of data science. Future projects could include building a machine learning recommender system that allows one to take all of these colleges with a corresponding score and recommending automatically the best college/major for a given student's score. 