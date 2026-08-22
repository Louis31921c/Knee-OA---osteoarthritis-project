# Knee-OA---osteoarthritis classification from machine learning


***Hi there*, in this project, I fine-tune a pretrained ResNet18 to grade knee articular cartilage, aka knee osteoarthritis, from X-ray images, using the Kellgren-Lawrence (KL) grading system — the clinical standard for classifying these symptoms with the following scale:**



- - Grade 0 — Healthy knee
- - Grade 1 — Doubtful narrowing, possible osteophytic lipping
- - Grade 2 — Definite osteophytes, possible joint space narrowing
- - Grade 3 — Multiple osteophytes, definite narrowing, mild sclerosis
- - Grade 4 — Large osteophytes, severe narrowing, severe sclerosis


**Goal would be to take any X-ray from a patient as input and predict its grade, using this machine learning model.**

**This dataset - from [kaggle](https://www.kaggle.com/datasets/shashwatwork/knee-osteoarthritis-dataset-with-severity) contains 8260 frontal X-ray of knees, already divided by grade from 0-4 and splitted in test/train/val. images are poorly reparted and it's the main issue we face ub this model. grade 4 is underrepresented when grade 0 and 2 take over 50% of the file.**


---


### **Approach:**
Most parameters and hyperparameters are easily tweakable to adjust performance and/or inputs

### **Evaluations:**
overall accuracy, per-class precision, ROC curves on the test set, final qualification model

### **Model:**
ResNet18 pretrained on ImageNet

### **Stacks:**
PyTorch · torchvision-ResNet18 · scikit-metrics · matplotlib · seaborn-visualization
