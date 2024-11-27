# Benchmark IDP

Ce projet implémente un benchmark comparant trois solutions d'extraction de contenu de documents sur un ensemble de métriques clés. Les résultats sont visualisables dans une interface interactive.

---

## **Solutions Comparées**

1. **Docling v2**  
   Une solution moderne utilisant des modèles avancés pour extraire et structurer le contenu des documents.

2. **LayoutParser**  
   Une bibliothèque Python dédiée à l'analyse de la mise en page et à l'extraction de contenu à partir de documents numérisés.

3. **Tesseract + TableBank**  
   Une combinaison d'OCR via Tesseract et d'extraction de tableaux basée sur TableBank.

---

## **Métriques Évaluées**

1. **Temps de Traitement**  
   Mesure la rapidité des solutions pour extraire le contenu d'un document.

2. **Similarité Textuelle**  
   Compare le contenu extrait à un texte de référence en utilisant des métriques telles que :
   - **Cosine Similarity**
   - **BLEU**
   - **ROUGE**

---

## **Structure du Projet**

### **Répertoires**

- `data/input/`  
  Contient les documents à traiter (PDF, images, DOCX, etc.).
  
- `data/output/`  
  Stocke les résultats des extractions et des analyses.

- `notebooks/benchmark.ipynb`  
  Contient le notebook principal qui exécute :
  - Le chargement des solutions d'extraction.
  - Le calcul des métriques.
  - La visualisation des résultats.

### **Visualisation**

Le notebook génère une interface utilisateur permettant de :
- Comparer les résultats des solutions sur des documents donnés.
- Visualiser les annotations, textes extraits et tableaux détectés.
- Explorer les performances des solutions via des graphiques et des métriques.

---

## **Installation**

### **Prérequis**
- Python 3.10 ou supérieur.
- Jupyter Notebook.

### **Étapes**

1. Clonez le dépôt :
   ```bash
   git clone [<URL-DU-REPO>](https://github.com/Artemis-IA/benchmark-idp.git)
   cd benchmark-idp
