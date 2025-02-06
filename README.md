# Personal Information Extraction using NLP & Regex

## Overview
This project demonstrates how to extract personal information such as name, age, birth date, and birth place from unstructured text using **Natural Language Processing (NLP)** and **Regular Expressions (Regex)**. It can be used for text processing tasks in AI applications like chatbots, data mining, and automated reporting.

## Features
- Extracts structured personal data from raw text
- Uses **Regular Expressions** to identify key entities
- Supports parsing information such as:
  - **Name**
  - **Age**
  - **Birth Date**
  - **Birth Place**
- Easily extensible for additional fields (e.g., occupation, relatives, nationality)

## Installation
Ensure you have **Python 3.x** installed along with the required libraries.

### Clone the Repository
```sh
git clone https://github.com/Sanjaykrishnank29/Regex_code_for_Chatbot.git
cd regex_for_information_extraction
```

### Install Dependencies
```sh
pip install -r requirements.txt
```

## Usage
```python
from extractor import extract_personal_information

text = '''
Born	Mukesh Dhirubhai Ambani
19 April 1957 (age 64)
Aden, Colony of Aden
(present-day Yemen)
'''

result = extract_personal_information(text)
print(result)
```

### Expected Output:
```python
{
  'name': 'Mukesh Dhirubhai Ambani',
  'age': 64,
  'birth_date': '19 April 1957',
  'birth_place': 'Aden, Colony of Aden'
}
```

## File Structure
```
NLP-Personal-Info-Extraction/
│── extractor.py         # Core logic for regex-based extraction
│── test_data.txt        # Sample text files for testing
│── README.md            # Project documentation
└── main.py              # Entry point for running the script
```

## Contributing
Feel free to fork this repository, submit issues, and contribute by making pull requests.

## License
This project is licensed under the **MIT License**. See the `LICENSE` file for details.

