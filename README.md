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

# 📁 Datasets Included in This Repository


## **A. Combined Voice Emotion Dataset**

**Location:** `emotions/`

### **Overview**

The Combined Voice Emotion Dataset is a **unified collection of emotional speech recordings** created by integrating multiple widely used, publicly available audio-emotion corpora. This dataset consists exclusively of **speech audio files**, each annotated with a **standardized emotion label**.  

Its primary objective is to provide a **diverse, comprehensive, and well-structured dataset** suitable for research in **speech emotion analysis** and **affective computing**.


### **Source Datasets**

- [**RAVDESS**](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio) – Ryerson Audio-Visual Database of Emotional Speech and Song  
- [**TESS**](https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess) – Toronto Emotional Speech Set  
- [**CREMA-D**](https://www.kaggle.com/datasets/ejlok1/cremad) – Crowd-Sourced Emotional Multimodal Actors Dataset  
- [**SAVEE**](https://www.kaggle.com/datasets/ejlok1/surrey-audiovisual-expressed-emotion-savee) – Surrey Audio-Visual Expressed Emotion  
- [**EmoDB**](https://www.kaggle.com/datasets/piyushagni5/berlin-database-of-emotional-speech-emodb) – Berlin Database of Emotional Speech  

These datasets are integrated to provide a **diverse set of speakers, age ranges, accents, languages, and recording conditions**, resulting in a unified and representative emotional speech dataset.


### **Contents in this repository**

- Audio files combined from all five datasets into a **single harmonized emotional-speech dataset**  
- Standardized emotion labels:  
  - angry, fear, happy, neutral, sad, surprised  
  - Additional labels (e.g., calm, disgust, boredom) appear when provided by specific datasets  
- **Unified metadata fields (when available):**  
  - Speaker ID  
  - Gender (male/female)  
  - Emotion label  
  - Intensity level (if specified by the source dataset)  
  - Transcript text (if available)  
  - Source dataset  
- All files follow **harmonized naming conventions** across the combined datasets


### **Emotion Classes**

The primary emotion categories in this dataset are:

- Angry  
- Fear  
- Happy  
- Neutral  
- Sad  
- Surprised  

Other emotions appear only when explicitly included in a source dataset.


### **Dataset Type and Structure**

All files in this dataset are:

- **WAV audio recordings**  
- Contain **speech produced by human speakers**  
- Represent a mixture of **male and female voices**  
- Recorded in **diverse acoustic and environmental conditions**  

Each audio sample retains its original content but is assigned a **unified and standardized emotion label** to harmonize differences among source datasets.


### **Purpose**

This dataset provides a **consolidated, high-diversity emotional speech resource**, suitable for:

- Cross-dataset emotion analysis  
- Robust evaluation of emotion-recognition systems  
- Research on variability across speakers, languages, and recording conditions  
- Studies in **affective computing**, **human–computer interaction**, and **speech psychology** .
   
  By combining multiple high-quality emotional speech datasets into a single curated resource, it offers **improved generalizability**, **broader emotional representation**, and **enhanced suitability for advanced academic and scientific research**.
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

### **Why combine FER2013 + CK+**
- **FER2013** → Real-world, diverse, imperfect images → robust learning.  
- **CK+** → Controlled, high-quality expressions → precise modeling.  

Together they provide balanced training data for **facial emotion recognition**.

---

## C. Text Datasets 

**Location:** `dataset_all_characters_copy.csv`

### Overview  

The Text Dataset is a unified collection of emotional and therapeutic text samples created by integrating multiple publicly available text corpora. It contains *cleaned and standardized lines of text* annotated with *emotion labels, role labels, and character types*.  

This dataset is designed to provide a *comprehensive and structured resource* for research in emotion classification, therapeutic chat agents, context-based empathy modeling, psychological NLP, and IFS-style cognitive pattern mapping.  



### Source Datasets

- [*GoEmotions*](https://www.kaggle.com/datasets/debarshichanda/goemotions) – Emotional text from various contexts  
- [*Empathetic Dialogues*](https://www.kaggle.com/datasets/atharvjairath/empathetic-dialogues-facebook-ai) – Conversations demonstrating empathy  
- [*DailyDialog*](https://www.kaggle.com/datasets/thedevastator/dailydialog-multi-turn-dialog-with-intention-and) – Multi-turn dialogues with intention annotations  
- [*Reddit Mental Health*](https://www.kaggle.com/datasets/neelghoshal/reddit-mental-health-data) – Mental health discussion posts  
- [*Medical Dialogue Dataset 100K*](https://www.kaggle.com/datasets/thedevastator/medical-conversation-corpus-100k) – Medical conversation corpus  
- [*Emotions Dataset for NLP*](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp) – Emotion-labeled text data  
- [*Mental Health Conversational Data*](https://www.kaggle.com/datasets/elvis23/mental-health-conversational-data) – Conversations related to mental health  
- [*Counsel-Chat*](https://huggingface.co/datasets/nbertagnolli/counsel-chat/viewer/default) – Counseling and therapeutic chat dataset  

These datasets are combined to provide a *diverse set of text samples across topics, roles, emotions, and conversational contexts*, resulting in a unified and representative text dataset.  



### Characters

The dataset contains text associated with the following *characters*:  

Inner Critic, Perfectionist, Controller, Avoidant Part, Procrastinator, Addictive Part, Blamer, Victimized Part, Fearful Part, Nurturer, Wounded Child, Sage, Warrior, Protector, Healer, Seeker, Reassurer, Self_Presence  


### Contents in this Repository

- Cleaned emotional text samples  
- Counseling and therapeutic conversations  
- Multi-turn dialogues with:  
  - Emotion labels (joy, sadness, anger, fear, neutral)  
  - Topics  
  - Text content  
  - Role labels (user/agent/therapist)  
- Unified emotion label mapping across datasets  
- Text assigned to predefined *character types*  


### Dataset Type and Structure

- *CSV text data*  
- Each line represents a *text sample*  
- Annotated with:  
  - id  
  - text  
  - character (assigned character type)  
  - emotion (primary emotion)  
- Multi-turn dialogues retain *role information*  
- *Balanced representation* for all character types  

---

### Purpose

This dataset provides a *high-quality resource for NLP research* and development, suitable for:  

- Emotion classification in text  
- Training therapeutic chat agents  
- Context-based empathy modeling  
- Psychological NLP applications  
- IFS-style cognitive pattern mapping  

  By consolidating multiple high-quality text datasets into a single curated resource, it offers *broad emotional coverage, diverse conversational contexts, and improved generalizability* for machine learning and NLP tasks.
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

