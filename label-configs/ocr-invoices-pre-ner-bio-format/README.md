# OCR of Invoices for NER Tagging with BIO Format

This labeling config enables the first step of Named Entity Recognition (NER) on images of invoice documents - OCR text extraction and tokenization with all tokens initially tagged as "O" (Outside) in the BIO (Beginning, Inside, Outside) format. The output of this step will be used as input for the subsequent [NER tagging process](../ner-tagging-invoices-bio-format/).

---

## Preview

![ner-tagging-invoices-preview](./preview/ner-tagging-invoices-preview.png)

---

## Author & Contributors

- **Author**: [@meditas](https://community.labelstud.io/u/meditas/summary)
- **Contributors**: [@redeipirati](https://github.com/redeipirati)

---

## Special Instructions

This configuration provides a streamlined interface for OCR text verification and correction:

### OCR Requirements

Before using this configuration, ensure your invoice images are preprocessed with an OCR model:

- Full text content
- Word-level bounding boxes
- Initial "O" labels for all words

Supported OCR engines: Tesseract OCR, Azure Form Recognizer, LayoutLM, or other compatible engines.

A complete working example with an ML backend implementation can be found in the [Label Studio Community Forum](https://community.labelstud.io/t/label-studio-not-presenting-the-labels-and-ocr-text/530).

## More Info

For general usage and installation instructions, see the main
[README](../../README.md) of this repository.
If you have any feedback or suggestions, open a PR or issue on GitHub! 