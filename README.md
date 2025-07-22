# astrial_whisper

This repositories contains cross-compiled libraries that are necessary to execute the [*speech_recognition*](https://github.com/hailo-ai/Hailo-Application-Code-Examples/tree/main/runtime/hailo-8/python/speech_recognition) application on the System Electronics Astrial board.

## Instructions
- Download the package cross-compiled for your OS version from the Releases section, for example:
  ```
  curl -LO https://github.com/topper-ai/astrial_whisper/releases/download/astrial-v1.1.4/astrial-v1.1.4.zip
  ```
- Extract the files, copy the libraries to the */usr/lib/* and the *FFmpeg* binaries to the */usr/bin* folder
- Verify that FFmpeg is working
  ```
  ffmpeg
  ```
- Install the [*speech_recognition*](https://github.com/hailo-ai/Hailo-Application-Code-Examples/tree/main/runtime/hailo-8/python/speech_recognition) application as per instructions.
- If you do not see the *app/hef* folder, please change the interpreter in *app/download_resources.sh* and run the script to download the resources again.
- Run the app as per instructions.  
  **Note**: initialization on the Astrial may take tens of seconds, due to the Python libraries being imported. 

## Additional notes
If using a microphone that does not support 16 KHz sampleing frequency, please modify the *SAMPLE_RATE* value in *record_utils.py* (if using the CLI) or in *gui.py* (if using the GUI) with a frequency value that is supported by your microphone. Do **not** modify the value in *audio_utils.py*, which must be set to 16 KHz.

## Licensing of Included Libraries

This release includes the following third-party libraries:

- **FFmpeg**: Licensed under the [LGPL/GPL](https://ffmpeg.org/legal.html). See `LICENSES/ffmpeg.LICENSE`.
- **PortAudio**: Licensed under the [MIT License](http://www.portaudio.com/license.html). See `LICENSES/portaudio.LICENSE`.

If required, source code for FFmpeg can be provided upon request or obtained from [FFmpeg.org](https://ffmpeg.org).
