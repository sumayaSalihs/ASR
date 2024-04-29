# ASR(Automatic Speech Recognition on Multiple Ghanaian Languages)
Develop an automatic speech recognition (ASR) model using Speech Dataset collected by UG

## Dataset pre-processing
The dataset pre-porcessing was one of the time consuming yet interesting stage for me. It started first with getting to understand download the dataset onto my personal computer. With the dataset being large, I was only able to achieve this by purchasing a month free trial subscription on Dropbox, the leverage the dropbox storage to reduce burden on my personal computer. I spent days getting to understand the dataset, from listening to audios and also going through the selected transcribed audio excel sheet to understand the dataset. After have a fair understanding of the dataset, I decided to use only the selected transcripts audio files, firstly because not doing so wasn’t going to be possible because of my machine memory 
Setback, and secondary due to the fact that it had a transcription to it audio. So I had it in mind to employ supervised learning for its training. 

## Creation of Dataframe
I began first by reading the data from all five languages excel sheet existing in the selected transcribed audio directory into a dataframe object. After which I then combined all five data frames as one for a single processing of all datasets I will be using. The combination of all the dataset after cleanup was about 93,166, which was very large. So I thought to obtain a sample by IMAGE_SRC_URL grouped by each, I ensured that each locale was equally represented. I shrink datasize to allow me to have a huge room to augment in order to several varities of audio for a given transcription for my model to learn from. I employed a mechanism to change audio pitch and speed. After sampling I worked on he feature extraction with librosa library 'feature.mfcc' function. Right after I moved on to normalize my y_values. Using integer encoding, where each character is mapped with a character in the list of transcription. Because I used Stratified approach for splitting my dataset for both training and testing, both datasets had equal represemtation of unique transcription. The most difficult part of this stage was arriving at a shape that my model Architecture can work with. This mearnt that I kept looping between this step and the Model develepment and Training stage.

## Model development



## Training

## Evaluation

## Testing
