# Flight Booking Completion Prediction

This project builds a machine learning pipeline to predict whether a flight booking will be completed based on customer behavior and flight details. The pipeline includes data preprocessing, feature engineering, model training with cross-validation, evaluation metrics, feature importance visualization, and automatic PowerPoint summary slide generation.

## 📁 Project Structure

```
├── customer_booking.csv # Input dataset
├── flight_booking_model.py # Main script (modeling + PowerPoint)
├── PowerPoint_Template.pptx (opt.) # Optional template for presentation
├── flight_booking_model_summary.pptx # Output presentation file
├── README.md # You're here!

```

---

## 🚀 How to Run

### 1. Clone this repo or download the files

```bash
git clone https://github.com/your-username/flight-booking-model.git
cd flight-booking-model
```
### 📊 Features Engineered

The script adds custom features to enhance model prediction power:

total_wants: Sum of extra services requested.

log_purchase_lead: Log of lead time to booking.

log_length_of_stay: Log of duration at destination.

early_booking: Indicator for bookings made 30+ days in advance.

is_weekend_flight: Flag for weekend flights.

is_night_flight: Flag for night flights (after 8 PM or before 6 AM).

### 🤖 Model & Evaluation

Model: RandomForestClassifier (with balanced class weights)

Cross-validation: 5-fold StratifiedKFold

Metrics:

ROC-AUC Score

Precision, Recall, F1-Score

Confusion Matrix & Classification Report

The script outputs the scores and plots feature importance.

### 📽️ Output: PowerPoint Summary
After running the script:

A PowerPoint file named flight_booking_model_summary.pptx is created.

It includes key performance metrics and top 5 most important features.

If PowerPoint_Template.pptx is found in the folder, it's used as the base.

### ✅ Requirements
Python 3.7+

Libraries:

pandas

numpy

scikit-learn

matplotlib

python-pptx
