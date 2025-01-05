# Gen AI Pipeline 

## 1. Data Acquisition

1. **Available Data**: Data in formats such as `.csv`, `.txt`, etc.
2. **Other Data Sources**: Databases, internet, APIs, etc.
3. **No Data (Create Your Own Data)**:
   - **Generate with LLM**: Use a language model to create synthetic data. Options include:
     1. **Data Augmentation**: Artificially increase dataset size by creating modified versions of existing data.
        - Example: Add synonyms for major keywords.
     2. **Image Augmentation**: Apply transformations such as horizontal flip, brightness adjustment, noise addition, etc.
     3. **Bigram Flip**: Rearrange text to create new data.
        - Example: "I am Raj" -> "Raj is my name".
     4. **Back Translation**: Translate a sentence into another language (e.g., English -> Bengali -> Spanish -> English).
     5. **Add Additional Data/Noise**: Create variations.
        - Example: "I am Raj" -> "I am Raj, I am a boy".

## 2. Data Preprocessing

### 2.1 Cleanup
- Process of removing HTML tags, emojis, and correct spelling errors.

### 2.2 Basic Preprocessing
1. **Tokenization**:
   - Sentence-level tokenization.
   - Word-level tokenization.
2. **Optional Steps**:
   - Stop word removal.
   - Stemming: Convert words with the same root meaning into a single form.
   - Lemmatization: More commonly used, reduces words to their base form.
   - Punctuation removal.
   - Lowercase conversion.
   - Language detection.

### 2.3 Advanced Preprocessing
1. **Part-of-Speech Tagging**: Assign grammatical roles like verbs, nouns, etc., to tokens.
2. **Parsing**: Create a tree structure to represent tokenized sentences.
3. **Coreference Resolution**: Identify relationships between pronouns and their references.
   - Example: In "Chaplin is a boy. His father is in the army," link "Chaplin" and "his".

## 3. Feature Engineering

- **Text Vectorization Techniques**:
  - TF-IDF (Term Frequency-Inverse Document Frequency).
  - Bag of Words.
  - One-hot Encoding.
  - Transformer-based models.
  - Word2Vec.

## 4. Modelling

- Choose appropriate models: Open-source LLMs or paid models.

## 5. Evaluation

- **Intrinsic Evaluation**:
  - Use metrics like F1 score.
  - Typically performed by Gen AI engineers.
- **Extrinsic Evaluation**:
  - Conducted post-deployment.
  - Gather user feedback to assess real-world performance.

## 6. Deployment

- **Monitoring**: Ensure model performs as expected in production.
- **Retraining**: Update the model periodically with new data or feedback.

## 7. Monitoring and Model Updating

- Continuously track model performance.
- Incorporate new data for improvements.

---

## Common Terms

- **Corpus**: The entire text collection.
- **Vocabulary**: The set of unique words in a corpus.
- **Documents**: Individual rows or lines of text.
- **Word**: A single token in the text.

