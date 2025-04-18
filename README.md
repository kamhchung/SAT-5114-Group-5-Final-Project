# SAT-5114-Group-5-Final-Project
Group five, Ananya Kamath and Kameron Chung

Persistent Pulmonary Hypertension of the Newborn (PPHN) is a condition that is prominent in infants, characterized by pulmonary vascular resistance. In infants, this can cause blood shunting and hypoxemia affecting multiple organs (Lakshminrusimha & Keszler, 2015). Combined, these factors can result in decreased oxygen availability which presents as cyanosis, increased work of breathing, acidosis, brain damage, and possible death if not treated early enough (Tauber, 2024). For this project, the target population for early diagnosis of PPHN is term and late preterm infants.

This model will provide significant support in clinical settings such as Pediatric and Neonatal Intensive Care Units. PPHN typically develops and presents within the first 12 hours following birth (Nandula & Shah, 2023). Due to the presentation period of this complication, most diagnoses happen at the mother's bedside or within the NICU and treatment may be escalated to neonatal or pediatric cardiology. When an infant is born, the entire circulatory system is rerouted in order to transition from placental oxygenation to pulmonary oxygenation. When an issue with this transition occurs, PPHN can develop. Given the severity of the condition, patients who are stabilized at birth will still require continuous monitoring. 

# Methodology
To start, the team began considering the model types that would best serve the intent of the project. For supervised learning models, diagnostic classification is a key element. As such, using logistic regression was extremely important to use in this model. 


# ICD Codes
When implementing any tool in a setting, it is important to ensure that it is being used for the appropriate situation and environment. The first step of the model uses ICD codes to classify diseases. Using this check, the model will verify appropriate use.

# APGAR score calculator
APGAR scoring is extremely important in quickly evaluating a neonate's overall health at 1 minute of life, five minutes of life and ten minutes of life. Many facilities follow the Neonatal Resusitation Program's guidance on action to take based on APGAR scores. 

# Symptoms Entry
To accommodate an AI model, the input of symptoms and demographics are formatted in a categorical/binary fashion. Each symptom and risk factor indicative of PPHN will be encoded as a binary feature or multi-class depending on the values of the symptom. 


# Determining Patient Risk / Mortality Risk
The model allows providers to identify neonates at risk of developing PPHN. The calculator will include common perinatal and neonatal risk factors of PPHN. The results will show if further diagnostic testing is appropriate and recommended.


# Input Layer
The user will input the following information:

Infant Gestational Age: Physicians should input the gestational age of the patient in weeks and days to determine that the patient is in the appropriate range for diagnosis of PPHN.

Sex: Studies show that males are at a higher risk for developing PPHN, so the sex of the patient can impact model calculations (Razzaq et. al., 2013).

Delivery Mode: Studies show that infants born via caesarean section are at a higher risk for developing PPHN (Razzaq et. al., 2013). 

APGAR Score: Determines infant health immediately after birth. It measures appearance, pulse, grimace, activity, and respiration to calculate a score between 0 and 10 that can determine if further evaluation and treatment after birth is required.The User will enter each criteria into a calculator.

Symptoms: Presence of relevant symptoms that can impact diagnosis, risk, and mortality.

# Output Layer
For this layer, the model will provide the following information to aid physicians and patients:

ICD 10 Check: Determine whether the patient is appropriate for this model. Will ensure the user has the correct information for the model.

APGAR Calculator: Gives APGAR score and recommendations.

PPHN Assessment tool: Determine PPHN risk, mortality risk, and recommended actions.

PPHN Mortality Risk Predictor: Plot the patient on a graph compared to sample patients to show mortality risk.

Treatment Plan support: The model will suggest appropriate monitoring frequency based on current status, recommended monitoring, labs, and test, as well as an age-based trend prediction to provide families with information on trends of disease progression.

Disease Summary: Provide families with a summary of the disease that they can access at any time to ensure understanding and transparency with diagnosis.

# Data
This model was trained on data from an observational study done at the Children's Hospital and the Institue of Child Health in Multan, Pakistan in 2012. Our team attempted to use the CDC's Period Linked Birth-Infant Death File from 2015, however, the dataset was too large and incompatible with the Google Colab Notebook we used to write the program. In the future, we would like to figure out how to use this data to implement during training, using direct patient data containing all of the input criteria our model is using.  

# Recorded Presentation
Please follow this link to watch our recorded presentation.

https://youtu.be/fCcd6RjMLBI

# Summary
In summary, our model utilized data from the given dataset to calculate risk for neonates developing PPHN and is be able to suggest diagnostic proceedings if necessary.

