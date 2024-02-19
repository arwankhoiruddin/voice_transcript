# Introduction

In this project, our goal is to convert WAV audio files into speech. Here's our approach:

* Silence Detection: We begin by detecting silent regions within the WAV audio file. These silent regions serve 
as potential points to split the audio into smaller segments.

* Splitting the WAV: Using the detected silent regions, we segment the WAV audio file into smaller chunks. Each 
chunk is delineated by periods of silence.

* Speech Recognition: With the audio split into manageable chunks, we apply speech recognition techniques to 
transcribe the speech contained within each segment.

By implementing these steps, we enable the conversion of WAV audio into textual speech output, facilitating 
further processing and analysis of the audio content.


# Running code

* Open `jupyter notebook` and open `mp4 transcript.ipynb`
* Install the required libraries: `pip install speech_recognition` and `pip install pydub`
* Run cells in the notebook. It will create some wav chunks and provide the output


# Video source

Alan Watts - The Dream of Life (No Music): https://www.youtube.com/watch?v=npgVq7-Fioo&t=51s


# Results

For `watts_cropped.wav`, it will produce following outputs:

```
Chunk 1 Text: let's suppose that you were able every night to dream Any Dream you wanted to
Chunk 2 Text: 75 years of time or any length of time you wanted to have
Chunk 3 Text: and you would naturally as you began on this adventure of dreams you would fulfill all your
Chunk 4 Text: 75 years of total pleasure each you would say wow that was pretty great
```


# Limitations

This code works only on `no music` audio. Need to do more pre processing for audio with music
