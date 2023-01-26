# pandas_challenge

This assignement requires the use of Panda DataFrames to analyze school and standardized test data.

## Prep Work

Before you start:

* Create a new repository (e.g.- one that did not previously exist) for this project called `pandas_challenge`.

* Clone the new repository to your computer.

* Inside your local git repository, create a directory called **`PyCitySchools`**.

* Add your Jupyter Notebook to this folder.

* Push these changes to GitHub.

* Download the following files to get started:
https://static.bc-edx.com/data/dl-1-2/m4/lms/starter/Starter_Code.zip

## District Summary

Perform the necessary calculations and create a DataFrame showing the following:

* Total number of unique schools

* Total students

* Total budget

* Average math score

* Average reading score

* % passing math (the percentage of students who passed math)

* % passing reading (the percentage of students who passed reading)

* % overall passing (the percentage of students who passed math AND reading)

  ```Text
	Total Schools	Total Students	Total Budget	Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing
	   15	    	 39,170	   	$24,649,428.00	    78.985371	             81.87784	        74.980853	      85.805463	        65.172326
  ```

## School Summary

Perform the necessary calculations and create a DataFrame showing the following:

* School name

* School type

* Total students

* Total school budget

* Per student budget

* Average math score

* Average reading score

* % passing math (the percentage of students who passed math)

* % passing reading (the percentage of students who passed reading)

* % overall passing (the percentage of students who passed math AND reading)

```Text
	School            Type	 Total Students	TotalSchoolBudget PerStudentBudget  Ave.Math Score Ave.Reading Score % Passing Math % Passing Reading % Overall Passing
Bailey High School	District	4976	$3,124,928.00	   $628.00		77.048432	81.033963	66.680064	81.933280	54.642283
Cabrera High School	Charter		1858	$1,081,356.00	   $582.00		83.061895	83.975780	94.133477	97.039828	91.334769
Figueroa High School	District	2949	$1,884,411.00	   $639.00		76.711767	81.158020	65.988471	80.739234	53.204476
Ford High School	District	2739	$1,763,916.00	   $644.00		77.102592	80.746258	68.309602	79.299014	54.289887
Griffin High School	Charter		1468	$917,500.00	   $625.00		83.351499	83.816757	93.392371	97.138965	90.599455
Hernandez High School	District	4635	$3,022,020.00	   $652.00		77.289752	80.934412	66.752967	80.862999	53.527508
Holden High School	Charter		427	$248,087.00	   $581.00		83.803279	83.814988	92.505855	96.252927	89.227166
Huang High School	District	2917	$1,910,635.00	   $655.00		76.629414	81.182722	65.683922	81.316421	53.513884
Johnson High School	District	4761	$3,094,650.00	   $650.00		77.072464	80.966394	66.057551	81.222432	53.539172
Pena High School	Charter		962	$585,858.00	   $609.00		83.839917	84.044699	94.594595	95.945946	90.540541
Rodriguez High School	District	3999	$2,547,363.00	   $637.00		76.842711	80.744686	66.366592	80.220055	52.988247
Shelton High School	Charter		1761	$1,056,600.00	   $600.00		83.359455	83.725724	93.867121	95.854628	89.892107
Thomas High School	Charter		1635	$1,043,130.00	   $638.00		83.418349	83.848930	93.272171	97.308869	90.948012
Wilson High School	Charter		2283	$1,319,574.00	   $578.00		83.274201	83.989488	93.867718	96.539641	90.582567
Wright High School	Charter		1800	$1,049,400.00	   $583.00		83.682222	83.955000	93.333333	96.611111	90.333333
```

## Highest-Performing Schools (by % Overall Passing)

Sort the schools by `% Overall Passing` in descending order and display the top 5 rows.
Save the results in a DataFrame called "top_schools".

