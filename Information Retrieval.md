
## 2. Text Processing

Information Retrieval Definition:

Tokenization: 

Tokenization: segmenting text into tokens  
- Token: a sequence of characters  
- Type: class of all tokens with the same character sequence  
- Term: a (normalized) type that is included in the IR dictionary  

Terms are usually derived from tokens by various normalization process such as:  
- case-folding (reducing all letters to lowercase)  
- stemming, lemmatization  
- stopword removal  etc

Training  
1. Pre-tokenization  
2. Compute consecutive character-pair frequencies  
3. Merge the most frequent pair  
4. Recalculate character-pair frequencies  
5. Repeat 3, 4 until vocab size V is reached  

Tokenizing  
1. Pre-tokenization  
2. Get individual chars; replace chars not in training vocab with UNK  
3. Iterate over chars  
4. Iterate over merge rules and apply first applicable  
5. Repeat 4 until 3 is complete