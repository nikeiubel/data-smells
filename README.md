Data Smells (Work in Progress)
===========

Steps in verifying whether datasets are credible:

1. Verify dataset source, do some reporting
=
  1.1 Institution publishing data may have a poor track record. Example: Air quality in China

	1.2 Even if not, data might still look suspicious. Use common sense! Don't be tempted by the sensational headline. Example: rape statistics in Brazil
"Never mind - Poll that sparked Brazil's outrage was wrong"
http://uk.reuters.com/article/2014/04/04/uk-brazil-poll-clothing-idUKBREA331S920140404

	1.3 Problematic data entries vs. problematic dataset
	
	1.4 If suspicious, look at original data collection points, original datasets (JOINS might introduce errors, meanings of attributes might be different, data may have been parsed wrong)

2. Clean up dirt
=
	2.1 Check for 'missing data', 'inconsistent values', 'unresolved duplicates'

	2.2 Categorization of variables will allow you to see flaws in data (example: genders that are not 'M' or 'F')

  2.3 Simple statistics: max, min, mean, median, mode, quantiles
  
  2.4 Simple random spot checks: verify randow rows and check that they're probably formatted
  
	2.5 Visual encodings: Histograms, Time Series (look for sharp curves)
	
	2.6 Extreme Outliers, thresholds
But outliers may be valid data: Data from DC is different from data from every other state

"Although the ‘real’ analysis is just about to start (step 4), John has made dozens of transformations, repeated the process several times, made important discoveries relating to the quality of the data, and made many decisions impacting the quality of the final ‘clean’ data."

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




5. Go ahead and write the story
=
