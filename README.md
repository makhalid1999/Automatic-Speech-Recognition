# Automatic-Speech-Recognition
Codes for classifying speech for recognition of words being said.
There are two codes here:
- First one uses Nvidia's Nemo's pre-Trained Model in order to recognize speech
- The second one is a custom CNN model to train for the "AudioMNIST" dataset available at https://github.com/soerenab/AudioMNIST/tree/master/data/01
## Custom Model
### Preprocessing
The data was obtained. It had different lengths, albeit the same sampling freqeuncy of 22050Hz. \\ The data was converted to the frequency domain using the FFT algorithm built in the system, which ultimately finds the equivalent of the DFT, i.e, the Discrete Fourier Transform. Now that we have gotten the signal into the frequency domain. We take the log of the signal as speech recognition is all about perception of sound waves and human beings perceive that in a logarithmic fashion, this is why the intensity of sound is taken in decibels.
### Classification
A CNN model was trained and used for classification. We got a somewhat good validation accuracy.
