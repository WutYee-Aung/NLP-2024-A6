# NLP-2024-A6

# Student Information

Name : Wut Yee Aung - st124377

# Model Comparison and Analysis

| Student Layer | Training Loss | Validation Loss | Validation Accuracy |
|---------------|---------------|-----------------|---------------------|
|Top-K Layer    |0.2767         |0.9077           |0.5800               |
|Bottom-K Layer |0.4476         |1.0835           |0.3600               |
|Odd Layer      |0.4080         |1.0879           |0.3000               |
|Even Layer     |0.7188         |1.1147           |0.3400               |


| Teacher Model                 | Training Loss | Validation Loss | Validation Accuracy |
|-------------------------------|---------------|-----------------|---------------------|
|BertForSequenceClassification  | 0.0856        | 1.4365          | 0.6700              |


According to the training loss, Top-K layer gets the minimum training loss and validation loss but get the maximum value in validation accuracy. Among the remaining three layer types, Even Layer type got the highest training loss. In conclusion, initial layer selection has impact on training part but not much difference in validation loss and validation accuracy.

With my current resources, it took around 17 hours to train 1 selected student layer with 100,000 sample size. So that I have reduced the sample size into 1,000. It is required high performance resources for large size of training data to get high performance model.
