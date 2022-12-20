# 📚 **BookEssence**: *Distill the Core of Knowledge in Minutes*

**BookEssence** is an AI-driven book synopsis tool that distills complex text into its most essential insights and primary takeaways. With **BookEssence**, you can quickly unpack the core of a book and save precious time without compromising comprehension.

## Key Features

- **Chapter-by-Chapter Summarization**: **BookEssence** provides detailed summaries for each chapter, allowing you to focus on specific areas of interest.
- **Whole Book Synopsis**: For books without chapter divisions, **BookEssence** condenses the entire text into a comprehensive overview.
- **Powered by Natural Language Processing (NLP)**: Leveraging cutting-edge NLP techniques, **BookEssence** intelligently processes text, capturing the most pertinent and informative content.
- **Sleek User Interface**: **BookEssence** features a clean and intuitive interface, making the summarization process smooth and user-friendly, regardless of technical proficiency.

## Workflow

**BookEssence** utilizes the `T5-small` pretrained model from HuggingFace Transformers to generate precise and readable summaries. The process unfolds as follows:

1. **Chunking**: The text of the book is segmented into chunks, either by chapter or as a whole.
2. **Tokenization**: The chunks are tokenized using the `T5Tokenizer` to be compatible with the `T5` model.
3. **Summary Generation**: The tokenized text is input into the `T5ForConditionalGeneration` model, which outputs summary token IDs.
4. **Decoding**: The summary token IDs are decoded back into intelligible text using the `T5Tokenizer`'s `decode()` function, resulting in the final summary.

## How to Begin

1. Clone the repository: `git clone https://github.com/Bella1i/BookEssence.git`
2. Install the necessary dependencies: `pip install -r requirements.txt`
3. Launch the application: `python3 app.py`

For more detailed instructions and advanced usage, please refer to the source code.

## Contributing

We value contributions from the community! If you wish to contribute to **BookEssence**, please feel free to submit a pull request or open an issue. Your feedback and support are greatly appreciated!

## License

**BookEssence** is distributed under the [MIT License](https://github.com/Bella1i/BookEssence/blob/master/LICENSE).
