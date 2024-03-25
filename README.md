# Disease Identification System

## Description
The Disease Identification System is a machine learning-based system that predicts the disease based on the symptoms provided by the user. It utilizes a Random Forest Classifier to classify the disease based on the input symptoms.

## Installation
To use the Disease Prediction System, follow these steps:
1. Clone the repository to your local machine: `git clone https://github.com/shan-2804/Disease_Identification_Model `
2. Install the required dependencies: `pip install -r requirements.txt`

## Usage
To use the Disease Prediction System, follow these steps:
1. Ensure that you have installed all dependencies and have the trained model file (`trained_model.joblib`).
2. Import the necessary functions from the provided modules.
3. Use the `predict_disease` function to predict the disease based on the input symptoms.

## Example
```python
from predict_disease import predict_disease

# Define symptoms and model
input_symptoms = ["cough", "fever", "headache"]
symptom_names = ["itching", "skin_rash", "nodal_skin_eruptions", "continuous_sneezing",
    "shivering", "chills", "joint_pain", "stomach_pain", "acidity",
    "ulcers_on_tongue", "muscle_wasting", "vomiting", "burning_micturition",
    "spotting_urination", "fatigue", "weight_gain", "anxiety",
    "cold_hands_and_feets", "mood_swings", "weight_loss", "restlessness",
    "lethargy", "patches_in_throat", "irregular_sugar_level", "cough",
    "high_fever", "sunken_eyes", "breathlessness", "sweating", "dehydration",
    "indigestion", "headache", "yellowish_skin", "dark_urine", "nausea",
    "loss_of_appetite", "pain_behind_the_eyes", "back_pain", "constipation",
    "abdominal_pain", "diarrhoea", "mild_fever", "yellow_urine",
    "yellowing_of_eyes", "acute_liver_failure", "fluid_overload",
    "swelling_of_stomach", "swelled_lymph_nodes", "malaise",
    "blurred_and_distorted_vision", "phlegm", "throat_irritation",
    "redness_of_eyes", "sinus_pressure", "runny_nose", "congestion",
    "chest_pain", "weakness_in_limbs", "fast_heart_rate",
    "pain_during_bowel_movements", "pain_in_anal_region", "bloody_stool",
    "irritation_in_anus", "neck_pain", "dizziness", "cramps", "bruising",
    "obesity", "swollen_legs", "swollen_blood_vessels",
    "puffy_face_and_eyes", "enlarged_thyroid", "brittle_nails",
    "swollen_extremeties", "excessive_hunger", "extra_marital_contacts",
    "drying_and_tingling_lips", "slurred_speech", "knee_pain",
    "hip_joint_pain", "muscle_weakness", "stiff_neck", "swelling_joints",
    "movement_stiffness", "spinning_movements", "loss_of_balance",
    "unsteadiness", "weakness_of_one_body_side", "loss_of_smell",
    "bladder_discomfort", "foul_smell_of_urine", "continuous_feel_of_urine",
    "passage_of_gases", "internal_itching", "toxic_look_(typhos)",
    "depression", "irritability", "muscle_pain", "altered_sensorium",
    "red_spots_over_body", "belly_pain", "abnormal_menstruation",
    "dischromic_patches", "watering_from_eyes", "increased_appetite",
    "polyuria", "family_history", "mucoid_sputum", "rusty_sputum",
    "lack_of_concentration", "visual_disturbances",
    "receiving_blood_transfusion", "receiving_unsterile_injections", "coma",
    "stomach_bleeding", "distention_of_abdomen",
    "history_of_alcohol_consumption", "fluid_overload", "blood_in_sputum",
    "prominent_veins_on_calf", "palpitations", "painful_walking",
    "pus_filled_pimples", "blackheads", "scurring", "skin_peeling",
    "silver_like_dusting", "small_dents_in_nails", "inflammatory_nails",
    "blister", "red_sore_around_nose", "yellow_crust_ooze"
]  # List of all symptom names
model = model = RandomForestClassifier(n_estimators=50, max_depth=5, random_state=40)  # Trained machine learning model

# Predict disease
predicted_disease = predict_disease(input_symptoms, model, symptom_names)
print("Predicted Disease:", predicted_disease)
```

## Contributing
Contributions to the Disease Prediction System are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (git checkout -b feature/your-feature-name).
3. Make your changes.
4. Commit your changes (git commit -am 'Add new feature').
5. Push to the branch (git push origin feature/your-feature-name).
6. Create a new Pull Request.
7. License

## Authors
Shnatanu Devaliya

## References
https://www.geeksforgeeks.org/disease-prediction-using-machine-learning/
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8896926/

## Troubleshooting
If you encounter any issues or have questions, please feel free to open an issue in the repository.


