## Description:
TL;DR: Lets the bot answer you with a picture!  

Stable Diffusion API pictures for TextGen, v.1.1.0  
An extension to [oobabooga's textgen-webui](https://github.com/oobabooga/text-generation-webui) allowing you to receive pics generated by [Automatic1111's SD-WebUI API](https://github.com/AUTOMATIC1111/stable-diffusion-webui)

<details>
<summary>Interface overview</summary>

![Interface](https://raw.githubusercontent.com/Brawlence/texgen-webui-SD_api_pics/main/illust/Interface.jpg)

</details>

Load it in the `--chat` or `--cai-chat` mode with `--extension sd_api_pictures` alongside `send_pictures` (it's not really required, but completes the picture, *pun intended*).  

The image generation is triggered either:  
- manually through the 'Force the picture response' button while in Manual or Interactive modes OR  
- automatically in Immersive/Interactive mode if the words `'send|main|message|me'` are followed by `'image|pic|picture|photo|snap|snapshot|selfie|meme'` in the user's prompt  
- always on in Picturebook/Adventure mode (if not currently suppressed by 'Suppress the picture response')  

## Prerequisits

One needs an available instance of Automatic1111's webui running with an `--api` flag. Ain't tested with a notebook / cloud hosted one but should be possible.   
To run it locally in parallel on the same machine, specify custom `--listen-port` for either Auto1111's or ooba's webUIs.  

## Features:
- API detection (press enter in the API box)  
- VRAM management (model shuffling)  
- Three different operation modes (manual, interactive, always-on)  

The model input is modified only in the interactive mode; other two are unaffected. The output pic description is presented differently for Picture-book / Adventure mode.  

Connection check:  
![API-check](https://raw.githubusercontent.com/Brawlence/texgen-webui-SD_api_pics/main/illust/API-check.gif) 

---

## Demonstrations:

Those are examples of the version 1.0.0, but the core functionality is still the same

<details>
<summary>Conversation 1</summary>

![EXA1](https://user-images.githubusercontent.com/42910943/224866564-939a3bcb-e7cf-4ac0-a33f-b3047b55054d.jpg)
![EXA2](https://user-images.githubusercontent.com/42910943/224866566-38394054-1320-45cf-9515-afa76d9d7745.jpg)
![EXA3](https://user-images.githubusercontent.com/42910943/224866568-10ea47b7-0bac-4269-9ec9-22c387a13b59.jpg)
![EXA4](https://user-images.githubusercontent.com/42910943/224866569-326121ad-1ea1-4874-9f6b-4bca7930a263.jpg)


</details>

<details>
<summary>Conversation 2</summary>

![Hist1](https://user-images.githubusercontent.com/42910943/224865517-c6966b58-bc4d-4353-aab9-6eb97778d7bf.jpg)
![Hist2](https://user-images.githubusercontent.com/42910943/224865527-b2fe7c2e-0da5-4c2e-b705-42e233b07084.jpg)
![Hist3](https://user-images.githubusercontent.com/42910943/224865535-a38d94e7-8975-4a46-a655-1ae1de41f85d.jpg)

</details>

