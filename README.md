# Indian Language Spell Checker

A Python-based spell correction system specifically designed for Indian languages written in English transliteration. This tool addresses the unique challenges of spell checking transliterated Indian text, where the same word can have multiple valid romanized spellings due to dialectal variations and lack of standardized transliteration.

## Features

- **Hybrid Correction Algorithm**: Combines phonetic matching using Double Metaphone with fuzzy string matching for optimal accuracy
- **Multi-dialect Support**: Handles various transliteration styles and regional spelling variations
- **Weighted Scoring System**: Uses a balanced approach (60% phonetic + 40% edit distance) for better matching
- **Batch Processing**: Efficiently processes multiple words from input files
- **Custom Dictionary Support**: Works with user-defined reference dictionaries

## How It Works

1. **Phonetic Analysis**: Uses Double Metaphone algorithm to generate phonetic codes for both reference words and input errors
2. **String Similarity**: Calculates edit distance using fuzzy matching (Levenshtein-based)
3. **Hybrid Scoring**: Combines phonetic and edit distance scores with optimized weights
4. **Best Match Selection**: Returns the highest-scoring correction from the reference dictionary


## Technical Details

- **Phonetic Algorithm**: Double Metaphone for sound-based matching
- **String Distance**: Fuzzy ratio calculation for character-level similarity
- **Scoring Formula**: `0.6 × phonetic_score + 0.4 × edit_score`
- **Language Support**: Optimized for Indian language transliterations

## Acknowledgments

Built for improving the accuracy of Indian language spell checking in digital content and research applications.
