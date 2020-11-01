# Objective  
Develop a classification model to predict Parkinson’s disease using the given patient’s
biomedical voice measurements.  

# Context  
Parkinson’s Disease (PD) is a degenerative neurological disorder marked by
decreased dopamine levels in the brain. It manifests itself through a deterioration of
movement, including the presence of tremors and stiffness. There is commonly a
marked effect on speech, including dysarthria (difficulty articulating sounds),
hypophonia (lowered volume), and monotone (reduced pitch range). Additionally,
cognitive impairments and changes in mood can occur, and risk of dementia is
increased.
Traditional diagnosis of Parkinson’s Disease involves a clinician taking a neurological
history of the patient and observing motor skills in various situations. Since there is no
definitive laboratory test to diagnose PD, diagnosis is often difficult, particularly in the
early stages when motor effects are not yet severe. Monitoring progression of the
disease over time requires repeated clinic visits by the patient. An effective screening
process, particularly one that doesn’t require a clinic visit, would be beneficial. Since
PD patients exhibit characteristic vocal features, voice recordings are a useful and
non-invasive tool for diagnosis. If machine learning algorithms could be applied to a
voice recording dataset to accurately diagnosis PD, this would be an effective
screening step prior to an appointment with a clinician.

# Data Description  
The data & attributes information for this project is available
at https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/  
The data consists of those diagnosed with Parkinson Disease and those who do not.
Kindly use parkinsons.data file.  
This dataset is composed of a range of biomedical voice measurements from 31
people, 23 with Parkinson's disease (PD). Each column in the table is a particular voice
measure, and each row corresponds to one of 195 voice recordings from these
individuals ("name" column). The main aim of the data is to discriminate against
healthy people from those with PD, according to the "status" column which is set to 0
for health and 1 for PD.
The data is in ASCII CSV format. The rows of the CSV file contain an instance
corresponding to one voice recording. There are around six recordings per patient, the
name of the patient is identified in the first column.
name - ASCII subject name and recording number
MDVP:Fo(Hz) - Average vocal fundamental frequency
MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
MDVP:Flo(Hz) - Minimum vocal fundamental frequency
MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several
measures of variation in fundamental frequency
MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:
APQ,Shimmer:DDA - Several measures of variation in amplitude
NHR,HNR - Two measures of ratio of noise to tonal components in the
voice
status - Health status of the subject (one) - Parkinson's, (zero) - healthy
RPDE,D2 - Two nonlinear dynamical complexity measures
DFA - Signal fractal scaling exponent
spread1,spread2,PPE - Three nonlinear measures of fundamental
frequency variation  

# Steps and Milestones (100%):
1. Load the dataset
2. It is always a good practice to eye-ball raw data to get a feel of the data in terms
of number of structure of the file, number of attributes, types of attributes and a
general idea of likely challenges in the dataset. (2.5 points)  
3. Using univariate & bivariate analysis to check the individual attributes for their
basic statistics such as central values, spread, tails etc. What are your
observations? (15 points)
4. Split the dataset into training and test set in the ratio of 70:30 (Training:Test).
5. Create a decision tree model using “entropy” method of reducing the entropy and
fit it to training data. (5 points)
6. Test the model on test data and what is the accuracy achieved. Capture the
predicted values and do a crosstab. (7.5 points)
7. Use regularization parameters of max_depth, min_sample_leaf to recreate the
model. What is the impact on the model accuracy? How does regularization
help? (20 points)
8. Next implement the Random Forest model and find the accuracy (10 points)  

# Learning Outcomes:  
o Predictive Analytics  
o Ensemble Classifiers – Random Forests  
o Decision Tree Classifier  
o Fine-tuning Model with Grid Search  
o Data Preparation  
o Feature Engineering  
o Visualization  
