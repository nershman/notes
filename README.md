# notes
My Stars. I try to organize them in this sheet or one of the other files in this repo.

## sounds/music  stuff

### Idea Sparks
* https://github.com/hwpoison/audio-transcode-stream-flask realtime transcoding.


### Pitch - Shifting

* [SoundTouch Audio Processing](https://gitlab.com/soundtouch/soundtouch/-/blob/master/include/SoundTouch.h) - the main file for audacity's pitch-shifting functionalities.
  - pitch-shifting is done by using a combination of rate-change and tempo-change. I think "anti-aliasing" tries to smooth over the resulting choppiness of tempo changes. Tempo change method is simple granular synthesis type technique.

* [AudioFFT by robersiegel](https://github.com/robertsiegel/AudioFFT) - implementation of pitch shifting using fast fourier transforms.
    *   Use [Hanning Windows](https://numpy.org/doc/stable/reference/generated/numpy.hanning.html) to create grains
    *   doesn't run  at all, its essentially pseudocode :)
    *   todo: try to make it run :))
* [same thing implemented in C](https://sites.google.com/site/mikescoderama/pitch-shifting) and an [explanation of STFT (short time fourier transform](http://blogs.zynaptiq.com/bernsee/pitch-shifting-using-the-ft/)
    * step 1: cut sample into grains s.t. grains are relatively stationary.
    * ???
    * measure "partial frequencies" of grains. ( I believe this is the decomposition / finite fourier series)
    * scale the frequencies (these are sine waves so you are just generating new size wave at relative different frequency and relative position to other frequencies)
    * "We also see why pitch shifting using this procedure automatically includes anti-aliasing: we simply do not compute bins that are above our Nyquist frequency by stopping at fftFrameSize2. This does not even need an additional processing step."

* https://www.youtube.com/watch?v=WGYVOSFqcGY
* https://github.com/juandagilc/Audio-Effects


### Auto-Tune

* [implementation in C](https://github.com/dot-operator/Auto-Tuner)

* [implementation in python & C](https://github.com/ederwander/PyAutoTune) which is based on http://tombaran.info/autotalent.html (which seems to have more interesting singal processing toys)

### Generative Music

* https://github.com/jisungk/deepjazz
* https://github.com/omgimanerd/markov-music
* https://github.com/calclavia/DeepJ
* https://github.com/ybayle/awesome-deep-learning-music


### Formants

http://formantbros.jp/activity/

* [Nobuyasu Sakonda's Max patches](http://formantbros.jp/sako/download.html)

### Misc
* [Neural Wavetable Synthesizer](https://github.com/RichardYang40148/Neural_Wavetable_Synthesizer)
* https://github.com/despoisj/DeepAudioClassification
* [Piano Transcription to MIDI](https://github.com/bytedance/piano_transcription) uses Pytorch to transcribe sound to MIDI. I am assuming this functions in a more interesting way that whatever online MIDI converters do.
*  https://github.com/electro-smith/DaisySP
*  https://github.com/magenta/mt3
*  https://github.com/hwpoison/audio-transcode-stream-flask
*  https://github.com/tyiannak/pyAudioAnalysis


## Image Processing
* https://github.com/axu2/image-quilting
* https://github.com/andrewdcampbell/seam-carving
* https://github.com/axu2/improved-seam-carving

## Various Utlities I ...
### Should Use
* [Pomodoro for Taskwarrior](https://github.com/coddingtonbear/taskwarrior-pomodoro)
* [Python code formatter: black](https://github.com/psf/black)
* [Python code formatter; yapf](https://github.com/google/yapf)
* [OSX Audio Utility: individual vol controls](https://github.com/kyleneideck/BackgroundMusic)
* [zrythm open source DAW :o ](https://github.com/zrythm/zrythm)
* [beets music library manager](https://github.com/beetbox/beets)
* [extend android battery life](https://github.com/VR-25/acc)

### Use / Like
* https://github.com/jbarlow83/OCRmyPDF
* https://github.com/ankitects/anki
* https://github.com/ActivityWatch/activitywatch
* https://github.com/kawaiiDango/pScrobbler

## FDA
* https://github.com/GAA-UAM/scikit-fda
* http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones


## Data
### Scrapers
 * [Colly: framework for collecitng structured data in Golang](https://github.com/gocolly/colly)

### Datasets: network analysics
http://konect.cc/networks/hiv/

### Datasets: Misc
 * [crowdsourced annotated dash cam photos](https://github.com/commaai/comma10k)

## Research Intern 
* https://github.com/MartinThoma/lidtk
  * CLD2 is the one we're interested in using. it's licensed by apache and this package implements the C++ library by making a python wrapper for the java wrapper for the c++???
  * other wrappers for CLD2.
    * https://github.com/aboSamoor/pycld2 probably will use this one.
 
* https://pypi.org/project/langdetect/ in case lidtk isnt usable.


## Misc General

### Cool C+= Projects 
* https://github.com/CLD2Owners/cld2 categorizes langauges suing probaiblities and letter sequences !
