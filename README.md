# Image Translation with CycleGAN

## 📜 Project Overview
This project demonstrates the use of **Cycle-Consistent Generative Adversarial Networks (CycleGANs)** for unpaired image-to-image translation. Unlike traditional supervised learning methods, CycleGANs do not require paired datasets. Instead, they use cycle-consistency loss to learn mappings between two domains.

## 📜 Project Description
This project implements a Cycle-Consistent Generative Adversarial Network (**CycleGAN**) to perform image-to-image translation between two unpaired datasets:
- **Horse2Zebra:** Transform horse images into zebra images and vice versa.
- **Maps:** Convert satellite images into maps and vice versa.

CycleGAN achieves these translations by employing two generators, two discriminators, and a cycle-consistency loss function to ensure semantic coherence between the input and the output.

## 🧩 Key Features

- **Unpaired Image Translation:** No need for paired images during training. 
- **Multiple Datasets:** Supports both the **horse2zebra** and **maps** datasets.
- **Advanced Techniques:** 
  - **Cycle Consistency Loss**: Ensures that images can be translated back to their original form.
  - **Instance Normalization**: Stabilizes training and improves results.
  - **GAN Losses**: Used in generators and discriminators for realistic outputs.
 

## 📂 Project Components

### 1. **Datasets**
- **Horse2Zebra Dataset**:
  - Source: TensorFlow Datasets.
  - Contains unpaired images of horses and zebras. This dataset is ideal for demonstrating unpaired image-to-image translation tasks using CycleGAN.
- **Maps Dataset**:
  - Source: TensorFlow Datasets.
  - Consists of unpaired satellite images and their corresponding map views. It is designed to test CycleGAN's ability to translate between geographic and visual domains.


### 2. **Model Architecture**
The CycleGAN model consists of:
- **Generators:** Create transformed images between two domains (e.g., horses → zebras).
- **Discriminators:** Identify whether images are real or generated.
- **Cycle Consistency Loss:** Ensures transformations maintain the original structure when reversed.


## 🔍 Insights and Learnings

- **CycleGAN Advantages:**  
  - Works without paired data.  
  - Applicable to diverse domains.  

- **Challenges:**  
  - Training GANs requires balancing generator and discriminator.  
  - Model performance depends on hyperparameter tuning.


## 📜 References
- **CycleGAN Paper:** https://keras.io/examples/generative/cyclegan/
- **Maps Dataset:** https://www.tensorflow.org/datasets/catalog/cycle_gan?hl=tr#cycle_ganmaps
- **horse2zebra Dataset:** https://www.tensorflow.org/datasets/catalog/cycle_gan?hl=tr#cycle_ganhorse2zebra


## 🤝 Contributors
🚀 **Developed as part of a group project** 
- Derya Çahan [GitHub](https://github.com/DeryaCahan)
- Sinem Şaziye Karaca [GitHub](https://github.com/SinemSKaraca)
- Zehra Bak [GitHub](https://github.com/zehrabak) 
- Umut Bide [GitHub](https://github.com/umutbide1)



