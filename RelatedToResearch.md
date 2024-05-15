5-9-24 4:57 am

- #### What are the specific techniques used to decode text from EEG brain signals?

  - Coherence: This technique measures the degree of correlation between the activities of different brain regions in the frequency domain, providing insights into the functional relationships and synchronization patterns between various regions.

  - Phase synchronization: This evaluates the temporal alignment of neural oscillations across different regions, revealing intricate patterns of neural communication crucial for cognitive and motor functions.

  - Deep neural networks: Specifically, recurrent neural networks (RNNs) and Long Short-Term Memory (LSTM) networks have demonstrated significant potential in decoding EEG signals into text.

  - Bidirectional Auto-Regressive Transformers (BART): Known for its effectiveness in natural language processing tasks, BART is being adapted to interpret and convert EEG signals into text.

- #### What are the challenges in EEG Signal Decoding for Text Generation ?

  - acquiring proper brain wave data :
    - acquiring clean and proper brain wave data is crucial for efficient thought to text genegration
    - ###### problems are:
      - EEG waves are non stationary i.e. they frequently tend to change, extracting features and information from this changing waves is challenging.
      - EEG waves are high dimensional and constains redunt information cleaning this is a complex task.
      - calibrating EEG device to individual user is essential for accurately decoding neural signals is time consuming.
      - training data is limited.
      - privacy concerns related to the user advance encryptions are required to protect the data.

- #### is there any currently availabel models that can decdode thought to text?
- yes

  - Raw Wave: The process begins with the collection of raw EEG signals, which are the electrical activities recorded from the scalp representing brain activity.

  - Band Filter: The raw EEG data is then passed through band-pass filters. These filters are used to eliminate noise and retain only those frequency bands that are relevant to the task, such as the alpha, beta, gamma, delta, and theta waves, each associated with different brain activities.

  - Eye Fixation Sliced Waves: In parallel with band filtering, the model focuses on specific segments of the EEG signals that correspond to moments when the eyes are fixated on certain points. These slices of data are considered significant because they could be closely related to cognitive processes during reading or looking at texts.

  - Transformer: The filtered EEG signals and the eye fixation sliced waves are then fed into a Transformer. The Transformer is a type of deep learning model that has been highly successful in various natural language processing tasks. It can handle sequential data and is adept at capturing complex relationships within the sequence of brain signal inputs.

  - Projection Layer: After processing the signals through the Transformer, the output is passed through a projection layer, the complex features extracted by the another Transformer into a simpler representation that can be used for classification or regression tasks.

  - Discrete Codex: The output from the projection layer is then represented as discrete codes. These codes are likely symbolic representations of the decoded brain signals, which have been mapped to elements of written language.

  - Gradients: The gradients, which are computed during the training of the model, are used to update model weights, minimizing the difference between the predicted text and the actual text. This optimization process is crucial for model learning and improving accuracy over time.

  - Output: Finally, the decoded discrete codex is translated into a human-readable output, which is the text representation of the thought or intended message originally represented within the EEG signals.
    ![model of a DE WAVE Model](./images/de-wave.png)
