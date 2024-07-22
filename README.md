## Project Overview
This project focuses on time-domain audio separation using a modified U-Net (encoder-decoder) architecture. The goal is to separate different audio sources from a mixed audio signal, which has various applications such as noise reduction, music source separation, and enhancing audio quality for hearing aids. This work was conducted during my internship, where I researched and developed this model.

### Model Architecture
Modified U-Net (Encoder-Decoder)
The U-Net architecture, originally designed for image segmentation tasks, is adapted here for audio separation. The encoder-decoder structure allows the model to learn both global and local features of the audio signal, making it well-suited for source separation tasks.

### Separation Module
In the separation module of this model, a sequence of Convolutional Neural Networks (CNNs), Recurrent Neural Networks (RNNs), and feed-forward layers is applied to the input audio to achieve the most refined separation results. Each component of the module plays a crucial role in processing the audio signal:

CNN: Captures local patterns and features in the audio signal.
RNN: Models the temporal dependencies and dynamics of the audio signal.
Feed-Forward Layer: Refines the output by combining features learned by CNN and RNN.

### Dataset
The dataset used for training and testing the model consists of various audio samples with mixed sources. These samples are preprocessed to ensure compatibility with the model architecture.

