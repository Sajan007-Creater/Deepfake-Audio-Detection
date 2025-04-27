# Deepfake-Audio-Detection

Deepfake-Audio-Detection is an advanced tool designed to enhance security and authenticity in communications by accurately detecting and preventing the misuse of deepfake audio. It leverages state-of-the-art machine learning models to distinguish between genuine and AI-generated (deepfake) audio clips.

## Features
- Detects AI-generated (deepfake) audio with high accuracy
- Streamlit web interface for easy audio analysis and visualization
- Provides waveform plots and probability scores
- Command-line utilities for batch processing and evaluation
- Supports multiple audio formats (e.g., MP3)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sajan007-Creater/Deepfake-Audio-Detection.git
   cd Deepfake-Audio-Detection
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Web App (Streamlit)
Run the Streamlit app for an interactive interface:
```bash
streamlit run app.py
```
- Upload an audio file (MP3 format)
- Click "Analyze Audio" to view results, including probability of being a deepfake and waveform visualization

### Command-Line Utilities

#### 1. Evaluate a Batch of Audio Clips
```bash
python eval.py --eval_path <path_to_test.tsv> --output_path <output_directory> --preset <preset_name>
```

#### 2. Classify a Single Audio Clip
```bash
python is_this_from_tortoise.py --clip <path_to_audio_clip>
```

#### 3. Text-to-Speech Generation (for testing)
```bash
python do_tts.py --text "Your text here" --voice <voice_name> --output_path <output_directory>
```

#### 4. Read Longform Text
```bash
python read.py --textfile <path_to_text_file> --voice <voice_name> --output_path <output_directory>
```

## Example
- Upload an audio file via the web interface to get an instant deepfake probability score and waveform plot.
- Use the CLI tools for batch processing or automated pipelines.

## Requirements
- Python 3.8+
- torch
- torchaudio
- streamlit
- librosa
- plotly
- numpy
- scipy

All requirements can be installed via `pip install -r requirements.txt`.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for improvements, bug fixes, or new features.

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
