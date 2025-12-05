# ANA-IFS-Data

This repository (`ANA-IFS-Data`) contains curated multimodal datasets including:

- **FacialEmotionsDataset/** → Training and testing images, CK+ metadata CSV  
- **emotions/** → Emotion-labeled images for model-specific classification  
- **questionnaire_data/** → Split CSV files of 34 IFS questionnaire questions  
- **ANA_Healing_Plan_Dataset.xlsx** → Excel sheet for IFS character healing plans  
- **HandGesturesDataset.csv** → Hand gesture dataset for multimodal integration  
- **dataset_all_characters_copy.csv** → Complete dataset of all 19 IFS characters

The goal is to provide a unified dataset collection for emotion recognition, psychological modeling, IFS-based analysis, and multimodal AI systems.

---

## 📁 Datasets Included in This Repository

---

## **A. Combined Voice Dataset**

**Location:** `emotions/`

### **Source datasets**
- [RAVDESS](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio)  
- [TESS](https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess)  
- [CREMA-D](https://www.kaggle.com/datasets/ejlok1/cremad)  
- [SAVEE](https://www.kaggle.com/datasets/ejlok1/surrey-audiovisual-expressed-emotion-savee)  
- [EmoDB](https://www.kaggle.com/datasets/piyushagni5/berlin-database-of-emotional-speech-emodb)  

### **Contents in this repository**
- Audio files combined from all five datasets into a **single harmonized dataset**.
- Standardized emotion labels:
  - happy, sad, angry, fear, disgust, surprise, neutral  
  - plus calm, boredom, depending on dataset availability.
- Unified metadata:
  - speaker ID  
  - gender  
  - emotion  
  - intensity (if provided)  
  - transcript (if available)  
  - dataset source  
- Harmonized naming conventions across all datasets.

### **Purpose**
This dataset enables robust **emotion recognition from speech** across:
- multiple speakers  
- age groups  
- languages  
- recording conditions  

Useful for emotion-AI, psychoacoustic modeling, therapeutic speech agents, and multimodal fusion.

---

## **B. Facial Expression Dataset**

**Location:** `FacialEmotionsDataset/` 

### **Source datasets**
- [FER2013](https://www.kaggle.com/datasets/msambare/fer2013)  
- [CK+ (Cohn-Kanade Extended)](https://www.kaggle.com/datasets/davilsena/ckdataset)

### **Contents in this repository**
- Cleaned grayscale facial images (48×48) and labeled expression images.
- CK+ sequence-based images including transitions: neutral → expression.
- Emotion labels include:
  - anger, disgust, fear, happiness, sadness, surprise, neutral  
  - (optional: contempt in CK+)

### **Why combine FER2013 + CK+?**
- **FER2013** → Real-world, diverse, imperfect images → robust learning.  
- **CK+** → Controlled, high-quality expressions → precise modeling.  

Together they provide balanced training data for **facial emotion recognition**.

---

## **C. Text Datasets**

**File:** `dataset_all_characters_copy.csv`

The text dataset is created by combining, cleaning, and standardizing samples from:

- **GoEmotions** – https://www.kaggle.com/datasets/debarshichanda/goemotions  
- **Empathetic Dialogues** – https://www.kaggle.com/datasets/atharvjairath/empathetic-dialogues-facebook-ai  
- **DailyDialog** – https://www.kaggle.com/datasets/thedevastator/dailydialog-multi-turn-dialog-with-intention-and  
- **Reddit Mental Health** – https://www.kaggle.com/datasets/neelghoshal/reddit-mental-health-data  
- **Medical Dialogue Dataset 100K** – https://www.kaggle.com/datasets/thedevastator/medical-conversation-corpus-100k  
- **Emotions Dataset for NLP** – https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp  
- **Mental Health Conversational Data** – https://www.kaggle.com/datasets/elvis23/mental-health-conversational-data  
- **Counsel-Chat** – https://huggingface.co/datasets/nbertagnolli/counsel-chat/viewer/default  

### **Contents in repository**
- Cleaned emotional text samples.
- Counseling & therapeutic conversations.
- Multi-turn dialogues with:
  - emotion labels  
  - topics  
  - text  
  - role labels (user/agent/therapist)  
  - dataset origin  
- Unified emotion label mapping across datasets.

### **Purpose**
Perfect for:
- emotional classification  
- therapeutic chat agents  
- context-based empathy modeling  
- psychological NLP  
- IFS-style cognitive pattern mapping  

---

## **D. Hand Gesture Dataset**

**File:** `HandGesturesDataset.csv`

This repository includes a gesture dataset **based on the HaGRID dataset**:

- **HaGRID** → https://www.kaggle.com/datasets/kapitanov/hagrid  

### **Contents in repository**
- Curated subset of HaGRID-style gestures:
  - stop, peace, okay, fist, thumbs-up, palm, victory, etc.
- Standardized metadata:
  - gesture label  
  - file path  
  - lighting (if applicable)  
  - dataset origin  
- Balanced class distribution.

### **Purpose**
Useful for:
- human–computer interaction  
- multimodal fusion  
- gesture recognition systems  

---

# **E. Synthetic IFS Questionnaire Dataset**


It contains **1.9 million+ synthetic psychological samples**.


## **IFS Character System**

### **Included: 19 characters**
- **10 Protectors**
  - e.g., Inner Critic, Perfectionist, Controller, Avoidant, Pleaser, etc.
- **9 Self-Led Parts**
  - e.g., Self, Nurturer, Healer, Sage, Confident Self, etc.

Each character has:
- emotional tendencies  
- fears  
- needs  
- personality rules  
- motivations  

Responses are generated based on these psychological patterns.

---

## **Questionnaire Structure**

**Location:** `questionnaire_data/`

### **Total questions: 34**  
Divided into **10 questionnaire pages** with 4 input types (Writing, Numerical scale 0–10, Single-choice, Multi-choice).
created based on IFS MAPPING.

---

## **All 34 Questionnaire Questions**

1. What brings you here today, and what part of you feels most activated right now?  
2. How comfortable do you currently feel exploring your inner world (0–10)?  
3. Are you aware of any internal tension, discomfort, or emotional pressure at the moment?  
4. Which part seems to need the most attention right now?  
5. How does this part usually show up in your daily life?  
6. What emotions does this part often carry or express?  
7. When did you first notice this part becoming active in your life?  
8. How intense does this part feel right now (0–10)?  
9. What does this part want you to understand about its feelings?  
10. What situations or thoughts activate this part the most?  
11. When this part is triggered, what typical behaviors or reactions follow?  
12. Does this part try to protect you from something specific?  
13. If yes, what is it trying to protect you from?  
14. What is this part afraid would happen if it stopped doing its role?  
15. How overwhelmed does this part feel (0–10)?  
16. What unmet needs does this part want you to know about?  
17. Does this part want safety, control, validation, reassurance, or calm?  
18. What would help this part feel more supported or understood?  
19. Does this part trust your core Self?  
20. If not, what concerns does it have?  
21. What emotions does this part hide beneath the surface?  
22. What does this part wish you could express more freely?  
23. What past events shaped this part’s personality?  
24. Does this part feel alone or burdened?  
25. How willing is this part to cooperate right now (0–10)?  
26. What would make this part feel safe enough to step back or relax?  
27. What positive intention does this part hold, even if its methods seem harsh?  
28. What does this part fear losing if it lets go of control?  
29. What boundaries does this part want you to establish?  
30. What new patterns or behaviors does this part want you to develop?  
31. How ready is this part to try a new approach (0–10)?  
32. What reassurance does this part need from you?  
33. What kind of support or guidance does this part want in difficult moments?  
34. Which character label best represents this part's personality? *(Final classification column)*

---
### F. ANA Healing Plan Dataset  

The **ANA Healing Plan Dataset** (`ANA_Healing_Plan_Dataset.xlsx`) contains structured information designed for **IFS-based psychological mapping and intervention planning**. It provides guidance on identifying, understanding, and supporting internal system parts (IFS “characters”) for therapeutic or research purposes.

#### Contents:
- **IFS Characters / Subpersonalities:**  
  - Each row represents one of the 19 IFS characters identified for the ANA model.  
- **Attributes & Metadata:**  
  - Character name, role, typical emotional patterns, triggers, and coping strategies.  
- **Healing & Intervention Guidelines:**  
  - Suggested approaches for working with each character, including reflective prompts, supportive dialogues, and therapeutic activities.  
- **Integration with Questionnaire Data:**  
  - Each character maps to relevant questionnaire items, allowing **automated or semi-automated evaluation** and research analysis.  

#### Purpose:
- Supports **IFS-style therapeutic modeling** in research or AI-assisted interventions.  
- Can be used alongside **voice, facial, and text datasets** to study correlations between emotional expression, internal parts, and therapeutic outcomes.  
- Ideal for researchers or developers building **multimodal emotion recognition, psychological analysis, or personalized intervention systems**.
  
---

# 📁 Repository Structure

```text
ANA-IFS-Data/
├── .gitattributes
├── README.md
├── FacialEmotionsDataset/
│   ├── test/                    # Test set images
│   ├── train/                   # Training set images
│   ├── CKdataset.csv           # CK+ dataset labels and metadata
├── emotions/                   # Separate emotion-labeled images folder
│   ├── angry/                  # Anger expression images
│   ├── fear/                   # Fear expression images
│   ├── happy/                  # Happiness expression images
│   ├── neutral/                # Neutral expression images
│   ├── sad/                    # Sadness expression images
│   └── surprise/               # Surprise expression images
├── questionnaire_data/
│   ├── questionnaire_dataset_part1.csv
│   ├── questionnaire_dataset_part2.csv
│   └── questionnaire_dataset_part3.csv
├── ANA_Healing_Plan_Dataset.xlsx
├── HandGesturesDataset.csv
└── dataset_all_characters_copy.csv

