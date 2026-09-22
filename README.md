# Task 6: Text Analysis Tool

A Python-based text processing script designed to analyze a given block of text. This tool automates basic natural language processing (NLP) tasks, providing structural metrics and frequency counts for any input text.

## Features

- **Word Count**: Calculates the total number of words by splitting text accurately after removing punctuation.
- **Character Count**: Computes the absolute character count including spaces and special characters.
- **Vowel Frequency**: Counts the total occurrences of vowels (`a`, `e`, `i`, `o`, `u`) in a case-insensitive manner.
- **Repeated Words Detection**: Identifies words that appear more than once and logs their exact frequency using standard library optimizations.

## Getting Started

### Prerequisites

To run this project, you need to have Python installed on your system:
- Python 3.6 or higher

### Tools Used
- **Python**: Core programming language.
- **Jupyter Notebook**: Recommended environment for interactive execution and analysis.

### Installation & Execution

1. Clone or download this repository to your local machine.
2. Open your terminal or command prompt.
3. Run the script using Python:
   ```bash
   python text_analysis.py
   ```

## Implementation Details

The core logic follows standard NLP preprocessing steps:
1. **Case Normalization**: Converts all text to lowercase to prevent duplicate counting based on capitalization (e.g., treating "Python" and "python" as identical).
2. **Punctuation Removal**: Uses regular expressions (`re` module) to strip out punctuation marks so they do not attach to words.
3. **Tokenization**: Uses the `.split()` method to isolate individual words.
4. **Frequency Collection**: Utilizes `collections.Counter` to construct an optimized hash map of word distributions.

## Example Output

Given a sample paragraph, the tool outputs metrics in the following format:

```text
--- Text Analysis Results ---
Total Words: 24
Total Characters (with spaces): 173
Total Vowels: 54

Repeated Words and their counts:
 - 'language': 2 times
 - 'is': 2 times
 - 'a': 2 times
 - 'science': 2 times
```