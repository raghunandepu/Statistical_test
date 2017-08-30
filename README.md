# UD_MLFND_P2
Test a Perceptual Phenomenon

# Project 2: Test a Perceptual Phenomenon 
## Background information
In a Stroop task, participants are presented with a list of words, with each word displayed in a color of ink. The participant’s task is to say out loud the color of the ink in which the word is printed. The task has two conditions: a congruent words condition, and an incongruent words condition. In the congruent words condition, the words being displayed are color words whose names match the colors in which they are printed: for example RED, BLUE. In the incongruent words condition, the words displayed are color words whose names do not match the colors in which they are printed: for example PURPLE, ORANGE. In each case, we measure the time it takes to name the ink colors in equally-sized lists. Each participant will go through and record a time from each condition.

**Dataset:** <a href="https://github.com/raghunandepu/UD_MLFND_P2/blob/master/stroopdata.csv">View CSV</a>

## Questions for investigation

## 1. What is our independent variable? What is our dependent variable? 
 
Dependent variable: Time to name ink colours

Independent variable: Word Condition (congruent/incongruent)


## 2. What is an appropriate set of hypotheses for this task? What kind of statistical test do you expect to perform? Justify your choices.

#### Hypothesis test
Null Hypthesis **Ho**: Time to name colours is the same for congruent and incongruent tasks

Alternative Hypothesis **Ha**: Time to name colours is not the same for congruent and incongruent tasks

The Dependent Samples t-Test is the appropriate statistical test as the same subjects are assigned two different conditions. The different conditions are dependent because by doing the first test you have some practice doing it and you might have an unfair advantage due to this learning effect in doing the similar type of test second. In addition, we don't have any population parameters provided (so a z-test would not be appropriate here).

## 3. Report some descriptive statistics regarding this dataset. Include at least one measure of central tendency and at least one measure of variability.
#### Congruent
Mean: 14.0
Standard Deviation SD: 3.6
#### Incongruent
Mean: 22.0
Standard Deviation SD: 4.8

## 4. Provide one or two visualizations that show the distribution of the sample data. Write one or two sentences noting what you observe about the plot or plots.

![alt text](https://github.com/raghunandepu/UD_MLFND_P2/blob/master/Completion-plot.PNG)

**Observation:** Congruent word condition appear to be consistently completed faster than incongruent  word condition


## 5.What is your confidence level and your critical statistic value? Do you reject the null hypothesis or fail to reject it? Come to a conclusion in terms of the experiment task. Did the results match up with your expectations?

```
α = .01 
df = 23 
tcrit = -2.50 
t = -8.02 
P-value = < .0001 
```

At the 99% confidence level (α = .01) and 23 degrees of freedom, the critical statistic value for a one-tailed test in the negative direction is -2.5. The calculated t-statistic for the difference in colour recognition time means of the congruent and incongruent word data is -8.02. Since the t-statistic is in the critical region, the ***null hypothesis is rejected***. With the data presented, it is very unlikely that the 7.96 second difference in mean time for colour recognition for the congruent data vs. the incongruent data is obtained if the two means are actually the same (or if μC > μI). By conventional criteria, this difference is considered to be extremely statistically significant. 
There is sufficient evidence at the α = .01 level of significance to support the claim that it takes less time to recognize the colour of words with the congruent condition compared to words with the incongruent condition. The result confirms my expectations.

## 6. What do you think is responsible for the effects observed? Can you think of an alternative or similar task that would result in a similar effect? Some research about the problem will be helpful for thinking about these two questions!

The brain has an image association between the shape of the word and the colour. When there is a mismatch, additional time is necessary for the prefrontal cortex to process the information and decide on its meaning.
A similar effect would likely be observed if the participants were shown words of the correct colour but the wrong text.  However, the difference would be less pronounced as I’d expect the visual colour representation to be more ingrained in the brain that word shape associations.
