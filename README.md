# Simple CNN Thin Section XPL or PPL Classifier
 
Trained model (contained in model folder) where a pre-trained .h5 keras model (trained using 2180 images) is used for distinguishing between PPL and XPL thin sections

### Example of result given in the notebook (.ipynb)

![Classified XPL heart](result1.png)

### Result of classification on XPL and PPL in test images

![Clasification of all images in testimgs folder](animation.gif)

## Abour the model elaboration:

The model was trained on 2180 images (1090 XPL, 1090 PPL), due to a lack of computational power I reduced the image quality from around 1000x1000 px to 400x400px to train the model. All images are RGB.

The Training dataset and valitadion dataset were splitted 80% - 20% and data augmentation was used (width shift, height shift, zoom, flip).

### Accuracy on training set: 94%
### Accuracy on validation set: 88%

### Model Used

Standard model for binary classification with data augmentation:

<img width="400" alt="Standard model used" src="model.png">



### Training and Validation Accuracy
![Matplotlib graph with train and val acc](trainvalacc.png)

Maybe should have continued with more epochs... 

### Training and Validation Loss
![Matplotlib graph with train and val loss](trainvalloss.png)

-- UNAL, Iván Ferreira
