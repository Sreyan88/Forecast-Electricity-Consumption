# TCS-HumAIn
### This Repository contains the code for TCS HumAIn competition

### Problem Statement:

Forecast the electricity consumption of top 3 households with highest number of samples on an hourly basis based on the previous usage pattern. The major features for analysis includes household id, the plans used (standard or dynamic time of use), date, time, meter readings in Kwh and acorn group.


<p align="center">
<b>Model Proposed</b><br><br>
<img width="299" height="451" src="https://github.com/Sreyan88/TCS-HumAIn/blob/master/Extra/tatadiag.png">
</p></br>

<p align="center">
  <b> Model Description </b><br>
  </p></br>
  
 ### Major Components of the model:
 
 1. Most important layers include Bi-directional LSTM, Bi-directional GRU and Conv 1D layers.
 
 2. Cyclic Learning Rate was used to train the model to take into account the problem of exploding and vanishing gradients.
 
 3. The auxillary input to the model consists of various features taken from the time-series sequence. The features include fractal dimension of the time-series and the hour of the day in the measurement was recorded.More information about the extra features is included with the code.
 
 4. Validation was done for MSE and MAE metrics.
 
 5. The model was trained and tested for 5 folds with Stratified K-Fold Startegy.
 
 
 ### Future Work for next round:
 
 1. Plan to use neural architecture search for finding better parameters for number of layers to be used.
 
 2. Tune the no. of time-steps to be used for prediction.
