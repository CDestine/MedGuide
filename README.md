# MedGuide – Assistant IA de compréhension d’ordonnances médicales
Building AI course Project

## Résumé
MedGuide est un assistant intelligent qui aide les patients à comprendre leurs ordonnances médicales.  
À partir d’une photo ou d’un fichier PDF, l’IA analyse le texte, identifie les médicaments, les dosages et les horaires de prise, puis reformule les informations en langage clair, avec des pictogrammes et, en option, des rappels automatiques.  
L’objectif est de réduire les erreurs médicamenteuses, améliorer l’observance et rendre l’information médicale plus accessible à tous, notamment aux personnes âgées et aux non-francophones.

## Contexte
### Le problème
De nombreuses personnes peinent à comprendre les prescriptions médicales : écriture illisible, termes techniques, instructions complexes.  
Cela entraîne des erreurs de prise de médicaments, pouvant avoir des conséquences graves sur la santé.

### Pourquoi c’est important
Les erreurs médicamenteuses représentent une cause importante d’hospitalisations évitables.  
En rendant les ordonnances compréhensibles, MedGuide contribue directement à la sécurité et au bien-être des patients.

### Motivation personnelle
Ce projet est né de l’observation de proches ayant des difficultés à suivre leurs traitements correctement faute d’explications claires.

## Données et techniques d’IA
- **Sources de données** :
  - Images ou PDF d’ordonnances (fictives ou anonymisées)
  - Bases publiques de médicaments (ANSM, DrugBank)
  - Jeux de données OCR (IAM Dataset, SROIE)
- **Techniques utilisées** :
  - **OCR** : Tesseract, EasyOCR
  - **NLP** : spaCy, modèles Transformers pour l’extraction d’entités médicales
  - **Simplification** : reformulation automatique du texte médical
  - **Pictogrammes** : bibliothèques d’icônes médicales

## Utilisation
1. L’utilisateur charge une photo ou un PDF de son ordonnance.
2. L’IA effectue l’OCR pour extraire le texte.
3. Les informations clés (médicament, dosage, horaire) sont identifiées.
4. L’ordonnance est affichée en langage clair avec pictogrammes.
5. Optionnel : rappels automatiques via notification.

**Utilisateurs cibles** :
- Patients
- Aidants
- Professionnels de santé

## Défis
- OCR sur écritures manuscrites difficiles à lire.
- Confidentialité et protection des données médicales (RGPD, HIPAA).
- Précision des extractions pour éviter toute erreur d’interprétation.
- Adaptation multilingue.

## Et ensuite
- Module vocal pour expliquer oralement la prescription.
- Intégration avec le Dossier Médical Partagé.
- Version mobile avec réalité augmentée affichant les instructions sur la boîte de médicament.

## Remerciements
- **OCR** : [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
- **NLP** : [spaCy](https://spacy.io/), [Hugging Face](https://huggingface.co/)
- Bases médicales : [ANSM](https://ansm.sante.fr/), [DrugBank](https://go.drugbank.com/)
- Inspirations : projets open source d’accessibilité médicale
