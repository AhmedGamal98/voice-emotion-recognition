# Voice Emotion Recognition

> Detects emotions (calm, happy, fearful, disgust and more) from speech audio using MFCC, chroma and mel features with a neural-network classifier.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

## How it works

1. Read each `.wav` file with `soundfile`.
2. Extract audio features: **MFCC**, **chroma** and **mel spectrogram** (averaged over time).
3. Keep the target emotions and split the data into train and test sets.
4. Train a scikit-learn **MLPClassifier** and measure accuracy on the test set.
5. Save the trained model with `pickle`.

## Dataset

Uses the **RAVDESS** dataset (*Ryerson Audio-Visual Database of Emotional Speech and Song*, Livingstone & Russo, 2018, CC BY-NC-SA 4.0). It is not stored in this repo.

1. Download `Audio_Speech_Actors_01-24.zip` from [Zenodo](https://zenodo.org/record/1188976).
2. Extract it into a folder named `voice data set/` next to the notebook, so the files are at `voice data set/Actor_01/*.wav` and so on.

## Run it

```bash
pip install librosa soundfile numpy scikit-learn jupyter
jupyter notebook Model.ipynb
```

## Author

**Ahmed Gamal Saber**, Full-Stack Web Developer & AI Engineer
[LinkedIn](https://linkedin.com/in/ahmed-gamal-saber-382081169) · [GitHub](https://github.com/AhmedGamal98)
