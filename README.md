# The CVPR 2021 Chart Question Answering Challenge

We designed the CQA challenge to test how different algorithms can generalize across graphical perception stimuli.

The challenge includes 3 levels: from low-level visualization building blocks to semantic reasoning that requires text extraction.

More information and datasets are available here: https://cqaw.github.io/challenge

## Data

We provide 3 datasets with increasing complexity. Each dataset includes training data with labels and testing data without labels.

Here is an example `TRAIN_metadata.csv` that includes the labels.
```
filename,level,classtype,query,label
LENGTH_train_0b0.png,1,length,What is the length of the line in the figure?,106
LENGTH_train_1b0.png,1,length,What is the length of the line in the figure?,160
...
```

And, here is a snippet from `TEST_metadata.csv` without the label.

```
filename,level,classtype,query
LENGTH_test_0b0.png,1,length,What is the length of the line in the figure?
LENGTH_test_1b0.png,1,length,What is the length of the line in the figure?
...
```

These two examples are from the low-level stimuli dataset. The questions vary per dataset.

## Submission

**Please submit your predictions via pull request to this repository (fork it first!).** Please create a folder for your team and include the name of the challenge in your filename (e.g. `TEAM_A/lev1_TEST_metadata.csv`). The submission should add a column to the test csv file that includes your predicted label.

We will evaluate your predictions and update the leaderboard accordingly.

## Data Generation
 
Here is the code for the stimuli generation: https://github.com/LE-V-EL/cqaw_datagenerator

You do not need this code - instead please download the generated datasets here: https://cqaw.github.io/challenge

## Questions?

Please contact cqaw < at > mpsych . org ! 
