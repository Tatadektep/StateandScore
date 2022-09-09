# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis


### Problem Statement


1. It is increasingly unaffordable to pursue higher education in the United States of America. There are numerous barriers for students to pursuing higher education. Affordability is one of the primary barriers. As financial investment required to take a semester course is considerable. 
2. Higher education is becoming more competitive. This would exacerbate the inequality as college graduates tend to earn more cumulatively than high school graduates. This is particularly true in underserved groups that are less likely to attend college, such as inner-city and rural populations. 
3. The cost of living for some states has been increasing significantly from the cost of goods, housing costs, utility costs, transportation costs and miscellaneous costs. The option for remote work has become more common. Should remote workers and their family move to a different 
state to save cost and maximise the likelihood to obtain higher education with limited resources?

---

### Background
Education is fundamental to development and growth of our children as it is one of the most important factors to create opportunities and successes. Yet, there is a significant between the states due to the vast difference among U.S. states policies. U.S. school systems are very similar to one another, teacher labor markets are not drastically different, and education systems are regulated under the same federal rules. If students with similar family academic resources in some states make much larger gains than in other states, those larger gains are more likely to be related to specific state policies that could then be applied elsewhere in the United States.1

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications ([*read more about this here*](https://www.cnn.com/2020/04/14/us/coronavirus-colleges-sat-act-test-trnd/index.html)).

### Datasets
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State
* [`cost_2019.csv`](./data/cost_2019.csv): 2019 Cost of Living by State
* [`cost_2019.csv`](./data/cost_2020.csv): 2020 Cost of Living by State
* [`cost_2019.csv`](./data/cost_2021.csv): 2021 Cost of Living by State

#### Provided Data

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|sat17-19|A state is a constituent political entity, of which there are currently 50.<br> This dataset also includes District of Columbia. The total number states in this dataset is 51.| 
|**participation**|*float*|sat17-19| Participation rate is a percentage of student taking SAT. There mulitiple factors affecting the rate from required testing or favouring of ACT by the state.
|**english**|*float*|cost| English is an average SAT score of Evidence-Based Reading & Writing. The minimum score is 200. The maximum score is 800.
|**math**|*float*|cost| Math is an average Math SAT score. The minimum score is 200. The maximum score is 800.
|**total**|*float*|cost| Total is an comprising of average English and Math SAT score. The minimum score is 400. The maximum score is 1600.
|**cost_index**|*float*|cost| Cost of living indexes meant to compare the expenses an average person can expect to incur to acquire food, shelter, transportation, energy, clothing, education, healthcare, childcare, and entertainment in different regions.
|**housing_cost**|*float*|cost| Housing cost of living indexes meant to compare the housing expenses an average person can expect to incur in different regions.
|**average_participation**|*float*|cost| Average score is a 3-year average of participation rate from 2017 to 2019.
|**average_score**|*float*|cost| Average score is a 3-year average of total SAT score from 2017 to 2019.
|**average_cost**|*float*|cost| Average cost is a 3-year average of cost of living indexes from 2019 to 2021.
|**score_cost**|*float*|cost| Score cost is a 3-year average score over cost of living indexes. <br> 15 can be intrepret as 1500 SAT score for national average (100) cost of living index.
|**score_house_cost**|*float*|cost| Score housing cost is a 3-year average score over housing cost of living indexes.

### **Conclusions**
1. Expensive States do not have to better average SAT score at state level. Therefore, relocating to lower cost of living states are likely to have no negative impact on test score.
2. There is a strong negative correlation between average participation rate and average score. The most likely explanation is only highly qualified candidates take the SAT in low average participation states.

### **Recommendations**
1. Mississippi, Kansas and Missouri are great states for consideration for most value state for SAT score by cost of living. 
2. The education policies differ significantly between the states further research is needed before considerations.

### Additional Information
Carnoy, M., García, E. &amp; Khavenson , T., 2015. Bringing it back home: Why state comparisons are more useful than international comparisons for improving U.S. education policy. Economic Policy Institute. Available at: https://www.epi.org/publication/bringing-it-back-home-why-state-comparisons-are-more-useful-than-international-comparisons-for-improving-u-s-education-policy/ [Accessed September 8, 2022]. <a class="anchor" id="fourth-ref"></a> 

Cheng, A., 2021. Average SAT scores by state (most recent). Average SAT Scores by State (Most Recent). Available at: https://blog.prepscholar.com/average-sat-scores-by-state-most-recent [Accessed September 8, 2022]. <a class="anchor" id="first-ref"></a> 

Council for Community and Economic Research (C2ER), 2022. What is the Cost of Living Index? C2ER Cost of Living Index. Available at: https://www.coli.org/about/ [Accessed September 8, 2022]. <a class="anchor" id="second-ref"></a> 

Reynolds , R., 2021. The impact of affordability. TEL Education. Available at: https://www.tel-education.org/the-impact-of-affordability/ [Accessed September 8, 2022]. <a class="anchor" id="third-ref"></a> 
