Data Smells (Work in Progress)
===========

Steps in verifying whether datasets are credible:

1. Verify dataset source, do some reporting
=
  1.1 Institution publishing data may have a poor track record. Example: Air quality in China

	1.2 Even if not, data might still look suspicious. Use common sense! Don't be tempted by the sensational headline. Example: rape statistics in Brazil
"Never mind - Poll that sparked Brazil's outrage was wrong"
http://uk.reuters.com/article/2014/04/04/uk-brazil-poll-clothing-idUKBREA331S920140404

	1.3 Problematic data entries vs. problematic dataset: Human error during manual data entry
	
	1.4 If suspicious, look at original data collection points, original datasets (JOINS might introduce errors, meanings of attributes might be different, data may have been parsed wrong)

2. Clean up dirt
=
	2.1 Check for 'missing data', 'inconsistent values', 'unresolved duplicates'

	2.2 Categorization of variables will allow you to see flaws in data (example: genders that are not 'M' or 'F')

  2.3 Simple statistics: max, min, mean, median, mode, quantiles, thresholds
  
  2.4 Simple random spot checks: verify randow rows and check that they're probably formatted
  
	2.5 Visual encodings: Histograms, Time Series (look for sharp/abrupt curves)
	The visualization chosen must also fit the semantics of the data. For example, an error in the encoding of geographic locations may not become apparent until plotted on a map.
	
	2.6 Extreme Outliers and Missing Data
But outliers may be valid data: Data from DC is different from data from every other state
"Outliers often stand out in a plot, sometimes reducing the visibility of other data points owing to an extreme scale. Similarly, missing data may surface as a promi- nent gap or zero value in the data."

	2.7 Duplicate or misspelled
	Duplicate or misspelled values may appear adjacent to one another in a sorted list/categorization of variable

"Although the ‘real’ analysis is just about to start (step 4), John has made dozens of transformations, repeated the process several times, made important discoveries relating to the quality of the data, and made many decisions impacting the quality of the final ‘clean’ data."
	
	2.8 
	choices of representation (e.g. matrix diagram) and parameterization (e.g. default sort order) are crit- ical to unearthing data quality issues.
example: facebook API

	2.9
	

3. Then run more deep analysis
=
	3.1 Benford's Law

	3.2 Deep random spot checks: verify each data entry
	
	3.3. Social media data? Be aware of bots!


4. Compare it against other datasets
=

List of Data Smells
- JOINS might introduce errors
- meanings of attributes might be different
- Some cells are blank as opposed to empty!
- Data looks suspicious
- Extreme outliers
- 

"Li et al.11 outline 41 different types of dirty data, and examine the costs of fixing these errors within different contexts. Kim et al.12 propose a taxon- omy of 33 dirty data types."


Mü̈ller and Freytag13 roughly classify data anomalies into syntactical, semantic, and coverage anomalies.
- Syntactical anomalies are errors in data format and values. 
- Semantic anomalies include inconsistencies within or across data sets (e.g. integrity constraint violations, contradictions, duplicates, and invalid tuples). 
- Coverage anomalies refer to missing or incomplete data.

5. Go ahead and write the story
=



