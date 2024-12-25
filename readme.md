# SAT-SED: Semi-supervised Sound Event Detection by Pseudo-Labeling with Self-Adaptive Threshold Strategy

## Introduction
We propose self-adaptive threshold SED (**SAT-SED**).
- The SAT strategy adjusts the threshold in a self-adaptive manner during training based on the learning status of each class.
- The SAT strategy is composed of self-adaptive clip- (**SACT**) and frame-wise threshold (**SAFT**) strategies. As the SAT strategy is exclusively employed during the training phase, it improves the system’s performance without increasing the model’s parameters and inference time.
<div align="center"><img src="https://github.com/Spray-N/SAT-SED/blob/main/archive/img/pipeline.png?raw=true" width=100%> </div>

## Results
DESED2022 validation set
<table>
  <tr>
    <th>Methods</th>
    <th>EB-F1</th>
    <th>PSDS1</th>
    <th>PSDS2</th>
  </tr>
  <tr>
    <td>Baseline (CRNN)</td>
    <td>0.429</td>
    <td>0.351</td>
    <td>0.552</td>
  </tr>
  <tr>
    <td>+SAT</td>
    <td>0.534</td>
    <td>0.447</td>
    <td>0.650</td>
  </tr>
  <tr>
    <td>FDY-CRNN</td>
    <td>0.525</td>
    <td>0.435</td>
    <td>0.653</td>
  </tr>
  <tr>
    <td>+SAT</td>
    <td>0.542</td>
    <td>0.457</td>
    <td>0.662</td>
  </tr>
</table>

## Visualization
Comparison of pseudo-labelling accuracy in the case of different thresholding strategies on the DESED2022 validation set, where fading colors of diagonal elements refer to the disparity of accuracy.
<div align="left"><img src="https://github.com/Spray-N/SAT-SED/blob/main/archive/img/acc_compare.png?raw=true" width=50%> </div>

