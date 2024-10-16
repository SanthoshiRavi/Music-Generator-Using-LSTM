# 🎶 Music Generation Using Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM)

## Project Overview
This project demonstrates music generation using Recurrent Neural Networks (RNN) with Long Short-Term Memory (LSTM) units. The model predicts key musical elements such as **pitch**, **step** (time between notes), and **duration**. It is trained using symbolic music data (MIDI files) and allows users to interact with various parameters to generate music.

## Features
- Generate musical notes with predicted **pitch**, **step**, and **duration**.
- Visualize music notes through a **piano roll**.
- Use histograms to display the **distribution** of generated features.
- Interactive controls allow customization of parameters like **number of notes** and **temperature**.
- Convert generated notes into MIDI files for playback.

## Technologies and Tools
- **TensorFlow & Keras**: Building and training the RNN and LSTM model.
- **PrettyMIDI**: For handling MIDI files.
- **Fluidsynth**: Synthesizing MIDI into audio for playback.
- **IPyWidgets**: Creating interactive UI components.
- **NumPy & Pandas**: Data manipulation and processing.
- **Matplotlib & Seaborn**: Visualizing the results with piano rolls and histograms.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/music-generation-rnn.git
    cd music-generation-rnn
    ```

2. **Install dependencies**:
    Make sure Python 3.7 or later is installed. Run:
    ```bash
    pip install -r requirements.txt
    ```

3. **Install Fluidsynth** (optional):
    ```bash
    sudo apt install -y fluidsynth
    ```

## Dataset
The model is trained using the **Maestro v2.0.0 MIDI Dataset**, a rich collection of MIDI files representing symbolic music data. The dataset is automatically downloaded and extracted during runtime.

## Usage

1. **Run the notebook**:
    Open the Jupyter notebook to train the model and generate music:
    ```bash
    jupyter notebook
    ```
    In the notebook, you can adjust parameters and generate music interactively.

2. **Interactive Music Generation**:
    Users can customize:
    - **Temperature**: Controls the randomness of generated notes.
    - **Number of Notes**: Defines how many notes to generate.
    - **Instrument**: Choose from instruments like Piano, Violin, etc.

3. **Music Playback**:
    The generated music is saved as a MIDI file and can be played back using the `Fluidsynth` synthesizer.

## Screenshots
- **Model Architecture**:
    ![Model Architecture](path-to-model-architecture.png)
  
- **Piano Roll**:
    ![Piano Roll](path-to-piano-roll.png)

- **True vs Predicted Pitch**:
    ![True vs Predicted Pitch](path-to-true-predicted-pitch.png)

## Results and Evaluation
- The model performed well in predicting **step** and **duration** with low error rates, but **pitch prediction** accuracy requires improvement.
- Evaluation metrics and plots, such as the **true vs predicted pitch** plot and distribution histograms, are available in the notebook.

## Future Work
- Improve the model’s ability to predict **pitch**.
- Incorporate additional musical elements like **chords** and **dynamics**.
- Develop a more comprehensive user interface for real-time music composition.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
