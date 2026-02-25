#  Pet Breed Classification: CNN vs. SIFT-BoVW

A comparative Computer Vision study exploring how to tackle fine-grained image classification in a **low-data regime** (~160 images per class from the Oxford-IIIT Pet Dataset). 

This project pits a modern Deep Learning approach against a Traditional Feature Engineering pipeline to see which handles data scarcity better.
For a detailed analysis read the pdf report!

### Key Features
* **Multi-Task Learning CNN:** A custom Dual-Head U-Net that learns to classify the breed *and* segment the pet (Foreground/Background) simultaneously, using segmentation as a regularizer.
* **Traditional Pipeline (BoVW):** A classic Bag-of-Visual-Words model utilizing **SIFT** descriptors, K-Means clustering, and a Multi-Layer Perceptron (MLP).
* **Robustness Testing:** Evaluates both models against synthetically generated noisy backgrounds to test spatial attention.
* **Mask-Guided SIFT :** An experimental pipeline that builds visual vocabularies strictly from foreground object features, achieving the highest accuracy in the study!

### Tech Stack
* **Deep Learning:** PyTorch
* **Computer Vision:** OpenCV (SIFT, Image Processing)
* **Data Science:** NumPy, Matplotlib

### How to Run
The entire pipeline is contained within a single Jupyter Notebook. Simply open the notebook in a clean Google Colab environment and run it from top to bottom. It will automatically download the dataset, process the images, train the models, and generate the final visualization report.
