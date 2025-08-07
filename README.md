
Building AI course project
#  MedGuide – Assistant IA de compréhension d’ordonnances médicales

##  Résumé
**MedGuide** est un assistant intelligent qui aide les patients à comprendre leurs ordonnances médicales.  
À partir d’une photo ou d’un fichier PDF, l’IA analyse le texte, identifie les médicaments, les dosages et les horaires de prise, puis reformule les informations en langage clair, avec des pictogrammes et, en option, des rappels automatiques.

---

##   Contexte
### Problème à résoudre
De nombreux patients notamment les personnes âgées, les non-francophones et les personnes ayant des difficultés de lecture  peinent à comprendre leurs prescriptions médicales.  
Cela entraîne des erreurs de dosage, des oublis ou des prises incorrectes.

### Fréquence et importance
Les erreurs médicamenteuses sont une cause fréquente de complications médicales évitables.  
Une meilleure compréhension des ordonnances peut réduire ces risques et améliorer l’observance du traitement.

### Motivation personnelle
Rendre les instructions médicales compréhensibles et accessibles à tous, pour améliorer la santé publique et réduire les hospitalisations évitables.

---

##   Données et techniques d’IA
- **Sources de données** :
  - Images et PDF d’ordonnances (fictives ou anonymisées).
  - Bases publiques de médicaments (ANSM, DrugBank).
  - Jeux de données OCR open source (IAM Dataset, SROIE).
- **Techniques d’IA** :
  - **OCR** (reconnaissance optique de caractères) – ex. Tesseract, EasyOCR.
  - **NLP** (traitement du langage naturel) pour extraire noms de médicaments, dosages et horaires.
  - **Simplification automatique de texte** pour reformuler en langage clair.
  - **Pictogrammes** via bibliothèques médicales ou génération automatique.

---

##   Comment est-elle utilisée
1. L’utilisateur prend une photo de son ordonnance ou téléverse un PDF.
2. L’IA lit le texte (OCR) et l’analyse (NLP).
3. Les informations sont affichées sous forme :
   - d’un texte clair et simplifié ;
   - de pictogrammes illustrant moments de prise et précautions (ex. « Avant repas », « Matin »).
4. Optionnel : notifications automatiques pour rappeler les prises.

**Utilisateurs concernés** :
- Patients
- Aidants familiaux
- Médecins et pharmaciens

---

##  Schéma de fonctionnement

---

##  Défis
- Précision de l’OCR sur écritures manuscrites médicales.
- Mises à jour régulières des bases de médicaments.
- Respect strict de la confidentialité .
- Gestion multilingue et formats variés.

---

##  Et ensuite
- Ajout d’un module vocal pour expliquer oralement la prescription.
- Intégration avec le dossier médical partagé.
- Adaptation internationale (bases locales, langues multiples).
- Réalité augmentée : afficher les instructions directement sur la boîte.

---

##  Ressources
- **OCR** : [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) (Apache 2.0 License)
- **NLP** : [spaCy](https://spacy.io/), [Hugging Face Transformers](https://huggingface.co/) (Apache 2.0 License)
- Bases de données médicales : [ANSM](https://ansm.sante.fr/) (open data), [DrugBank](https://go.drugbank.com/) (licence spécifique)
- Inspiration : initiatives de santé publique pour l’accessibilité médicale

---
