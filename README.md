# Bird-Chirping-Classification
**Bird Chirping Classification from Audio Signal**

**Disclaimer:** This is a university group project's final report.
For a detailed project specification, look up the [Machine Learning & Pattern Classification Moodle page](https://www.jku.at/en/institute-of-computational-perception/teaching/alle-lehrveranstaltungen/machine-learning-and-pattern-classification-vl-ue/).

### Group Members

| Student ID | First Name    | Last Name |
|------------|---------------|-----------|
| k12141871  | Luiz-Henrique | Madjarof  |
| K11944603  | Abel          | Boros     |

### Goal of the Project

Our overall goal for this year’s project is to train a system that can tell, for any instant in
an audio recording, which bird species is audible (if any). Turning this into a machine
learning problem entails:
1. splitting up the audio into small fragments (“frames”), which will become the
   training examples,
2. computing a set of audio features for each frame,
3. assigning a label to each frame,
4. training a classifier to predict the label from the audio features.

The workload was split into three phases:

## 1. Data Annotation & Data Exploration:

**Data Annotation:**

In this part the whole university class had to annotate bird sounds (part where it's audible and parts where we have silence.)
Every Audio file was annotated by 6 person separately.

**Data Exploration:**

After the annotation we finally had a dataset of 120.000 labeled audio fragments along with audio features (provided by university personell.)
During the Data exploration we had to report:

1. **Annotator agreement**: How consistent are the annotations? Do different annotators agree in their labels for the same fragment?
2. **Label characteristics**: How are the class labels distributed? Are the classes unbalanced, and how much? What is the average duration of a species’ calls (or
   drumming)? Are there large inter-/intra-class variations?
3. **Feature characteristics**: How are the features distributed? Are there any pairs or
   subsets of features that seem highly correlated or redundant?
4. **Feature/Label agreement**: Which features seem useful for classification? Which
   ones are correlated with the labels?
5. **Consequences**: Any conclusions you can draw from your analysis for doing classification?

The detaild report of this part can be found at: [Data_Exploration.pdf](Exploration%2FData_Exploration.pdf)