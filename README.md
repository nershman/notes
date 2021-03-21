# notes
This document came about as a way to better organize my starred repos. 

## sounds/music  stuff
### Pitch - Shifting

* [SoundTouch Audio Processing](https://gitlab.com/soundtouch/soundtouch/-/blob/master/include/SoundTouch.h) - the main file for audacity's pitch-shifting functionalities.
  - pitch-shifting is done by using a combination of rate-change and tempo-change. I think "anti-aliasing" tries to smooth over the resulting choppiness of tempo changes. Tempo change method is simple granular synthesis type technique.

* [AudioFFT by robersiegel](https://github.com/robertsiegel/AudioFFT) - implementation of pitch shifting using fast fourier transforms.
* [same thing implemented in C](https://sites.google.com/site/mikescoderama/pitch-shifting) and an [explanation of STFT (short time fourier transform](http://blogs.zynaptiq.com/bernsee/pitch-shifting-using-the-ft/)
    * step 1: cut sample into grains s.t. grains are relatively stationary.
    * ???
    * measure "partial frequencies" of grains. ( I believe this is the decomposition / finite fourier series)
    * scale the frequencies (these are sine waves so you are just generating new size wave at relative different frequency and relative position to other frequencies)
    * "We also see why pitch shifting using this procedure automatically includes anti-aliasing: we simply do not compute bins that are above our Nyquist frequency by stopping at fftFrameSize2. This does not even need an additional processing step."

* https://www.youtube.com/watch?v=WGYVOSFqcGY
* https://github.com/juandagilc/Audio-Effects

note: windows and grains are different... need to lookmore into it.



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
* 

## Various Utlities I Should...
### Use
* [Pomodoro for Taskwarrior](https://github.com/coddingtonbear/taskwarrior-pomodoro)
* [Python code formatter: black](https://github.com/psf/black)
* [Python code formatter; yapf](https://github.com/google/yapf)
* [OSX Audio Utility: individual vol controls](https://github.com/kyleneideck/BackgroundMusic)
* [zrythm open source DAW :o ](https://github.com/zrythm/zrythm)
* [beets music library manager](https://github.com/beetbox/beets)
* [extend android battery life](https://github.com/VR-25/acc)

### Not forget I like
* https://github.com/jbarlow83/OCRmyPDF
* https://github.com/ankitects/anki

## FDA
* https://github.com/GAA-UAM/scikit-fda
* http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones


## datasets
### network analysics
http://konect.cc/networks/hiv/
