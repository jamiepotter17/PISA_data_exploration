# PISA 2012 Data Exploration

To view the slide presentation, go to [https://jamiepotter17.github.io/PISA_data_exploration/](https://jamiepotter17.github.io/PISA_data_exploration/)

## Dataset

The data are from the 2012 round of the Programme for International Student
Assessment (PISA), a triennial international education survey organised by the
Organisation for Economic Co-operation and Development (OECD). The aim is to
provide meaningful international comparisons for the educational attainment of
15-16 year olds for participant nations.

Alongside a general questionnaire that quizzed pupils on various aspects of
school life and life at home, pupils take a two hour computer-based test.
Scores are then scaled so that the average in each of the three areas tested
(mathematics, reading, science) have mean 500, standard deviation 100.
Typically, the object of most media interest is the ranking that appears at the
end, where countries are ranked in terms of their mean scores. The 2012 survey
also included a section on problem-solving.

The dataset was downloaded on 06/11/2021 from Udacity's server [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip).

## Summary of Findings

In the exploration, I found that many things were associated with increased
student scores in fairly predictable ways - lower truancy rates, higher parental
education level, having one's own room, having a desk, the number of computers,
TVs, mobile phones, and books in the household. I found a small possible effect
of the sex of the student and mathematics score (with males slightly higher),
and a slightly larger possible effect in reading (with females higher). This was
the only occasion in which the three response variables differed in an
interesting way; the rest of the time, they were tightly intercorrelated. I
failed to find anything to do with perseverance or openness to problem-solving,
or something involving age.

I found a couple of interactions which I thought were interesting - firstly,
I found that wealth interacted with the highest education level achieved by the
pupils' parents. At higher wealth levels, the more parental education, the
better. But at lower wealth levels, the best performing pupils had parents with
a vocational/secondary education level. Secondly, the sex of the student
interacted with household wealth levels. Female scores in Mathematics and
Science increase 13% faster than they do for males as wealth level increases,
indicating an interaction between sex and wealth. But this effect is especially
pronounced in reading, where they female scores increase 22% faster than males
scores as wealth level increases.

## Key Insights for Presentation

For the presentation, I focus on the elements leading up to the two
interactions - sex and wealth. I omit age, truancy, perseverance, and openness
to problem-solving entirely. I include the possessions data simply to underline
the point that wealth matters, and because I think it's also interesting that
the number of books in the household does not have a special relationship with
reading.

The key insights are structured as follows:

1. Possessions are an indicator of household wealth. In general, the more
possession you have, the wealthier you are, and the higher your score in the
PISA test.
2. Books aren't special. The number of books in your household has no
discernible effect specifically on reading beyond being a general indicator of
wealth.
3. Household wealth interacts with parental education levels. At higher wealth
levels, pupils with parents having the highest education levels scored the best.
At lower wealth levels, pupils with the highest average test scores come from
households where the highest parental education levels are secondary/vocational.
4. Males tend to have slightly higher mathematics scores than females, but
females have higher reading scores than males.
5. Sex interacts with wealth, especially for reading scores. As wealth level
increases, female reading scores improve faster than male scores.

The first interaction comes at 3. and concerns the interaction between
household wealth and the highest education level of the students' parents. Once
that has been addressed, I then talk about the effect of the sex of the pupil,
and that leads into the second interaction at 5. concerning sex and wealth.

One thing I tried to do throughout the various plots I used was stick to a
consistent colour scheme - orange for mathematics scores, green for reading, and
purple for science, with other plots not using these specific colours.
