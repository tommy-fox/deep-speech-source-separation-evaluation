# deep-speech-source-separation-evaluation

<b>Abstract</b> 

Reliable automatic transcription of speech signals in noisy environments enhances technological access for individuals whose interaction would be otherwise limited. Applications include automatic closed captioning of video, hands-free voice control, and language translation systems among many others. Recently, end-to-end neural networks have been employed for the noisy speech transcription task, requiring little to no pre-processing of input data. In lieu of arduous feature engineering found in classical systems, end-to-end networks require large volumes of training data and carefully designed network architecture instead. While end-to-end neural networks have shown state of the art accuracy in transcribing noisy speech, there remains room for improvement. This work examined the effect of source separation preprocessing on the accuracy of the Deep Speech network, which was trained end-to-end. The data used for this experiment included two clean speech datasets and one dataset consisting of noise commonly found in urban environments. Deep Speech’s accuracy was tested using clean speech, unseparated noisy speech, and finally noisy speech after separation. Source separation methods included Open-Unmix, which utilizes Recurrent Neural Network-based Bidirectional Long-Short Term Memory, as well as Non-negative Matrix Factorization. Deep Speech’s Word Error Rate consistently improved across all signal to noise ratios and datasets processed with Open-Unmix, while Non-negative Matrix Factorization processing provided negligible improvement. These results indicate that deep learning context-based source separation preprocessing for speech transcription is an avenue worthy of further research, as is improving the model robustness of stand-alone end-to-end speech recognition systems.
<br><br>
 <p align="left">
 <b> Dataset Information <br>
 (used to train source separation methods and test Deep Speech) </b>
 </p>
<p align="center">
<img width="700" height="600" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/DATA_DURATION_DIST1.png">
</p>
<br><br>
 <p align="left">
 <b> Deep Speech Word Error Rate Results </b>
 </p>
<p align="center">
<img width="750" height="750" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/WER_CV1.png">
</p>

<p align="center">
<img width="750" height="750" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/WER_LIB1.png">
</p>

<br><br>
 <p align="left">
 <b> Spectrogram Examples from the Common Voice Dataset </b> <br>
This speech example was corrupted with dog barking at a 2to1 signal to noise ratio. <br>
Vocal separation was then applied using Open-Unmix (UMX) and Non-negative Matrix Factorization (NMF). <br>
Transcription label: "Could I please see you a minute.” <br>
 </p>
<p align="center">
<img width="600" height="300" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/spec_clean_no_dog_bark2.png">
</p>

<p align="center">
<img width="600" height="300" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/spec_noisy_dog_bark2.png">
</p>

<p align="center">
<img width="600" height="300" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/spec_nmf_dog_bark2.png">
</p>

<p align="center">
<img width="600" height="300" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/spec_umx_dog_bark2.png">
</p>
