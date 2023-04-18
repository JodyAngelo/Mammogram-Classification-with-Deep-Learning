# Mammogram-Classification-with-Deep-Learning</br>

Retrieved the public data set from the UCI repository https://archive.ics.uci.edu/ml/datasets/Mammographic+Mass </br>
This data contains 961 instances of masses detected in mammograms, and contains the following attributes: </br>

BI-RADS assessment: 1 to 5 (ordinal) </br>
Age: patient's age in years (integer) </br>
Shape: mass shape: round=1 oval=2 lobular=3 irregular=4 (nominal) </br>
Margin: mass margin: circumscribed=1 microlobulated=2 obscured=3 ill-defined=4 spiculated=5 (nominal) </br>
Density: mass density high=1 iso=2 low=3 fat-containing=4 (ordinal) </br>
Severity: benign=0 or malignant=1 (binominal) </br>
BI-RADS is an assesment of how confident the severity classification is; it is not a "predictive" attribute and so we will discard it. The age, shape, margin, and </br>
density attributes are the features that we will build our model with, and "severity" is the classification we will attempt to predict based on those attributes. </br>

Although "shape" and "margin" are nominal data types, which sklearn typically doesn't deal with well, they are close enough to ordinal that we shouldn't just discard 
them. The "shape" for example is ordered increasingly from round to irregular.</br>

A lot of unnecessary anguish and surgery arises from false positives arising from mammogram results. If we can build a better way to interpret them through building a Multi-Layer Perceptron and train it to classify masses, it could improve a lot of lives.</br>
