# set-difference-spark-mapreduce
 a mapreduce program to solve set difference(R - S) using pyspark

pseudo-code: 


	•	The map function: for each t in R, produce a key-value pair (t, R), and for each t in S, produce a key-value pair (t, S).

 
	•	The reduce function: for each key t, if the associated value list is [R] but not in [S}, then produce (t, t), otherwise, produce nothing.

 
The input is two files, R.text and S.text, and both have an integer number per line, the same integers may appear multiple times in any document. 
