# HuggingFace-CoNLL-Parquet-to-CoNLL-Converter

This repository contains Jupyter notebooks for converting HuggingFace CoNLL Parquet files to traditional CoNLL format. The project offers two conversion methods: one with label mapping and another without.

## Contents

1. `huggingface2conll_with_mapping.ipynb`: Converts Parquet files to CoNLL format with custom label mapping.
2. `huggingface2conll_without_mapping.ipynb`: Converts Parquet files to CoNLL format without label mapping.

## Features

- Convert HuggingFace CoNLL Parquet files to traditional CoNLL format
- Option to apply custom label mapping during conversion
- Preserve token and label information
- Handle multi-token entities
- Generate CoNLL files compatible with various NLP tools and frameworks

## Requirements

- Python 3.6+
- Jupyter Notebook
- pandas
- pyarrow (for reading Parquet files)

## Usage

1. Clone this repository:
   ```
   git clone https://github.com/SakibAhmedShuva/HuggingFace-CoNLL-Parquet-to-CoNLL-Converter.git
   cd HuggingFace-CoNLL-Parquet-to-CoNLL-Converter
   ```

2. Install the required dependencies:
   ```
   pip install pandas pyarrow jupyter
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

4. Open either `huggingface2conll_with_mapping.ipynb` or `huggingface2conll_without_mapping.ipynb` depending on your needs.

5. Follow the instructions in the notebook to load your Parquet file and perform the conversion.

## Notebooks Description

### huggingface2conll_with_mapping.ipynb

This notebook converts Parquet files to CoNLL format while applying a custom label mapping. It's useful when you need to transform or standardize the labels in your dataset.

Key features:
- Custom label mapping functionality
- Handles multi-token entities
- Generates IOB formatted output

### huggingface2conll_without_mapping.ipynb

This notebook performs a straightforward conversion from Parquet to CoNLL format without modifying the labels. Use this when you want to preserve the original labels from your HuggingFace dataset.

Key features:
- Direct conversion without label modification
- Preserves original label scheme
- Suitable for datasets with pre-standardized labels

## Contributing

Contributions to improve the conversion process or add new features are welcome. Please feel free to submit a Pull Request or open an Issue for discussion.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- HuggingFace for providing the datasets in Parquet format
- The NLP community for establishing and maintaining the CoNLL format standard
