## data/

The data directory. For now, we will not include raw College Scorecard data.
The purpose is to set up the structure so that it's the same across our
local repos.

To download the College Scorecard data.
```
# in data/
$ wget 'https://s3.amazonaws.com/ed-college-choice-public/CollegeScorecard_Raw_Data.zip'

# unzip to current dir
$ unzip -j CollegeScorecard_Raw_Data.zip
```

Data files have the following format: `MERGED<yyyy>_PP.csv`.
Data is available from 1996 to 2013, inclusive.
