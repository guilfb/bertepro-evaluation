# BERTEPro Evaluation Datasets: Bloom-Sentences-Similarity (BSS) and Bloom-Sentences-Similarity-en (BSS-en)

This repository contains the datasets created for evaluating the performance of the **BERTEPro** model on clustering tasks using the Bloom taxonomy as a reference framework. These datasets were designed to assess the ability of NLP models to group sentences into semantic categories based on the six cognitive levels of the Bloom taxonomy.

## Dataset Description

The datasets provided in this repository are:

- **Bloom-Sentences-Similarity (BSS)**: A dataset in French.
- **Bloom-Sentences-Similarity-en (BSS-en)**: A dataset in English.

Each dataset contains 36 sentences in total, grouped into six cognitive categories defined by Bloom's taxonomy. The categories reflect different levels of cognitive processes: comprehension, application, and higher-order thinking. 

Within each category, there are six sentences that are identical except for the verb, which is replaced with a synonym corresponding to that particular Bloom category. The goal is to test the capability of models to identify these semantic similarities and differences across the categories.

### Structure of the Dataset

Each dataset is structured as follows:

- **Cognitive Levels**: Sentences are divided into six categories according to Bloom's taxonomy:
  1. Remember
  2. Understand
  3. Apply
  4. Analyze
  5. Evaluate
  6. Create

- **Sentence Structure**: Sentences within each category share the same structure, with only the verb being replaced by a synonym corresponding to the specific cognitive process being represented. This ensures that models are evaluated on their ability to semantically differentiate between these verbs, rather than the broader sentence context.

The datasets are available in both French and English.

### Files Included

- `./data/BSS-fr.csv`: The French dataset (BSS) with sentences grouped by Bloom's categories.
- `./data/BSS-en.csv`: The English dataset (BSS-en) with sentences grouped by Bloom's categories.

### Dataset Format

Each dataset is provided in CSV format with the following columns:
- `category`: The Bloom cognitive category the sentence belongs to (e.g., "Remember", "Understand").
- `verb`: The verb used in the sentence, which corresponds to the specific cognitive level of the Bloom taxonomy.
- `sentence`: The sentence text.

### Example Entry

| category   | verb     | sentence                              |
|------------|----------|---------------------------------------|
| Remember   | memorize | Students should **memorize** the key concepts. |
| Remember   | recall   | Students should **recall** the main ideas.      |

## License

This dataset is available under the [MIT License](LICENSE).
