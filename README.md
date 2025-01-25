# Arabic Spelling Correction Project

## Project Description

This project focuses on improving the accuracy of Arabic spelling and grammatical error correction using a combination of advanced machine learning techniques and traditional algorithms. The goal is to enhance the quality of Arabic text by correcting both spelling and grammatical errors, which is particularly challenging due to the complexity of the Arabic language's morphological and syntactic rules.

The project implements three different models for Arabic spelling correction:

1. **Fine-Tuning with AraBART**: A pre-trained sequence-to-sequence (Seq2Seq) model specifically designed for Arabic text, fine-tuned for grammatical error correction.
2. **LSTM (Long Short-Term Memory)**: A neural network model used for predicting the next word in a sequence, which helps in improving the coherence and flow of Arabic text.
3. **Levenshtein Distance Algorithm**: A traditional algorithm used for correcting spelling errors at the word level by calculating the minimum number of edits (insertions, deletions, or substitutions) required to transform one word into another.

## Data Used in the Project

The project relies on three main types of data for training and evaluation:

### 1. Copy-GEC Arabic Dataset

- This dataset contains Arabic sentences with both uncorrected and corrected versions, specifically designed for grammatical error correction tasks.
- It was used to fine-tune the **AraBART** model, which is a pre-trained Seq2Seq model tailored for Arabic text.
- The dataset was preprocessed using the **Hugging Face** library, which tokenizes the text into numerical representations suitable for machine learning models.

### 2. Arabic Newspaper Texts

- This dataset consists of Arabic text collected from various newspapers (e.g., Al-Sabah, Hespress, Akhbaruna).
- The text was preprocessed to remove noise and ensure proper formatting before being used to train the **LSTM** model.
- The LSTM model was trained to predict the next word in a sequence, improving the coherence and flow of Arabic text.

### 3. Jamid Dataset

- This dataset contains different morphological forms of Arabic words, which are used to analyze and correct spelling errors.
- The **Levenshtein Distance** algorithm was applied to this dataset to correct spelling errors at the word level by comparing the target word with its corrected form.

## Models and Techniques

### 1. AraBART (Fine-Tuning)

- **AraBART** is a pre-trained Seq2Seq model designed for Arabic text, fine-tuned on the **Copy-GEC Arabic** dataset for grammatical error correction.
- The model was evaluated using the **ROUGE** metric to measure its accuracy in correcting grammatical errors.
- Results showed that AraBART is highly effective in correcting complex grammatical errors in Arabic sentences.

### 2. LSTM (Long Short-Term Memory)

- The **LSTM** model was trained on the Arabic newspaper dataset to predict the next word in a sequence, improving the coherence and flow of Arabic text.
- The model was evaluated using **accuracy** as the primary metric, and it showed promising results in predicting the next word in a sequence, which helps in improving the overall quality of Arabic text.

### 3. Levenshtein Distance Algorithm

- The **Levenshtein Distance** algorithm was used to correct spelling errors at the word level by calculating the minimum number of edits required to transform one word into another.
- The algorithm was applied to the **Jamid** dataset, which contains different morphological forms of Arabic words.
- The results showed that the Levenshtein algorithm is highly effective in correcting spelling errors, especially for words with complex morphological variations.

## Results and Comparison

- **AraBART** outperformed the other models in correcting grammatical errors, making it the most suitable model for handling complex sentence structures.
# F1 Score Comparison
![Comparison of F1 Scores](https://github.com/khaled-rashwani/Arabic-Spelling-Correction/blob/main/images/F1%20Score.png?raw=true)

# Precision Score Comparison
![Comparison of Precision Scores](https://github.com/khaled-rashwani/Arabic-Spelling-Correction/blob/main/images/Precision.png?raw=true)

# Recall Score Comparison
![Comparison of Recall Scores](https://github.com/khaled-rashwani/Arabic-Spelling-Correction/blob/main/images/Recall.png?raw=true)

- **LSTM** showed strong performance in predicting the next word in a sequence, which helps in improving the coherence and flow of Arabic text.
- **Levenshtein Distance** was highly effective in correcting spelling errors at the word level, especially for words with complex morphological variations.

## Conclusion

This project demonstrates the effectiveness of combining modern machine learning techniques (such as fine-tuning pre-trained models and using LSTM networks) with traditional algorithms (like Levenshtein Distance) for Arabic spelling and grammatical error correction. The results indicate that these methods can significantly improve the quality of Arabic text, making them suitable for various applications in natural language processing.
