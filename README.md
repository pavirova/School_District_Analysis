# School District Analysis

## Project Overview
The purpose of this analysis is to apply our knowledge of Python while using Pandas and Jupyter notebook to analyze different metrics regarding math and reading score for different high shools. A similar analysis was conducted, but since the initial analysis, it has been discovered that there was cheating in Thomas High School amongst the 9th graders. Our goal is to rerun the analysis after making the 9th grade math and reading scores NaN or "Not a Number", and seeing how not accounting for the ninth graders in Thomas High School affects the overall analysis.

## Results

### - How is the district summary affected?

Module Result
![district_summary_module](/district_summary_module.png)

Challenge Result
![district_summary_challenge](/district_summary_challenge.png)

As can be seen from the above images, there were different parts of the district summary that were changed after we replaced the Thomas High School (THS) 9th grade students' math and reading scores with NaN. When looking at the results rounded to the tenths place, we see that the average math score, average reading score, % passing math, % passing reading, and % overall passing decreased. They did not decrease by too much, however, since we removed only the 9th graders from one of the high schools, and they take up a very minor percentage of the total students involved. We can see that accounting for THS 9th grades students was slightly driving the score averages up.

### - How is the school summary affected?
Module Result
![school_summary_module](/school_summary_module.png)

Challenge Result
![school_summary_challenge](/school_summary_challenge.png)

When we compare the images above, we can see the average math score, average reading score, % passing math, % passing reading, and % overall passing decreased for Thomas High School, but remained the same for the rest of the schools. This makes sense, since we removed average scores that were overall pushing the average slightly higher. Though all decreased very little, the parameters that decreased the most were the % passing reading, which decreased by about 0.29 %, and the % overall scores, which decreased by about 0.32%.

### - How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Module Result
![top_schools_module](/top_schools_module.png)

Challenge Result
![top_schools_challenge](/top_schools_challenge.png)

From the images above, we can see that even though the metrics for Thomas High School went down (as shown in the school summary), the ranking at Thomas High School stayed the same. The decrease in scores and percentages were so small that it kept THS at the same ranking, the second best-performing schools. The change is minor because the number of student's scores that were removed is very small compared to the total students at THS.

### - How does replacing the ninth-grade scores affect the following:

#### - Math and reading scores by grade:
Since the math an reading scores for the 9th graders in THS were replaced with "NaN" those Thomas High School 9th grade students' scores are the only ones affected, since no other school's data was altered.

#### - Scores by school spending
Module Result
![spending_summary_module](/spending_summary_module.png)

Challenge Result
![spending_summary_challenge](/spending_summary_challenge.png)

The two spending summaries above show that the spending range that was affected was the $630 - $644 spending range per student. The images above show all decimal places so we can more clearly see the differences in the scores and percentages. Removing the 9th graders from THS lowered the average math and reading scores which in turn affected the percentages of students that are passing reading and math. The overall passing percentage went down by about 0.079%, again, not very different since the sample 9th graders at THS was small compared to the total number of students involved in the analysis.

#### - Scores by school size
Module Result

![size_summary_module](/size_summary_module.png)

Challenge Result

![size_summary_challenge](/size_summary_challenge.png)

The two summaries above show that the school sizes that were affected by removing THS 9th grade students were the medium sized schools, wich makes sense, since THS's student number falls under that medium school range. As can be seen from the images, all parameters for medium size schools went down slightly except for the average reading score, which actually went up by about 0.01%.

#### - Scores by school type
Module Result

![type_summary_module](/type_summary_module.png)

Challenge Result

![type_summary_challenge](/type_summary_challenge.png)

When organizing the data by school type, it's clear that charter schools are affected. Removing the 9th graders from THS lowered all parameters slightly except for the average reading score, which actually went up slightly, by 0.006%.

## Summary:
In summary, major changes that happened from switching the 9th grade THS scores to NaN, is that it caused both the math and reading averages in THS to go down. This, along with the new student count at THS being accounted for, lowered the % passing math and the % passing reading scores. On a larger scale, removing the 9th graders from THS also lowered the overall passing percentage in medium schools, as well as the overall passing percentage for charter schools. 
