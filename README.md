# Job Recommendation

Final project for the Building AI course

## Summary

Many people are getting jobs they don't really like. Based on a person's interests & skills this project aims to recommend jobs that make people happier.

## Background

Many people are getting jobs they don't really like. According to a global survey<sup>[2](#fn2)</sup> about job satisfaction from 2013, almost half of employees are unhappy in their jobs.
Often poor job choices are made due to students' lack of knowledge about certain jobs when deciding on their future career.
Which problems does your idea solve? How common or frequent is this problem? What is your personal motivation? Why is this topic important or interesting?

## How is it used?

The solution could be used in schools to prepare children for their future work life. By making students aware early on about jobs that they might've not heard about before but that fit well with their interests & skills, low job satisfaction can be prevented.

## Data sources and AI methods

In my brief research I haven't found any data that could be used to corelate interests & skills with jobs that people are happy with.
Thus this project requires making a large scale survey of employees across many sectors. They should be surveyed about their interests, skills (mainly soft skills) & their job satisfaction.

The resulting survey data might look something like this:

| job               | interests                     | skills                                    | satisfaction |
|-------------------|-------------------------------|-------------------------------------------|--------------|
| Software Engineer | computers,                    | logical thinking                          |     0.8      |
| Data Scientist    | computers, AI                 | mathematics, statistics, logical thinking |     0.85     |
| Writer            | books, stories, relationships | imagination, writing                      |     0.9      |

Since there are many synonyms for we need to preprocess the results by using common terminology for synonymous skills or interests.

Given suufficient data a neural net should be trained to find the corelations between interests & skills and jobs with high satisfaction rates for those.

## Challenges

There is a huge risk that bias could affect the job choices of many people. The tool might cause people to go into specific sectors more than others. If used on a big scale this has potentially negative effects on the job market. Also even if everyone is able to find a job they'll like this might not match the actual demand in the job market. Perhaps the model could be improved to incorporate market demand in recommendations to avoid this.

Additionally some people might still not find their dream job if they don't supply enough interests & skills or their chosen data cannot easily be matched to a job. This needs to be evaluated during the development.

## What next?

The biggest problem seems to be acquiring the data needed to train the model.
Some of the data like interests & skills could potentially be scraped from job networks like LinkedIn (LinkedIn itself forbids scraping) but they usually don't provide information about job satisfaction. Perhaps it might still be of use to complete the full dataset.

## Acknowledgments

1. <a name="fn1"></a> [Building AI: AI Idea Gallery](https://buildingai.elementsofai.com/Conclusion/ai-idea-gallery)
2. <a name="fn2"></a> [Nearly half of global employees unhappy in jobs: Survey](https://www.cnbc.com/2013/09/17/nearly-half-of-the-worlds-employees-unhappy-in-their-jobs-survey.html)
