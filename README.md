# Repository for WMT 2023 Quality Estimation Shared Task

Link to task website: [https://wmt-qe-task.github.io/](https://wmt-qe-task.github.io/)

New training, dev and test data for the 2023 Quality Estimation Shared Task will be uploaded here.


## Data structure

### Task 1

The tsv files uploaded contain the following tab-separated information:

- index: segment index
- original: source segment
- translation: target translation segment
- scores: DA scores given by each annotation in 0-100 range
- mean: mean score value computed over the scores in the previous column
- z_scores: standardised scores (standardisation computed for each annotator separately)
- z_mean: mean score value computed over the z-scores in the previous column: this is the main target score for the 2023 QE shared task

