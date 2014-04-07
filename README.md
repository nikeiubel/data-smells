Data Smells (Work in Progress)
===========

Steps in verifying datasets:

1. Verify dataset source, do some reporting
1.1 Institution publishing data may have a poor track record. Example: Air quality in China
1.2 Even if not, data might still be problematic. Use common sense! Don't be tempted by the sensational headline! Example: rape statistics in Brazil
1.3 Problematic data entries vs. problematic dataset

2. Clean up dirt \n
2.1 categorization tables will allow you to see flaws in data (example: genders that are not 'M' or 'F') \n
2.2 simple statistics: max, min, quantiles, thresholds \n
2.3 simple random spot checks: verify randow rows and check that they're probably formatted \n

3. Then run more deep analysis
3.1 Benford's Law
3.2 deep random spot checks: verify each data entry

4. Compare it against other datasets


5. Go ahead and write the story
