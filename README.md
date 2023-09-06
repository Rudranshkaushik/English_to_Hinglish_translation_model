# English_to_Hinglish_translation_model

## Overview
This repository contains a Hinglish translation tool that converts English text into Hinglish. The translated text aims to sound natural and be easily understood by both native Hindi speakers and non-native Hindi speakers. The project ensures that the translations maintain clarity by retaining certain words in English while accurately conveying the meaning of the original English sentences.

## Problem Statement
The primary goals of this project are as follows:

1. **Natural Translation**: Develop a translation model capable of producing Hinglish text that closely mimics the language patterns of spoken Hindi.

2. **Clarity and Retention**: Retain certain words in English to enhance clarity and ease of understanding, especially for non-native Hindi speakers.

3. **Meaning Accuracy**: Ensure that the Hinglish translations accurately reflect the meaning of the original English sentences.

## Code Implementation
The project code provided in this repository includes the following key components and functionalities:

- **Translation Model**: The core of the project is the translation model, which utilizes SpaCy and the Google Translate API to convert English sentences into Hinglish.
  
- **Noun Extraction**: A function is included to identify and extract nouns from input sentences using the SpaCy library.

- **Translation Function**: Another function utilizes the Google Translate API to translate English sentences to Hindi.

- **Replacement Logic**: A function replaces nouns in the Hindi translation with their English counterparts while retaining certain words in English for clarity.

## Usage
To use this translation tool for your projects, follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine.

2. **Install Dependencies**: Ensure you have the necessary dependencies installed, such as SpaCy and the Google Translate API. Refer to the code and any provided documentation for installation instructions.

3. **Run the Code**: Execute the code to translate English text into Hinglish. Customize the input text and other options as needed.

4. **Provide Feedback**: As per the project requirements, please provide feedback on the quality of the Hinglish translations, including naturalness and accuracy, in the comment section of the code.

## Sample Usage
Here is a sample usage of the provided code:

```python
import spacy
from googletrans import Translator

# Define your input sentence
english_sentence = "I was waiting for my bag."

# Translate it to Hinglish
hindi_translation = translate_to_hindi(english_sentence)

# Replace nouns with English counterparts
result_sentence = replace_nouns_with_english(hindi_translation, english_sentence)

print("Input English Sentence:", english_sentence)
print("Hinglish Translation:", hindi_translation)
print("Final Hinglish Sentence with Nouns:", result_sentence)
