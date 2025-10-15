# CNN-Assignment-Waste-Segregation
📊 Data Insights

The dataset contained seven waste categories — Cardboard, Food Waste, Glass, Metal, Paper, Plastic, and Other.

Image sizes varied significantly, so all images were resized to a uniform dimension (224×224) for model consistency.

Class distribution analysis showed moderate imbalance, with categories like Other having fewer samples compared to Paper and Plastic.

Visual inspection of random samples helped confirm that the dataset contained clear, representative images for most classes, though some overlap existed between visually similar categories (Plastic vs Glass, Metal vs Paper).

Overall, the dataset provided a good variety of real-world waste images, suitable for training a CNN model for automatic waste segregation.

🤖 Model Training Results

A Convolutional Neural Network (CNN) was built using three convolutional blocks with Batch Normalization and Dropout for better generalization.

The model was compiled with the Adam optimizer and trained using categorical cross-entropy as the loss function.

Class imbalance was addressed using computed class weights, ensuring minority classes contributed fairly to the learning process.

Callbacks such as ModelCheckpoint, ReduceLROnPlateau, and EarlyStopping helped stabilize training and prevent overfitting.

Training Outcomes:

Final training accuracy reached approximately 74%, with a Top-3 Accuracy of about 91% on the validation set.

The confusion matrix showed that most misclassifications occurred between Plastic and Glass items — indicating the model sometimes struggles with transparent or reflective materials.

The classification report demonstrated balanced performance across most classes, with Cardboard and Paper achieving the highest precision and recall.

Overall, the model successfully learned to distinguish between different waste types, making it a strong baseline for automated waste segregation systems.

🌍 Key Takeaways

Image preprocessing (resizing, normalization) was crucial for consistent model input.

Class balancing and proper callbacks significantly improved the model’s stability.

With additional data and augmentation, the model’s performance could exceed 85–90% accuracy.

The approach demonstrates how deep learning can contribute to sustainable waste management by automating the segregation process efficiently.
