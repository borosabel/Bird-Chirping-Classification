# Bird-Chirping-Classification
**Bird Chirping Classification from Audio Signal**

![img.png](img.png)

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

### **The detailed report of this part can be found at: [Data_Exploration.pdf](Exploration%2FData_Exploration.pdf)**

## 2. Data Classification:

See task description:

1. **Preprocess Data**: Convert audio fragments into a suitable format for machine learning, like Mel Spectrograms or MFCCs.
2. **Feature Extraction**: Extract relevant features from the audio data that will be used for classification.
3. **Model Training**: Train each selected model on the training data using various parameter settings.
4. **Model Evaluation**: Use cross-validation to evaluate each model and parameter setting, using your chosen metric(s).
5. **Analysis**: Compare the models and parameter settings, analyze the impact of parameters on overfitting and performance.

### **The detailed report of this part can be found at: [Classification.pdf](Classification%2FClassification.pdf)**

## 3. Challenge:

We got a test set of additional recordings, including the same set of
audio features that was available for training, but excluding the labels. Our task is to provide a label for the samples from the unknown test set. 
As the evaluation will differ a bit from what you used during your previous experiments, there are opportunities to tune your
system to maximize your evaluation score. 
You may try different solutions on the test
set by submitting your predictions to a challenge server that will run the evaluation.
You will document not only the final solution, but also the process of getting there.

### **The detailed report of this part can be found at: [Challenge.pdf](Challenge%2FChallenge.pdf)**