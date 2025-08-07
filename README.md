# MedGuide – AI Assistant for Understanding Medical Prescriptions
Building AI course project
## Summary
MedGuide is an intelligent assistant that helps patients understand their medical prescriptions.  
From a photo or PDF file, the AI reads the text, identifies the medicines, dosages, and intake schedules, then reformulates the information in plain language with visual icons, and optionally sets up automatic reminders.  
The goal is to reduce medication errors, improve adherence, and make medical information more accessible to everyone, especially elderly people and non-native speakers.

## Background
### The problem
Many people struggle to understand their medical prescriptions due to illegible handwriting, technical terminology, or complex instructions.  
This can lead to incorrect medication usage, which may have serious health consequences.

### Why it matters
Medication errors are a significant cause of preventable hospitalizations.  
By making prescriptions easier to understand, MedGuide directly contributes to patient safety and well-being.

### Personal motivation
This project was inspired by observing relatives who had difficulties following their treatment correctly due to unclear instructions.

## Data and AI techniques
- **Data sources**:
  - Images or PDFs of prescriptions (synthetic or anonymized)
  - Public drug databases (ANSM, DrugBank)
  - OCR datasets (IAM Dataset, SROIE)
- **Techniques**:
  - **OCR**: Tesseract, EasyOCR
  - **NLP**: spaCy, Transformers for medical entity extraction
  - **Text simplification**: automatic rephrasing of medical text
  - **Icons**: medical pictogram libraries

## How it is used
1. The user uploads a photo or PDF of their prescription.
2. The AI performs OCR to extract the text.
3. Key information (medicine, dosage, schedule) is identified.
4. The prescription is displayed in plain language with pictograms.
5. Optional: reminders are set via notifications.

**Target users**:
- Patients
- Caregivers
- Healthcare professionals

## Challenges
- OCR performance on handwritten prescriptions.
- Privacy and compliance with medical data protection (GDPR, HIPAA).
- Ensuring extraction accuracy to avoid interpretation errors.
- Multilingual adaptation.

## Next steps
- Voice module to explain the prescription orally.
- Integration with the Shared Medical Record.
- Mobile version with augmented reality to display instructions on the medicine box.

## Acknowledgements
- **OCR**: [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
- **NLP**: [spaCy](https://spacy.io/), [Hugging Face](https://huggingface.co/)
- Drug databases: [ANSM](https://ansm.sante.fr/), [DrugBank](https://go.drugbank.com/)
- Inspiration: public health accessibility initiatives
