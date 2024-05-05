# BCI-research

### THE IDEA

- providing basic visual informations to complete blind peoples using ML and BCI
- ## 1. A life long learning ML model that decodes the user thoughts to Image

  - ### Detect brain waves using a non invasive device.
  - Two ways to do it
    - #### Electroencephalography (EEG):
      - EEG measures electrical activity in the brain using electrodes placed on the scalp.
      - EEG can capture brain activity in real-time, making it suitable for applications like brain-computer interfaces (BCIs) and neurofeedback.
    - #### Functional Magnetic Resonance Imaging (fMRI):
      - Provides much more efficient brain wave patterns than EEG but is costly and less portable.
  - ### Decode recorded brain waves to text.

    - [A review paper based on EEG Brain Signals to Text](https://arxiv.org/pdf/2405.00726)

    - #### Training the model or recording Brain wave as a training data set
      - user undergo training while their brain activity is recorded.
      - its like imagining a word. that is predicted by the model and corrects itself.
      - It analyzes the features in the new data and attempts to decode the intended text based on the learned patterns from the training dataset.

  - ### Text to image generation
    - There are many models that can generate images **DALL-E** , **GOOGLE'S BARD** , **MID JOURNEY**
    - Tuning these models to generate simplified images

- 2. a system that can convert images to electrical signal in a range suitable for optical lobe to visuilize images
- 3. create a way for feed back for this AI/ML models
