# Highway-inspection-and-maintenence-using-AI
Problem Statement

Manual highway inspection for damages such as potholes, cracks, faded kerb paint, and damaged crash barriers is time-consuming, costly, and prone to human error. This delays maintenance and increases the risk of accidents.

Objective

To develop an AI-based computer vision system that automatically detects and classifies highway defects from road images, enabling faster and safer road maintenance decisions.

🔬 Methodology

Data Collection

Collected images from Roboflow, Kaggle, and open-source datasets.

Categories: potholes, cracks, faded kerb paint, damaged crash barriers.

Augmented data for varying lighting, weather, and road conditions.

Preprocessing

Removed blurry/unusable images.

Applied data augmentation (rotation, brightness, noise).

Normalized images for training.

Model Development

Trained YOLOv5 (You Only Look Once) object detection model.

Used transfer learning for better accuracy with limited data.

Fine-tuned hyperparameters (epochs, batch size, confidence threshold).

Evaluation

Achieved mAP (Mean Average Precision): ~92%.

High recall in pothole and crack detection.

Deployment

Built a simple web dashboard (Streamlit/Flask) to upload road images.

Model outputs detected damages with bounding boxes + severity level.

Suggested maintenance priority (urgent, moderate, low).

 Key Results

Automated damage detection with real-time inference (<1 sec per image).

Reduced manual inspection effort by ~70%.

Helps prioritize repairs → improves road safety.

 Applications

Government highway authorities.

Road maintenance contractors.

Smart city projects.

Autonomous vehicle navigation (road condition awareness).
