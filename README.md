# deep-speech-source-separation-evaluation

<b>Abstract</b> 

Reliable automatic transcription of speech signals in noisy environments enhances technological access for individuals whose interaction would be limited otherwise. 
Examples of this include automatic closed captioning of video, hands-free voice control, and language translation systems among many others. 
Recently, end-to-end neural networks have been employed for the noisy speech transcription task, requiring little to no preprocessing of input data. 
In lieu of arduous feature engineering, end-to-end networks require large volumes of training data. 
End-to-end neural networks have shown state of the art accuracy in transcribing noisy speech, however there remains room for improvement. 
This work examined the effect of source separation preprocessing on the accuracy of the Deep Speech network, which was trained end-to-end. 
The data used for this experiment included two clean speech datasets and one dataset consisting of noise commonly found in urban environments. 
Deep Speech’s accuracy was tested using clean speech, unseparated noisy speech, and finally noisy speech after separation. 
Source separation methods tested include Open-Unmix, which utilizes Bidirectional Long-Short Term Memory, as well as Non-negative Matrix Factorization. 
Deep Speech’s Word Error Rate consistently improves across all signal to noise ratios and datasets that were processed with Open-Unmix, while Non-negative Matrix Factorization showed no improvement. 
These results indicate that context-based source separation used in conjunction with end-to-end speech transcription is a worthy avenue of research. 
The present research could be expanded in the future to include tests involving convolutive noise. 
Future work should also explore this pipeline with alternate end-to-end speech recognition systems, as well as alternate source separation methods. 
<br><br>
 <p align="left">
 <b> Dataset Information </b>
 </p>
<p align="center">
<img width="700" height="600" src="https://raw.githubusercontent.com/tommy-fox/deep-speech-source-separation-evaluation/master/images/DATA_DURATION_DIST.png">
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
