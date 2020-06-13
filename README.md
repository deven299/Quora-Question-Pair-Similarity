# QuoraQuestionPairSimilarity
Identify which questions asked on Quora are duplicates of questions that have already been asked.

### What is Quora? 
- Quora is a place to gain and share knowledge. It's a platform to ask questions and connect with people who contribute unique insights and quality answers.
- Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

Credit > Kaggle

### Problem Statement:
- Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question.
- So the challenge here is to build a model that identifies which questions asked on QUora are duplicates of the questions already asked.

### Objectives and Constraints:
- Misclassification cost is very high.
- No low-latency constraints.
- Result should be partially interpretable.

### Data Overview:
- The dataset is taken from Kaggle. [Link](https://www.kaggle.com/c/quora-question-pairs)
- The dataset contains 5 columns: qid1, qid2, question1,question2, is_duplicate

### Posing the real-world problem as a ML problem:
- Type of Machine Learning problem: 
      It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate(=1) or not(=0).
- Performance Metrics:
      1. Log Loss.
      2. Binary Confusion Matrix. 
