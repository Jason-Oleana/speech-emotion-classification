# Speech-Emotion-Classification


## step 1: git clone project
```
git clone https://github.com/Jason-Oleana/Speech-Emotion-Classification.git
```

## step 2: Navigate to Speech-Emotion-Classification
```
cd Speech-Emotion-Classification
```

## Step 3: install all requirements

```
pip install -r requirements.txt
```

## step 4: Download RAVDESS-RawData
```
https://drive.google.com/drive/folders/1S3j7CkyGWDpjS6OMSGOL0ka_osKff_Vg?usp=sharing

Reference:
- Livingstone SR, Russo FA (2018) The Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS): A dynamic, multimodal set of facial and vocal expressions in North American English. PLoS ONE 13(5): e0196391. https://doi.org/10.1371/journal.pone.0196391
```

## step 5: Update my_path to RAVDESS-RawData in the .ipynb project
```
my_path = "your path to Ravdess-RawData"
```

## step 6: You can run the code :)

### Accuracy rate of SVM with MFCC features

```
3 emotions = happy, sad, neutral
5 emotions = happy, angry, neutral, sad, and fearful
8 emotions = happy, angry, neutral, sad, fearful, disgust, calm, surprised
```
![](SVM_results.PNG)

### Confusion matrix: best-performing SVM classifier (three emotions) with MFCC features

![](3-emotions-conf.PNG)

### Confusion matrix: best-performing SVM classifier (five emotions) with MFCC features

![](5-emotions-conf.PNG)

### Confusion matrix: best-performing SVM classifier (eight emotions) with MFCC features

![](8-emotions-conf.PNG) 

### Mel frequency cepstral coefficients (MFCCs)
Mel frequency cepstral coefficients are the most widely used speech feature for SER. 
Mel Frequency Cepstral Coefficients are derived from the cepstrum, which is the inverse spectral transform of the logarithm of the spectrum. 
They concisely describe the overall shape of a spectral envelope


### Speech feature categorization according to their temporal structure (suprasegmental vs. segmental) and parameterization (LLDs vs. functionals).


![](speech-features.PNG)


## Ideas 

- Data Augmentation (CNN needs more data for better training)
- Concatenate other speech features
- Concatenate other datasets for more training data
