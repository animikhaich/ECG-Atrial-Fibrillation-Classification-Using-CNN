[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="assets/icon.png" alt="Logo" width="150" height="150">

  <h2 align="center">ECG based Atrial Fibrillation Classifier using 1D CNNs</h2>

  <p align="center">
    A CNN based to classify the ECG signals of a patient with and without Atrial Fibrillation. Accuracy Achieved: 93.33%.
    <br />
    <a href="https://nbviewer.jupyter.org/github/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/blob/master/Data_Preprocessing.ipynb">Data Preprocessing Notebook</a>
    ·
    <a href="https://nbviewer.jupyter.org/github/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/blob/master/Model.ipynb">Model Notebook</a>
    ·
    <a href="https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/issues/new">Report Bug</a>
  </p>
</p>
<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
- [Jupyter Notebooks - nbViewer](#jupyter-notebooks---nbviewer)
- [Dataset Information](#dataset-information)
- [How to Run](#how-to-run)
  - [Hardware Used for the Experiment](#hardware-used-for-the-experiment)
  - [Built With](#built-with)
- [Changelog](#changelog)
- [Contributing](#contributing)
- [License](#license)
- [Future Improvements](#future-improvements)
- [Contact](#contact)
    - [Animikh Aich](#animikh-aich)

<!-- ABOUT THE PROJECT -->

## About The Project

This is a CNN based model which aims to automatically classify the ECG signals of a normal patient vs. a patient with Atrial Fibrillation and has been trained to achieve up to `93.33%` validation accuracy.

The CNN used here is 1D Convolutional Neural Networks.


## Jupyter Notebooks - nbViewer

- [Dataset Preparation Notebook](https://nbviewer.jupyter.org/github/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/blob/master/Data_Preprocessing.ipynb)
- [Model - Main Notebook Containing the Dataset Loader and Model Architecture](https://nbviewer.jupyter.org/github/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/blob/master/Model.ipynb)


## Dataset Information

- Download the dataset from [MIT-BIH Atrial Fibrillation Database](https://physionet.org/content/afdb/1.0.0/)

Note: The dataset has been moved from the original URL. Hence, the dataset provided above may be different from the one that was originally used to create this project. 

## How to Run

The experiment should be fairly reproducible. However, a GPU would be recommended for training. For Inference, a CPU System would suffice.

1. Download the dataset from the above mentioned link.
2. Put them in the desired path and change the path of the `Data_Preprocessing.ipynb` to be able to read the signals from the downloaded CSVs.
3. Save the processed dataset as a Numpy Object in the desired location.
4. In the file `Model.ipynb` read the saved processed dataset and train the model.
5. Any unknown dataset can be then classified by using `model.predict()` function after the `model` has been trained successfully. 

### Hardware Used for the Experiment

- CPU: AMD Ryzen 7 3700X - 8 Cores 16 Threads
- GPU: Nvidia GeForce RTX 2080 Ti 11 GB
- RAM: 32 GB DDR4 @ 3200 MHz
- Storage: 1 TB NVMe SSD (This is not important, even a normal SSD would suffice)
- OS: Ubuntu 20.10

Alternative Option: [Google Colaboratory - GPU Kernel](https://colab.research.google.com/)


### Built With

Simple List of Deep Learning Libraries. The main Architecture/Model is developed with Keras, which comes as a part of Tensorflow 1.x

- [Tensorflow](https://www.tensorflow.org/)
- [Scikit Learn](https://scikit-learn.org/)
- [Keras](https://keras.io/)
- [Matplotlib](https://matplotlib.org/)
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)


## Changelog

Since this is a Proof of Concept Project, I am not maintaining a CHANGELOG.md at the moment. However, the primary goal is to improve the architecture to make the predicted masks more accurate.


## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.

## Future Improvements
This is a preliminary attempt and is a work-in-progress:
1. In this particular implementation, only 10 Normal patients' data and 10 Abnormal patients' data has been taken and used. The entire dataset has not been used. Using the complete dataset may significantly improve the model accuracy. 
2. The CNN architecture can be further modified so as to find an optimal architecture that will learn better than the existing one.
3. As per experimentation, SGD (Stochastic Gradient Descent) optimizer works the best. However, with further change in model architecture, other optimizers like Adam and RMSProp may outperform the rather primitive SGD optimizer.

## Contact

#### Animikh Aich

- Website: [Animikh Aich - Website](http://www.animikh.me/)
- LinkedIn: [animikh-aich](https://www.linkedin.com/in/animikh-aich/)
- Email: [animikhaich@gmail.com](mailto:animikhaich@gmail.com)
- Twitter: [@AichAnimikh](https://twitter.com/AichAnimikh)



[contributors-shield]: https://img.shields.io/github/contributors/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN.svg?style=flat-square
[contributors-url]: https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN.svg?style=flat-square
[forks-url]: https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/network/members
[stars-shield]: https://img.shields.io/github/stars/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN.svg?style=flat-square
[stars-url]: https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/stargazers
[issues-shield]: https://img.shields.io/github/issues/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN.svg?style=flat-square
[issues-url]: https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/issues
[license-shield]: https://img.shields.io/github/license/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN.svg?style=flat-square
[license-url]: https://github.com/animikhaich/ECG-Atrial-Fibrillation-Classification-Using-CNN/blob/master/LICENSE.md
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/animikh-aich/
[product-screenshot]: assets/face-blur-demo.gif
