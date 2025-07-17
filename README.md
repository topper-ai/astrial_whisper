# astrial_whisper

This repositories contains cross-compiled libraries that are necessary to execute the [*speech_recognition*](https://github.com/hailo-ai/Hailo-Application-Code-Examples/tree/main/runtime/hailo-8/python/speech_recognition) application on the System Electronics Astrial board.

## Instructions
- Download the package cross-compiled for your OS version from the Release section:
  ```
  wget https://github.com/<user>/<repo>/releases/download/v1.0/release-v1.0.tar.gz
  ```
- Extract the files and copy them to the /usr/lib/ folder
- Install the [*speech_recognition*](https://github.com/hailo-ai/Hailo-Application-Code-Examples/tree/main/runtime/hailo-8/python/speech_recognition) application as per instructions.

## Licensing of Included Libraries

This release includes the following third-party libraries:

- **FFmpeg**: Licensed under the [LGPL/GPL](https://ffmpeg.org/legal.html). See `LICENSES/ffmpeg.LICENSE`.
- **PortAudio**: Licensed under the [MIT License](http://www.portaudio.com/license.html). See `LICENSES/portaudio.LICENSE`.

If required, source code for FFmpeg can be provided upon request or obtained from [FFmpeg.org](https://ffmpeg.org).
