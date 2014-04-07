Data Smells (Work in Progress)
===========

Steps in verifying datasets:

1. Verify dataset source, do some reporting
- Institution publishing data may have a poor track record. Example: Air quality in China
- Even if not, data might still be problematic. Use common sense! Don't be tempted by the sensational headline! Example: rape statistics in Brazil
- Problematic data entries vs. problematic dataset

2. Clean up dirt
- categorization tables will allow you to see flaws in data (example: genders that are not 'M' or 'F')
- simple statistics: max, min, quantiles, thresholds
- simple random spot checks: verify randow rows and check that they're probably formatted

3. Then run more deep analysis
- Benford's Law
- deep random spot checks: verify each data entry

4. Compare it against other datasets


5. Go ahead and write the story
