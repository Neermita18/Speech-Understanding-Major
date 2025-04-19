# Speech Understanding Major

This repository contains the code, transcripts, and results for my Speech Understanding Major consisting of three main components:

1. **Multilingual Speech Processing** - Transcription, translation, and audio generation in a low-resource language
2. **Audio Denoising and Transcription** - Analysis and enhancement of moderator speech in noisy environments
3. **Research on Multimodal Deception Detection** - Analysis of the next frontier in speech understanding


## Structure

```
.
├── B22CS092_Major.pdf                       # Final comprehensive report
├── B22CS092_Neermita_Q1_SU_Major.ipynb      # Jupyter notebook for Question 1
├── B22CS092_Neermita_Q2_SU_Major.ipynb      # Jupyter notebook for Question 2
├── base_transcript.txt                      # Original transcript from Google Cloud STT (used as reference) for Question 1 
├── bengali_with_my_voice.mp3                # Generated Bengali audio with custom voice for Question 1
├── clean_transcriptions.txt                 # Cleaned transcripts for Question 2 (no noise)
├── cleaned_base_transcript.txt              # Processed and cleaned Google Cloud STT transcript (used as reference) for Question 1
├── cleaned_lecture_transcript.txt           # Processed and cleaned lecture transcripts from Whisper for Question 1 
├── lecture_transcript.txt                   # Original lecture transcript from Whisper for Question 1 
├── ss_transcriptions.txt                    # Spectral subtraction transcriptions for Question 2
├── temp_bengali_tts.mp3                     # Temporary Bengali Google TTS output for Question 1 
└── w_transcriptions.txt                     # Wiener filter transcriptions for Question 2
```

## Question 1: Multilingual Speech Processing

### Description
This component involved transcribing a lecture with code-switched English and Hindi content, removing filler words, and generating audio in Bengali (a low-resource language) using a custom voice.

### Features
- Accurate transcription of code-switched content (English-Hindi)
- Automatic removal of filler words for improved clarity
- Translation to Bengali, a low-resource language
- Custom voice synthesis using speech features and TTS models

### Technologies Used
- Whisper for initial transcription
- Google Cloud Speech-to-Text for verification
- Custom preprocessing pipeline for filler word removal
- Google TTS system for Bengali voice generation

### Results
- Successfully generated high-quality Bengali audio with natural voice characteristics
- Evaluated using Mean Opinion Score (MOS) and Word Error Rate (WER) metrics
- Achieved clean transcriptions with removed filler words

## Question 2: Audio Denoising

### Description
This component focused on analyzing audio recordings from various events, designing and implementing denoising algorithms to enhance moderator speech clarity, and evaluating the performance of different approaches.

### Features
- Comprehensive noise level analysis of different events
- Implementation of 2 denoising algorithms
- Transcription of cleaned audio for evaluation
- Comparative analysis of denoising methods

### Technologies Used
- Spectral subtraction for baseline denoising
- Wiener filtering for advanced noise removal
- Google STT for transcription of denoised audio and clean audio for comparison

### Results
- Quantitative evaluation using Signal-to-Noise Ratio (SNR) improvement and PESQ scores
- Subjective assessment with Mean Opinion Score (MOS)
- Transcription accuracy measured using Word Error Rate (WER) and Character Error Rate (CER)

## Question 3: Research on Multimodal Deception Detection

### Description
This component presents original research on the possible novel challenge in Speech Understanding: Multimodal Deception Detection in Conversational Speech (MDDCS).

### Key Contributions
- Identification of a critical gap in current speech understanding systems
- Proposal of a novel architecture: Contextual Fusion Network for Deception Detection (CFN-DD)
- Detailed algorithm design integrating linguistic, acoustic, and visual modalities
- Comprehensive evaluation strategy with specialized metrics

### Methodology
- Multimodal approach combining speech, facial expressions, and body language
- Cultural calibration to account for cultural variations in deception markers
- Baseline behavior modeling for personalized analysis
- Confidence estimation for reliable decision making

### Potential Impact
- Scientific advancement in understanding cognitive and linguistic mechanisms of deception
- Commercial applications in security, fraud detection, and information verification
- Societal benefits in criminal investigations and public discourse integrity

## Installation and Usage

### Setup
1. Clone this repository
   ```
   git clone https://github.com/Neermita18/speech-understanding-project.git
   cd speech-understanding-project
   ```

3. Configure API credentials
   ```
   export GOOGLE_APPLICATION_CREDENTIALS="path/to/your/credentials.json"
   ```

### Running Question 1
```
jupyter notebook B22CS092_Neermita_Q1_SU_Major.ipynb
```

### Running Question 2
```
jupyter notebook B22CS092_Neermita_Q2_SU_Major.ipynb
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Speech Understanding course instructors for guidance
- Google Cloud for API access
- OpenAI for Whisper model
