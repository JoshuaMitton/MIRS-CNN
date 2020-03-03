# MIRS-CNN

These are the models used to create the paper Age and species prediction of natural malaria mosquitoes through deep learning of mid-infrared spectra.

These are Tensorflow models for the task of classifying age and species of lab reared lab mosquitoes, lab reared field mosquitoes, and semi-field reared lab mosqutioes.


<h2> Model architecture </h2>

![ScreenShot](/imgs/CNN.png)


<h2> Datasets </h2>

The dataset used for this paper is available at the following address:

```Link to come soon```

![ScreenShot](/imgs/UMAP_Embedded_Mosquito_RearCnd.png)

![ScreenShot](/imgs/UMAP_Embedded_Mosquito_Country.png)

<h2> Pre-trained Models </h2>

The following pre-trained models are provided:

[Predict Lab Mosquitoes](/CNN/CNN-model/Results/Predict_Lab_Only/)

[Predict Field Mosquitoes](/CNN/CNN-model/Results/Predict_Lab_Field/)

[Predict Semi-Field Mosquitoes](/CNN/CNN-model/Results/Predict_Semi_Field/)


<h3> To make predictions with the pretrained models </h3>

```
X_test = DATALOADER
model = load_model(f'{loaddir}Baseline_CNN_Model.h5))
y_predicted = model.predict(X_test)
```


<h2> Python environment </h2>

```
python 3.6.8
tensorflow-gpu 1.12.0
keras 2.2.4
sklearn 0.21.3
numpy 1.17.2
matplotlib 3.1.1
pandas 0.25.1
tqdm 4.36.1
```
