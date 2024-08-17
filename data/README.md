## Info

### About the data folders

- `for_mlm_ae_corpus` contains all document related to AEC 1
- `for_qa_data_annotated` contains all document related to AgXQA 1

However due to the size of the raw (and processed) files, we only provided a sample in those folders. Please reach out to [kpodojos](mailto:kpodojos@msu.edu) if you need the entirety of the documents pre- and post- processing.

### About the scripts/notebooks

- `aws_textract_pdf_conversion_ntbook.ipynb`
    - Please note that the processing (especially converting raw pdfs-to-text) requires Amazon Textract.
- `convert_joe_documents_to_text_ntbook.ipynb`
    - Mostly for the conversion and cleaning of HTML files to text
- `example_from_annotations_to_jsonl.ipynb`
    - Exporting the annotated file (json/csv) into proper SQuAD-like splits


### Outcomes

The final datasets are hosted and can be found here:
- [Agricultural Extension corpus](https://huggingface.co/datasets/msu-ceco/aec_v1)
- [Agricultural Extension question answering dataset](https://huggingface.co/datasets/msu-ceco/agxqa_v1)

