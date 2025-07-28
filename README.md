#  Dog Breed Classifier

> A deep learning project for classifying dog breeds and filtering out non-dog images using pre-trained CNN models (AlexNet, VGG, ResNet).  
> Forked and customized from Udacity's AI Programming with Python Nanodegree.

---

##  Project Goal

This project helps determine:
- Whether an image contains a **dog or not**
- If it's a dog, identify its **breed**
- Compare performance of **AlexNet**, **VGG**, and **ResNet**
- Measure runtime and evaluate accuracy/speed trade-offs

---

## 🗂️ Project Structure

```
.
├── data/
│   ├── check_images.py         # Main logic
│   ├── classifier.py           # Provided classifier using CNNs
│   ├── dognames.txt            # List of valid dog names
│   └── pet_images/             # Test images (dogs, cats, others)
├── test_classifier.py          # Run classifier manually
├── run_models_batch.sh         # Batch run for model comparison
├── requirements.txt            # Dependencies
├── README.md                   # Project documentation
```

---


## ✅ What I Did

- Extracted pet labels from filenames
- Used pre-trained CNNs (via classifier.py) to classify images
- Compared true labels with predicted labels
- Checked if predicted/true labels refer to dogs (via dognames.txt)
- Calculated and printed overall performance statistics

---

## 📊 Results Summary

| Model     | Dog Detection | Breed Accuracy | Not-a-Dog Detection |
|-----------|----------------|----------------|----------------------|
| AlexNet   |   100%         | 77.3%          | 100%               |
| ResNet    |   96.7%        | 88.7%          | 93.3%              |
| VGG       |   100%         |  93.3%         | 100%               |

 **Best model:** VGG — most accurate and consistent overall.

---

##  Project Overview

This project was developed by editing the main file: `check_images.py`.

### Main Steps:
- Parse command-line arguments
- Extract labels from image filenames
- Use classifier to predict labels
- Compare predictions with true labels
- Check if the image is of a dog or not
- Print results and statistics

> Models used are pre-trained on **ImageNet**.

---

##  Author

This project was completed as part of the AI Programming with Python Nanodegree.  
Customized and improved for portfolio and GitHub presentation.

