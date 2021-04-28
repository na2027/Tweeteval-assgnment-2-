# TweetEval
This is the repository for the [_TweetEval_ benchmark (Findings of EMNLP 2020)](https://arxiv.org/pdf/2010.12421.pdf). _TweetEval_ consists of three heterogenous tasks in Twitter, all framed as multi-class tweet classification. All tasks have been unified into the same benchmark, with each dataset presented in the same format and with fixed training, validation and test splits.

# TweetEval: The Benchmark

These are the three datasets of TweetEval (irony, hate, offensive), with its corresponding labels (more details about the format in the [datasets](https://github.com/na2027/Tweeteval-assignment-2) directory):

- **Irony Detection**, [SemEval 2018 (Irony Detection)](https://www.aclweb.org/anthology/S18-1005.pdf) - 2 labels: `irony`, `not irony`

- **Hate Speech Detection**, [SemEval 2019 (Hateval)](https://www.aclweb.org/anthology/S19-2007.pdf) - 2 labels: `hateful`, `not hateful`
  
- **Offensive Language Identification**, [SemEval 2019 (OffensEval)](https://www.aclweb.org/anthology/S19-2010/) - 2 labels: `offensive`, `not offensive`

#The main Model Building file is
https://github.com/na2027/Tweeteval-assignment-2/blob/main/TweetEval_project%20(2).ipynb

This is used to build or train the DataSets - Irony, Offensive and Hate.


# Evaluating your system

For evaluating your system, Build an individual predictions file for each of the tasks. The format of the predictions file is same as the output examples in the predictions folder (one output label per line as per the original test file). I have used the RoBERTa re-trained on Twitter (RoB-Rt in the paper).  

The Evaluation file find at location
https://github.com/na2027/Tweeteval-assignment-2/blob/main/Evaluation_Model.ipynb


Three optional arguments can be modified in the Evaluation File: 

*--tweeteval_path*: Path to TweetEval datasets. Default: *"./datasets/"*

*--predictions_path*: Path to predictions directory. Default: *"./predictions/"*

*--task*: Use this to get single task detailed results *(emoji|emotion|hate|irony|offensive|sentiment|stance)*. Default: ""






