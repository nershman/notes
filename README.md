# notes
This is just a personal document for specific pages of repos I'm interested in


* [SoundTouch Audio Processing](https://gitlab.com/soundtouch/soundtouch/-/blob/master/include/SoundTouch.h) - the main file for audacity's pitch-shifting functionalities.
  - pitch-shifting is done by using a combination of rate-change and tempo-change. I think "anti-aliasing" tries to smooth over the resulting choppiness of tempo changes. Tempo change method is simple granular synthesis type technique.