```Text
	School 	    Type  Total Students TotalSchoolBudget PerStudentBudget Average Math Score Average Reading Score % Passing Math % Passing Reading % Overall Passing
Cabrera High School Charter	1858	$1,081,356.00		$582.00		83.061895	  83.975780	 	94.133477	97.039828	91.334769
Thomas High School  Charter	1635	$1,043,130.00		$638.00		83.418349	  83.848930		93.272171	97.308869	90.948012
Griffin High School Charter	1468	$917,500.00		$625.00		83.351499	  83.816757	 	93.392371	97.138965	90.599455
Wilson High School  Charter	2283	$1,319,574.00		$578.00		83.274201	  83.989488	 	93.867718	96.539641	90.582567
Pena High School    Charter	962	$585,858.00		$609.00		83.839917	  84.044699	 	94.594595	95.945946	90.540541
```


## Lowest-Performing Schools (by % Overall Passing)
 
Sort the schools by `% Overall Passing` in ascending order and display the top 5 rows.
Save the results in a DataFrame called "bottom_schools".

```Text
School 	         Type Total Students Total School Budget Per Student Budget Average Math Score Average Reading Score % Passing Math % Passing Reading % Overall Passing
Rodriguez High School District	3999	$2,547,363.00	      $637.00			76.842711	80.744686	66.366592	80.220055	52.988247
Figueroa High School  District	2949	$1,884,411.00	      $639.00			76.711767	81.158020	65.988471	80.739234	53.204476
Huang High School     District	2917	$1,910,635.00	      $655.00			76.629414	81.182722	65.683922	81.316421	53.513884
Hernandez High School District	4635	$3,022,020.00	      $652.00			77.289752	80.934412	66.752967	80.862999	53.527508
Johnson High School   District	4761	$3,094,650.00	      $650.00			77.072464	80.966394	66.057551	81.222432	53.539172
```


## Math Scores by Grade

Perform the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.
	
	*Please note: The starter code contained an error for 11th grade and the below numbers for that column are not the results that should be displayed in your Jupyter Notebook
	
```Text
			   9th		  10th		  11th		  12th
Bailey High School	77.083676	76.996772	80.575873	76.492218
Cabrera High School	83.094697	83.154506	80.575873	83.277487
Figueroa High School	76.403037	76.539974	80.575873	77.151369
Ford High School	77.361345	77.672316	80.575873	76.179963
Griffin High School	82.044010	84.229064	80.575873	83.356164
Hernandez High School	77.438495	77.337408	80.575873	77.186567
Holden High School	83.787402	83.429825	80.575873	82.855422
Huang High School	77.027251	75.908735	80.575873	77.225641
Johnson High School	77.187857	76.691117	80.575873	76.863248
Pena High School	83.625455	83.372000	80.575873	84.121547
Rodriguez High School	76.859966	76.612500	80.575873	77.690748
Shelton High School	83.420755	82.917411	80.575873	83.778976
Thomas High School	83.590022	83.087886	80.575873	83.497041
Wilson High School	83.085578	83.724422	80.575873	83.035794
Wright High School	83.264706	84.010288	80.575873	83.644986
```


## Reading Scores by Grade

Create a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.
	
	*Please note: The starter code contained an error for 11th grade and the below numbers for that column are not the results that should be displayed in your Jupyter Notebook
	
```Text
			  9th		  10th		  11th		  12th
Bailey High School	81.303155	80.907183	82.559485	80.912451
Cabrera High School	83.676136	84.253219	82.559485	84.287958
Figueroa High School	81.198598	81.408912	82.559485	81.384863
Ford High School	80.632653	81.262712	82.559485	80.662338
Griffin High School	83.369193	83.706897	82.559485	84.013699
Hernandez High School	80.866860	80.660147	82.559485	80.857143
Holden High School	83.677165	83.324561	82.559485	84.698795
Huang High School	81.290284	81.512386	82.559485	80.305983
Johnson High School	81.260714	80.773431	82.559485	81.227564
Pena High School	83.807273	83.612000	82.559485	84.591160
Rodriguez High School	80.993127	80.629808	82.559485	80.376426
Shelton High School	84.122642	83.441964	82.559485	82.781671
Thomas High School	83.728850	84.254157	82.559485	83.831361
Wilson High School	83.939778	84.021452	82.559485	84.317673
Wright High School	83.833333	83.812757	82.559485	84.073171
```



