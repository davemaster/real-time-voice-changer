# realtime-voice-accent-improvement

### An attempt to improve some videos voice audio accent in english language; at realtime

[![audio improvement copy](https://github.com/user-attachments/assets/e3498928-a7cb-41c4-8034-27ed87342a33)](https://youtu.be/NERoC7uPx3U)

How many times, we found marvelouns information on video, but, BUT, when we start to see that media, KAPUT, the voice audio accent destroys ours ears; that's not meaning I have a great accent, in English Language, maybe for those with those accents, WE HAVE THE WORST... but, I want to AI and NVIDIA Workbench comes to rescue MY DAMAGED EARs, period. 

No body was hurt in the making of this project.

## Running the TTS Server
I will run this project, using a notebook into the jupyter lab environment provided by Nvidia AI Workbench. 

From there, I will call the [coqui-ai TTS server](https://github.com/coqui-ai/TTS/tree/dev?tab=readme-ov-file#installation), running from docker. How? I show You in details, with images or better, a Video about [HOW TO run the TTS Server from docker](https://github.com/coqui-ai/TTS/tree/dev?tab=readme-ov-file#docker-image).

1. docker run --rm -it -p 5002:5002 --entrypoint /bin/bash ghcr.io/coqui-ai/tts-cpu              #pull the server (if you don't have it) and then run in port 5002
2. python3 TTS/server/server.py --list_models                                                    #To get the list of available models
3. python3 TTS/server/server.py --model_name tts_models/en/vctk/vits                             # To start a server --mmodel_name tts_models/en/vctk/vits (the name of the model you're going to use from 2.

[![voice_changer_002-TTS Sever copy](https://github.com/user-attachments/assets/39aa7cd5-9454-4dd2-a9b8-5c034fdd320b)](https://youtu.be/ghJ44dYc33k)


## Install TTS into the jupyter lab NVIDIA AI Workbench 

Just run pip install TTS from a notebook, or add packacge from the windows within NIVIDA AI Workbench: Package, Add, select pip, then put TTS


