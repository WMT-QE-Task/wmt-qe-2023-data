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

### Task 2

The tsv files uploaded contain the following tab-separated information:

- mt_model: identifier of translation model
- doc_id: id of the document
- seg_id: id of segment
- annotator_id: id of annotator
- source: source segment
- target: target translation segment
- error start id: indices of beginning of error spans (character based) separated by a single whitespace for the case of mutliple error spans. -1 indicates no error spans present in the segment.
- error start id: indices of the end of error spans (character based) separated by a single whitespace for the case of mutliple error spans. -1 indicates no error spans present in the segment.
- error type: indication of *minor* or *major* error for each detected error span. The number of indices should match the number of errors. If there is no error span in a segment indicate with *no-error*.