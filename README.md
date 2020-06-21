# Speech-Recognition

My basic try on speech recognition using speech recognition library and google speech recogniton API(Not the Google cloud API) which provides free 50 daily pings.

The following python libraries have been used :
1. Speech recognition
2. pydub
3. PyAudio (if you want to use your Microphone)

Note : pydub requires ffmpeg in the environment to run, so install ffmpeg and include it in system path first.

The program has two modes:
1. Reading from an audiofile.
2. Reading user input through mic.

Speech recognition library supports only .wav, .aiff, .aiff-c and .flac(native flac format only, ogg-flac isnt supported) file types only so I have included the pydub library which calls ffmpeg for filetype conversion into .wav format.
If you have some noise in your audio try uncommenting the **adjust_for_ambient_noise** function in the program and play with the duration parameter to adjust whats best(it will occur in the interval 0.5 to 1 for most audios).
The paragraph converted in the .ipynb is the new.wav file (courtesy of my gf) and predicts the speech quite accurately.   
