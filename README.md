# spectrum_intern_finaltask
Final task of Spectrum ML internship

# PROJECT REPORT:

The goal of this project was to find out any relation
between the grades of a student and various aspects of his/her
student life.

I started by taking into consideration all the features
present in the corresponding dataset. Then I started using backward
elimination with the help of statsmodels api and started chopping of 
the features which seemed to be irrelevent, as suggested by their 'p'
values with a tolerence limit of 5%. After several rounds of elimination,
I ended up with six features, namely age, activities, family-relations, 
absences and the previous grades of the students(G1 and G2). I got an accuracy
score of 0.9775.

Out of these features, by far the most useful were the 
previous grades, as expected. The ages of the students also have a notable
significance on their performance. I found the average grade of a 15-16 
year old to be 33, that of a 17 year old to be 31, of an 18 year old to be 30
and of a 19 year old to be 27. I observed that the younger you are, the more likely
you are to get high grades. The average grade of 20 year olds is 40 but as there are
only 3 of them, we can consider them outliers.

The other features picked by the algorithm, like family relations and extra-
curricular activities didn't seemed to influence the grades hugely. Another interesting
finding is that for the 115 students who attended school everyday without any absences,
the average grade is 28, while for the 17 students who had exactly 10 days of absence, 
the average is 31. This may be an indication that attending classes regularly doesn't 
guarantee you high grades.

An interesting feature the algorithm failed to pick up is the parents occupation.
The average grade of a student whose father is teacher is 34, whose mother is teacher is 32.
If none of the parent is a teacher, this number falls down to 31, and if both the parents are 
teacher, the average grade is 40.


