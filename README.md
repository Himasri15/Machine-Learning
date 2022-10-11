# Car-Eval-using-Naive-Bayes

=>The model evaluates cars according to the following concept structure:

   buying             buying products
   maint              price of the maintenance
   doors              number of doors
   persons            capacity in terms of persons to carry
   lug_boot           the size of luggage boot
   safety              estimated safety of the car
   
=>The Car Evaluation Database contains  

->Attributes: buying, maint, doors, persons, lug_boot, safety.
  
->Number of Instances: 1728
   
->Number of Attributes: 6

->Attribute Values:
   buying       v-high, high, med, low
   maint        v-high, high, med, low
   doors        2, 3, 4, 5-more
   persons      2, 4, more
   lug_boot     small, med, big
   safety       low, med, high
 
=> PART 1
->Implimented a naïve Bayes Classifier
accuracy on data:
accuracy(in%) : 62.28070175438597

=> PART 2
-> k-fold cross validation
Applied cross validation using KFold
Output:
[0.71098266 0.69942197 0.61849711 0.6416185  0.63583815 0.69942197
 0.63583815 0.68023256 0.68604651 0.61627907]
0.6624176636644711

=> PART 3
->Confusion matrix
Applied confusion matrix on train and test datasets
output:
confusion Matrix is:
[[ 18   0  38  66]
 [  4   0   4   8]
 [ 10   0 321  85]
 [  0   0   0  16]]
 
 ->By using confusion matrix got Precision,recall,F1-Score,Macro,weighted F1
 ->By using classification_report we got
                precision    recall  f1-score   support

         acc       0.18      0.04      0.06        79
        good       0.00      0.00      0.00        15
       unacc       0.72      0.76      0.74       217
       vgood       0.21      1.00      0.35        16

    accuracy                           0.56       327
   macro avg       0.28      0.45      0.29       327
weighted avg       0.53      0.56      0.52       327
 
 
 -> So based on output
 On independent variables buying, maint, doors, persons, lug_boot and safety and dependent variable class after completing predictions by using confusion metric on each class value we can understand that unacc got 74%, vgood got 35%, acc got 8% and good got 0.So based on output we cannot recommend the cars.
 
 
 
