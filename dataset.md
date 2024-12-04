https://www.kaggle.com/datasets/naddamuhhamed/sleepy-driver-eeg-brainwave-data/data

---

# About Dataset

## Description

We collected EEG signal data from 4 drivers while they were awake and asleep using NeuroSky MindWave sensor. For safety precautions they weren't actually driving while acquiring the signals. Each driver wore the helmet for 5-8 minutes for each label (sleepy, not sleepy) and the signals are acquired approximately every second. The signals are measured in units of microvolts squared per hertz (μV²/Hz). This is a measure of the power of the EEG signal at a particular frequency.

The high values that you are seeing are likely due to the fact that the MindWave sensor is only measuring EEG data from a single location on the forehead. This is in contrast to medical-grade EEG devices, which typically use multiple electrodes placed on different parts of the scalp.

## Methodology

The driver would wear the [NeuroSky MindWave](https://store.neurosky.com/pages/mindwave) headset connected by a USB stick to the laptop and we would collect EEG signals from their brain. The NeuroSky mindwave headset is a single channel headset that measures the voltage between an electrode resting on the frontal lobe (forehead) and two electrodes (one ground and one reference) each in contact with one earlobe. The drivers were instructed to be awake or asleep and their EEG signals were recorded accordingly.

## Content

Attention and meditation are calculated from the headset itself, we didn't consider it a reliable feature.
All EEG signals are divided and specified by the headset. There was no signal preprocessing done.

## Inspiration

This dataset was made for our graduation project. We got an A- (90%).
Our highest accuracy was 82%, hopefully you can do even better.
I thought about uploading this dataset since we worked hard on it and it's a waste seeing it idle after we got our grade so hopefully other people might find it useful too!

## More references

here is our [proposal](https://drive.google.com/file/d/1n70BcMPvtGzscGGgcBA8ruXdO0AuEr_v/view?usp=sharing) document. The similar systems section would be very useful
you will find some results at the end of the document they were used using [this](https://www.kaggle.com/datasets/wanghaohan/confused-eeg) dataset as it used the same helmet as ours although not the same classification and that's why we got poor results but it was for a start

# About `acquiredDataset.csv`

= collected dataset and its classification

## Columns

**attention**
Proprietary measure of mental focus from 0-100

**meditation**
Proprietary measure of calmness from 0-100

**delta**
1-3 Hz of power spectrum

**theta**
4-7 Hz of power spectrum

**lowAlpha**
Lower 8-11 Hz of power spectrum

**highAlpha**
Higher 8-11 Hz of power spectrum

**lowBeta**
Lower 12-29 Hz of power spectrum

**highBeta**
Higher 12-29 Hz of power spectrum)

**lowGamma**
Lower 30-100 Hz of power spectrum

**highGamma**
Higher 30-100 Hz of power spectrum

**classification**
whether driver is sleepy
