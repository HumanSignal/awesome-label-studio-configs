# NER Tagging for Invoices (BIO Format)

This labeling config enables Named Entity Recognition (NER) on invoice documents using the BIO (Beginning, Inside, Outside) format. It combines OCR text recognition with entity tagging for key invoice elements.

---

## Preview

![ner-tagging-invoices-preview](./preview/ner-tagging-invoices-preview.gif)

---

## Author & Contributors

- **Author**: [@meditas](https://community.labelstud.io/u/meditas/summary)
- **Contributors**:
  - [@redeipirati](https://github.com/redeipirati)

---

## Special Instructions

- **Image Display**: This config displays the invoice image with zoom and rotation controls.
- **OCR Text**: Editable text area showing the recognized text from the invoice.
- **BIO Format Labels**: 
  - B- prefix: Beginning of an entity
  - I- prefix: Inside/continuation of an entity
  - O: Outside/not part of any entity
- **Entity Types**:
  - NIF: Tax identification number
  - FORN: Supplier information
  - DATA: Date information
  - VALOR: Amount/Value
  - NUMFAT: Invoice number

### OCR Preprocessing Required with Label Studio ML model backend

Before using this configuration, you need to preprocess your invoice images with OCR:

1. **OCR Preprocessing**: Run an OCR engine on your invoice images before importing them into Label Studio. You can use:
   - Tesseract OCR
   - Azure Form Recognizer
   - LayoutLM
   - Other OCR engines

2. **Data Format**: Ensure your OCR results include:
   - The full text content
   - Word-level bounding boxes
   - Initial "O" labels for all words

A complete working example with an ML backend implementation can be found in the [Label Studio Community Forum](https://community.labelstud.io/t/label-studio-not-presenting-the-labels-and-ocr-text/530).

## More Info

For general usage and installation instructions, see the main
[README](../../README.md) of this repository.
If you have any feedback or suggestions, open a PR or issue on GitHub! 