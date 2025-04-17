#Name: Jayadev Goskula(700757314)

# NLP Preprocessing Pipeline Observation

## Pipeline Components
✅ **Tokenization**: Splits text into individual words/punctuation  
✅ **Stopword Removal**: Filters out common English words (e.g., "the", "are")  
✅ **Stemming**: Reduces words to root form (e.g., "techniques" → "techniqu")

## Sample Output
For input:  
`"NLP techniques are used in virtual assistants like Alexa and Siri."`

1. **Original Tokens**: `['NLP', 'techniques', 'are', ..., 'Siri', '.']`  
2. **Without Stopwords**: `['NLP', 'techniques', 'used', ..., 'Alexa', 'Siri']`  
3. **Stemmed Words**: `['nlp', 'techniqu', 'use', ..., 'alexa', 'siri']`

## Notes
- Requires NLTK data packages (`punkt`, `stopwords`)
- Stemming may produce non-dictionary words (tradeoff for simplicity)
