# AI Assisted Automatic Audio-visual and Face-to-Face Translation of Indic Languages

This repository contains resources and notebooks for audio-visual translation and dubbing, which translates videos from one language to another. Initially, the given original .mp4 video is processed and the audio is extracted from it using FFMPEG. The audio stream is probed and then mapped to a .wav file. The extracted audio is then fed into Google’s Speech Recognition API using Python’s Speech Recognition module or Wav2Vec2, where the source language is transcribed into text. The resulting text is translated using Google Translate Ajax API and is converted into a .wav audio format using various TTS libraries (Google’s gTTS and Microsoft’s SAPI5), and automatically synthesized into target language speech using Wav2Lip. The visual material is translated into the target language by synthesizing the speaker’s lip movements to match the translated audio. Lip sychronization processing is done by Wav2Lip, whose capabilities have been researched in terms how well it performs with Indic Languages such as Hindi and Tamil.

![image](https://github.com/thelonelyextrovert/avt-indic/assets/48013139/929f0f09-18d8-4b91-bb6f-e852c3d8db05)

You can find the app built from the demos [here](https://huggingface.co/spaces/capstonedubtrack/Indiclanguagedubbing)

You can find generated tts datasets with this system with the videodataroot files and results discussed in our paper (in progress) under results.

Examples of generated videos include:

https://github.com/thelonelyextrovert/avt-indic/assets/48013139/b2dbfeb6-1b66-4afe-91f8-dd87d57fbf52
Video translated from English to Tamil (included in videodataroot- tamil tts) with lip sync


https://github.com/thelonelyextrovert/avt-indic/assets/48013139/b383b6da-eeaf-4907-aeaf-688cd1d8ec1d
Untranslated English video (included in videodataroot- tts) with lip sync




