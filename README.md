# Name: Jayadev Goskula (700757314)

# 1.NLP Preprocessing Pipeline Observation
## Pipeline Components
**Tokenization**: Splits text into individual words/punctuation  
**Stopword Removal**: Filters out common English words (e.g., "the", "are")  
**Stemming**: Reduces words to root form (e.g., "techniques" → "techniqu")

## Sample Output
For input:  
`"NLP techniques are used in virtual assistants like Alexa and Siri."`

1. **Original Tokens**: `['NLP', 'techniques', 'are', ..., 'Siri', '.']`  
2. **Without Stopwords**: `['NLP', 'techniques', 'used', ..., 'Alexa', 'Siri']`  
3. **Stemmed Words**: `['nlp', 'techniqu', 'use', ..., 'alexa', 'siri']`

## Notes
- Requires NLTK data packages (`punkt`, `stopwords`)
- Stemming may produce non-dictionary words (tradeoff for simplicity)


# 2.Named Entity Recognition (NER) Observation

## Implementation Highlights
- Uses spaCy's `en_core_web_sm` model for entity recognition
- Extracts entities with:
  - Text content
  - Entity type (PERSON, DATE, etc.)
  - Character positions in text

## Sample Output
Input:  
`"Barack Obama served as the 44th President..."`

Entities Found:
- `Barack Obama` (PERSON) [0:12]
- `the 44th` (ORDINAL) [21:28]
- `the United States` (GPE) [39:54]
- `the Nobel Peace Prize` (WORK_OF_ART) [64:84]
- `2009` (DATE) [88:92]

## Key Notes
- Requires spaCy and English language model
- Pre-trained model identifies common entity types
- Position tracking enables text highlighting/analysis


# 3.NLP Processing Pipeline - GitHub Observations

## 1. NLP Preprocessing Pipeline
### Core Functionality
- Tokenization using NLTK's `word_tokenize`
- Stopword removal (common English words)
- Porter stemming for word normalization

## 2. Named Entity Recognition (NER)
### Core Functionality
- Uses spaCy's pre-trained English model
- Identifies entities with labels and positions
- Handles PERSON, DATE, GPE, and WORK_OF_ART entities


## 3. Scaled Dot-Product Attention
### Core Functionality
- Implements transformer-style attention
- Computes Q·Kᵀ with √d scaling
- Applies softmax for attention weights
- Produces weighted value output

# 4.Sentiment Analysis Observation

## Implementation
- Uses Hugging Face's `transformers` pipeline
- Pre-trained model for sentiment classification
- Returns label (POSITIVE/NEGATIVE) with confidence score

## Key Features
- Zero-shot classification (no training needed)
- Handles nuanced sentiment (mixed statements)
- High confidence score indicates strong positive sentiment



