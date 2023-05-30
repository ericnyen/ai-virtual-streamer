# ai-virtual-streamer

Simple script used to read chat messages from Youtube live chat and OpenAI's GPT-3 language model to generate responses. The output from GPT-3 is then read out loud using a Text-to-Speech engine (Eleven Labs).

# Setup
Install Dependencies
```
pip install -r requirements.txt
```
You will also need to install [`ffmpeg`](https://ffmpeg.org/)

# Usage

Edit the variables 'El_key' and 'OAI_key' in 'config.json'

`EL_key` is the API key for [ElevenLabs](https://beta.elevenlabs.io/). Found in Profile Settings

`OAI_key` is the API key for OpenAI. Found [here](https://platform.openai.com/account/api-keys)

Then run `run.py`

### Default TTS
```
python run.py -id STREAMID 
```
### Elevenlabs TTS
```
python run.py -id STREAMID -tts EL 
```
## Notes
Replace `STREAMID` with the stream's ID that you can find on the Youtube Stream link

You can change the voice by changing `voice` in `config.json`. You can find the ID's [here](https://api.elevenlabs.io/docs) in `Get Voices`

# Other
I used [This VTS plugin](https://lualucky.itch.io/vts-desktop-audio-plugin) and [VB Audio cable](https://vb-audio.com/Cable/) to make her mouth move and be able to play music at the same time
