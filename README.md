# D209 Classification-with-KNN
Analysis of hospital data using KNN


## Research Question
Decision trees will be used for this analysis of the medical data set to determine which features indicate whether a patient is likely to be readmitted after the initial visit.  Also, I will look to see whether readmitted patients can be grouped by defined characteristics. 

## Goal
Readmitting patients into hospitals can be a costly endeavor.  The goal of this study is to identify which patients are likely to be readmitted and provide this ability to project stakeholders to better help them curve the trend of readmission.  

## Method Justification
The target variable, ‘ReAdmis’, and various features will be fed into the decision trees function. The decision trees function uses recursive partitioning to perform attribute-value testing and then splits the data into a flow chart which it uses to make grouped-based predictions (“Decis,” p.1). 

## Packages
  *  pandas
  *  numpy
  *  seaborn
  *  matplotlib
  *  sklearn.preprocessing - LabelEncoder
  *  sklearn.preprocessing - StandardScaler
  *  sklearn.neighbors - KNeighborsClassifier
  *  sklear.model_selection - train_test_split
  *  sklearn.metrics - accuracy_score
  *  sklearn.metrics - classification_report
  *  sklearn.metrics - confusion_matrix

## Initial Dataset
  * Hospital dataset
  * Data types of selected attributes
  * Rows:  9,999
  * Clolumns: 52
    
## Selected Attributes
  * <DT
        
## EDA
  *  <cp>  
  *  <heatmp>    pain
## Results 
  * K-value = 5
  * ** Mean Squared Error: ** 0.071  
  * Confusion matrix
 ![alt text](https://github.com/smithjs135/Classification-with-KNN/blob/main/CM.jpg "")
    
          <CM>
            <accuracy>
              <error_rate>
## Refinement
KNN requires an input variable called the “K” value.  I made an initial best guess of 5 as to the “K” value and received an accuracy value of 81%.  I then charted the error curves two different ways(Tarek Atwan, p.1). These charts provide clues to determine an ideal “K” value.  Screen shots of both error charts follow:
  * K-value = 15   
              <error_rate>
<CM2?              
## Accuracy
The model accuracy is 84% (0.836). The precision of predicting a patient being readmitted is 93%.  The precision of predicting a patient not being readmitted in 72%. The accuracy and precision score values indicate the model’s strong ability to prediction abilities. 
      
## Results  
K Nearest Neighbors was used to classify and predict which patients were likely to be readmitted. Features having the strongest correlation were selected. These features include: 'Initial_days', 'Population','Treatment','Doc_visits', 'VitD_levels'.  An optimal K-value was chosen based on charting out the error rate vs. K-values. The relatively high accuracy and precision of this model means hospital executives can predict which patients are likely to be readmitted into the hospital based on the above features.  
      
## Limitation
      KNN is quite sensitive to the scale of a dataset and can be thrown off quite easily by irrelevant features (Daniel Nelson, p. 1).  This model can be used as a focal point to target patients that possibly should be further interviewed and monitored for hospital readmittance. There is no guarantee that patients that are identified as likely to be readmitted will be readmitted.  
      
## Recommendation  
      Hospital executives and personnel can be trained to identify and assist those patients likely to be readmitted and / or identify those patients that are not likely to fully recover from their ailments. Hospital personnel can start to look for common patterns that lead to readmittance. Reducing readmittance, not only leads to hospital cost reduction, but also leads fewer patients checking in to the hospital, reduced suffering of the patients, and lower workloads and stress levels of the hospital staff. 
 
##  Sources for Third Party Code 
1.	Tarek Atwan(2017, P.1). How To Plot A Confusion Matrix In Python.
How To Plot A Confusion Matrix In Python – Tarek Atwan – Notes on Artificial Intelligence. https://tatwan.github.io/How-To-Plot-A-Confusion-Matrix-In-Python

2.	Bashir Alam(2022, P.1).  Implementing KNN Algorithm using Python. https://hands-on.cloud/implementing-knn-algorithm-using-python

##  Sources(in-line)

1.	Daniel Nelson. (2020, (P. 1)).  What is a KNN (K-Nearest Neighbors)?
https://www.unite.ai/what-is-k-nearest-neighbors/#:~:text=The%20main%20limitation%20when%20using%20KNN%20is%20that,algorithm%2C%20the%20proper%20value%20for%20K%20is%20chosen.

  
