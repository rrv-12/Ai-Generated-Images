# Welfare Scheme Information Extraction Pipeline

## Overview
This project is part of the NLP course assignment. It involves designing and implementing a Python pipeline to extract, summarize, and process information from welfare scheme documents. The goal is to transform the extracted data into descriptive write-ups, generate image prompts, ensure entity consistency, and evaluate outputs using machine learning and text-to-image models.

## Project Tasks

### Task 1: Data Processing and Understanding
- **Objective**: Collect and understand data for 10 welfare schemes.
- **Output**: 10 text files, each containing all data for a given welfare scheme.

### Task 2: Information Extraction
- **Objective**: Extract and generate three write-ups for each welfare scheme:
  1. Beneficiary and Problem Statement
  2. Application Process and Benefits
  3. Outcome and Impact
- **Approach**: Utilize free LLM APIs with descriptive prompts.
- **Deliverable**: A section in the report detailing the self-evaluation of information retention.

### Task 3: Summarization Using Transformer-Based LLMs
- **Objective**: Summarize the welfare scheme documents using models like Pegasus, DistilBERT, or T5.
- **Evaluation**: Use BLEU or ROUGE metrics to compare summaries with ground truth.
- **Improvement**: Perform parameter tuning or fine-tuning to improve evaluation scores.

### Task 4: Image Prompt Generation
- **Objective**: Convert write-ups into detailed image prompts suitable for text-to-image models.
- **Requirement**: Ensure clarity, specificity, and descriptive detail.

### Task 5: Ensuring Entity Consistency Across Prompts
- **Objective**: Maintain consistent representation of characters, objects, and locations across prompts.
- **Approach**: Use NLP techniques such as NER or LLMs for consistency.

### Task 6: Image Generation and Evaluation
- **Objective**: Generate images using text-to-image models (e.g., Stable Diffusion, DreamStudio).
- **Deliverable**: Evaluate the generated images for coherence and consistency.

## Implementation

### Tools and Technologies Used
- **Python Libraries**: `transformers`, `pandas`, `scikit-learn`, `numpy`, `matplotlib`
- **Text-to-Image Models**: Stable Diffusion, DreamStudio
- **LLMs**: Pegasus, T5, DistilBERT
- **Evaluation Metrics**: BLEU, ROUGE

### Deliverables
1. **Notebook**: `assignment_pipeline.ipynb` containing the complete pipeline implementation.
2. **Results File**: `results.txt` containing a list of dictionaries for each welfare scheme with prompts and generated results.
3. **Report**: `assignment_report.pdf` documenting methodology, results, and challenges.

### Example Output
For each welfare scheme:
1. **Original Text**
2. **Write-Ups**: Beneficiary and Problem Statement, Application Process and Benefits, Outcome and Impact.
3. **Image Prompts**
4. **Generated Images**
5. **Evaluation Metrics**

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/rrv-12/welfare-scheme-pipeline.git
   cd welfare-scheme-pipeline
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook:
   ```bash
   jupyter notebook assignment_pipeline.ipynb
   ```
4. Review the results and generated images.

## File Structure
- `assignment_pipeline.ipynb`: Main implementation.
- `results.txt`: List of results with image prompts.
- `assignment_report.pdf`: Detailed report with methodology, results, and challenges.
- `data/`: Directory containing text files for welfare schemes.
- `images/`: Directory containing generated images.

## Challenges and Solutions
- **Data Inconsistency**: Addressed by designing robust prompts and preprocessing the text data.
- **Model Performance**: Improved evaluation metrics through parameter tuning and fine-tuning.
- **Entity Consistency**: Leveraged NER and LLM techniques to ensure uniformity.

## Future Improvements
- Automate fine-tuning for transformer-based models.
- Explore advanced text-to-image models for better visual outputs.
- Extend the pipeline to handle multilingual welfare scheme documents.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- Thanks to the NLP course instructors for providing guidance.
- Tools like Stable Diffusion, Pegasus, and others made this project possible.

## Contact
For any queries, feel free to reach out:
- **Name**: Rishav Raj Verma
- **Email**: [rishavrajv255@gmail.com]
