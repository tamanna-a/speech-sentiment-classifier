# speech-sentiment-classifier

Objective: Emotion recognition in speech. 

Data: The speech segments are extracted from the Emotional Prosody Speech and Transcripts (https://catalog.ldc.upenn.edu/LDC2002S28). It uses 2,324 WAV files, and all files are named with the format “speaker_session_emotion_start-time_content.wav”. These files are from 7 speakers (cc, cl, gg, jg, mf, mk, mm), labeled with 15 emotions (anxiety, boredom, cold-anger, contempt, despair, disgust, elation, happy, hot-anger, interest, neutral, panic, pride, sadness, shame).

Feature Extraction:
1. Praat for pitch and intensity
2. OpenSMILE for comprehensive acoustic-prosodic features- I use IS09 feature set, which includes 384 features

Model Training:
- Multi-layer Perceptron
- Leave one speaker out cross validation
