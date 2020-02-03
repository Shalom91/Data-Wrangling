Instructions

This data contains personality scores for recruits, plus the department they applied for.

    Import the dataset personality_scores.csv. Examine the data frame for duplicates (based on ID), and drop any duplicates that exist. Use an assert statement to check that the new data frame is the length of the unique entries of the original data frame.

Tip: An example assert statement is assert 2*20=40 and it’s a great way to check that your modification of the data was successful.

    Create new columns containing the total score of each of the personality test subscales. To do this, write a function (or functions) that will calculate the total score for each of the subscales (conscientiousness, emotional stability, openness to new experience, agreeableness, extraversion), as set out in scoring. In other words, for the conscientiousness total score, all items marked as belonging to ‘conscientiousness’ should be summed.

The new data frame will look something like this:
I am always prepared 	I am easily disturbed 	I am exacting (demanding) in my work 	… 	Conscientiousness 	Emotional Stability
(3, 5) 	(4, 5) 	(3, 5) 	… 	10 	5
(3, 5) 	(4, 1) 	(3, 1) 	… 	6 	1
(3, 5) 	(4, 3) 	(3, 3) 	… 	8 	3

    Import the data in departments.csv. Merge this data frame with the personality score data frame, keeping all applicants within the department data frame. Use an assert statement to check that the newly created merged data frame has the same amount of rows as the department data frame, and the expected number of columns.

    Filter the merged data frame so that you get only the applicants who scored less than 30 on emotional stability, conscientiousness AND agreeableness. Print the ID numbers and departments of these applicants to the screen, and also assign these applicants the tag “high_risk” in a new column. All other applicants get the tag “low_risk”

    Create a new data frame with a count of the number of low and high risk applicants within each department. Let each department be a separate column. In other words, the data frame should look something like this:

Risk 	Multimedia 	Coding 	Data
Low risk 	150 	123 	239
High risk 	40 	15 	22
