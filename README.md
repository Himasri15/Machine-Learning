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
 
 
 
