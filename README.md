This juypter notebook demonstrates how sentiment analysis can be used to evaluate opions about individual features of a product. For example, one might want to know how good (or bad) the battery or volume of a bluetooth speaker is. An naive approach would be to read multiple customer reviews. However, this can be exhausting, since there might be a lot of reviews for that product, from which only a small portion contain information about the relevant feature. Hence, it would be beneficial to get these information in a more compressed and easy to understand form.  

To overcome this issue, a sentiment analysis model is trained with Amazon reviews data. This model, a Long-Short-Term-Memory (LSTM) neural network, is then used to compute sentiment scores from multiple reviews that contain opinions about certain product features . The single scores are then aggregated and expressed as a distribution or e.g. single metric (mean).  

The steps involve:  
1. Create a dataset from Amazon reviews  
2. Clean and pre-process the raw text data  
3. Train a LSTM with TensorFlow using Keras API  
4. Extract the top product features  
5. Use the sentiment model to predict and aggregrate customer's opinions about the product features  


The saved weights and tokenizer can be downloaded from dropbox:  
https://www.dropbox.com/sh/dd597epuxffhfxz/AAB7SsNhLGagVB9wk2XbcMWra?dl=0

Note: Sometimes github fails to load/render juypter notebooks. In this case you can copy-paste the link from the notebook into https://nbviewer.jupyter.org/ or just click the link below:  
https://nbviewer.jupyter.org/github/jj-curious/SentimentAMZN/blob/master/SentimentReviews.ipynb