## Scores by School Spending

Create a table that breaks down school performance based on average spending ranges (per student).
Use the code provided below to create four bins with reasonable cutoff values to group school spending:


  ```text
spending_bins = [0, 585, 630, 645, 680]
labels = ["<$585", "$585-630", "$630-645", "$645-680"]
  ```
  
  
Use `pd.cut` to categorize spending based on the bins.
Use the following code to then calculate mean scores per spending range:

  ```text
spending_math_scores = school_spending_df.groupby(["Spending Ranges (Per Student)"]).mean()["Average Math Score"]
spending_reading_scores = school_spending_df.groupby(["Spending Ranges (Per Student)"]).mean()["Average Reading Score"]
spending_passing_math = school_spending_df.groupby(["Spending Ranges (Per Student)"]).mean()["% Passing Math"]
spending_passing_reading = school_spending_df.groupby(["Spending Ranges (Per Student)"]).mean()["% Passing Reading"]
overall_passing_spending = school_spending_df.groupby(["Spending Ranges (Per Student)"]).mean()["% Overall Passing"]
 ```
Use the scores above to create a DataFrame called `spending_summary`.
Include the following metrics in the table:

* Average math score

* Average reading score

* % passing math (the percentage of students who passed math)

* % passing reading (the percentage of students who passed reading)

* % overall passing (the percentage of students who passed math AND reading)


```Text
		   Average Math Score	Average Reading Score	% Passing Math	% Passing Reading   % Overall Passing
Spending Ranges (Per Student)					
	<$585		83.455399	   83.933814		   93.460096	   96.610877		90.369459
	$585-630	81.899826	   83.155286		   87.133538	   92.718205		81.418596
	$630-645	78.518855	   81.624473	   	   73.484209	   84.391793		62.857656
	$645-680	76.997210	   81.027843		   66.164813	   81.133951		53.526855
```

## Scores by School Size

Use the following code to bin the `per_school_summary`:

  ```text
size_bins = [0, 1000, 2000, 5000]
labels = ["Small (<1000)", "Medium (1000-2000)", "Large (2000-5000)"]
  ```
  
Use `pd.cut` on the "Total Students" column of the `per_school_summary` DataFrame.
Create a DataFrame called `size_summary` that breaks down school performance based on school size (small, medium, or large).

```Text
		Average Math Score	Average Reading Score	% Passing Math	  % Passing Reading  % Overall Passing
School Size					
Small (<1000)		83.821598		83.929843	  93.550225	  	96.099437	89.883853
Medium (1000-2000)	83.374684		83.864438	  93.599695		96.790680	90.621535
Large (2000-5000)	77.746417		81.344493	  69.963361		82.766634	58.286003
```


## Scores by School Type

Use the `per_school_summary` DataFrame from the previous step to create a new DataFrame called `type_summary`.
This new DataFrame should show school performance based on the "School Type".


```Text
			Average Math Score	Average Reading Score	% Passing Math	% Passing Reading  % Overall Passing
School Type					
Charter				83.473852		83.896421	  93.620830	   96.586489	      90.432244
District			76.956733		80.966636	  66.548453	   80.799062	      53.672208
```


## Written Analysis

Present a written analysis that summarizes the data **AND** draw two conclusions or comparisons from the calculations. 




## Final Tips

* Commit your work and back it up with pushes to GitHub.
* Add a detailed `README.md` file to your repository.
* This `README.md` file contains the correct DataFrames that should appear from the script run in your Jupyter Notebook.


- - -
Data generated by Mockaroo, LLC Links to an external site., (2022). Realistic Data Generator. Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
