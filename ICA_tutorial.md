#How to Conduct and ICA (Independent Component Analysis)
**What is it?**
A method for correcting ocular artifacts using a blind source separation
technique to separate a set of independent signals from a set of mixed signals
In essence, ICA un-mixed the independent signals from the mixed signals so we
can better distinguish what we are looking for amidst the "noise"

**How to Conduct an ICA? step by step**
1. Run eeg lab and choose file/data you want to analyze/filter
2. Select tools .. decompose sata by ICA .. runica - ok [50-60min]
3. Select plot .. component maps .. 2D
4. In the Plot component scalp maps in 2D add the text: ','plotchans',[7:27]' to
in the 'Additional topoplot () options' field - ok
5. Save a copy of the file by selecting File - save
6. visually inspect data for ocular artifacts (refer to ICA_artifact_rejection.md)
7. Select plot - channel data (scroll) allows you to visualize recordings from
peri-ocular channels
8. Select PLot - component activations (scroll) allowing you to visualize the
time course of the ICA component(s) or in other words time when the artifact
occurred
9. select plot - component properties - then input '1:32' on 'component index to plot'
10. visually inspect each component for ocular artifacts
11. reject artifacts with ocular artifacts such as blinks by clicking on
accept - it will then turn red and say reject - ok
12. Finally remove artifacts/unwanted components by selecting tools - remove
components by data - plot single trials allowing you to see the change in your
data - black = before & red = after
