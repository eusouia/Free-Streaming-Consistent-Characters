# Free-Streaming-Consistent-Characters
[FREE WORKFLOWS] Create your own CONSISTENT characters with AI!
The Flux Consistent Characters workflow, created by Mickmumpitz, is a powerful ComfyUI tool that maintains the consistency of AI-generated characters across multiple outputs. Ideal for AI-driven cinematics, children’s books, or any project that requires stable character appearances, this Flux-based workflow simplifies the process of achieving consistent character appearances, reducing the need for multiple prompts and fine-tuning. 
Mickmumpitz developed the Flux Consistent Characters workflow and shared a detailed tutorial on his YouTube channel. While the workflow and environment setup are provided here for convenience, Mickmumpitz deserves full credit for creating this effective Flux-based Consistent Characters solution. Install Custom Node Request [FREE WORKFLOWS] Create your own CONSISTENT characters with AI! Free stream consistent characters. 

Attachments
https://www.patreon.com/posts/free-workflows-113743435

----------------------------------------------------------------------------------------------------------------------------------
[FREE GUIDE] Mickmumpitz Character Sheets with FLUX and SDXL

1 Install ComfyUI

Download ComfyUI: https://github.com/comfyanonymous/ComfyUI
Extract the folder to the location where you want to install ComfyUI.
install git https://git-scm.com/download/win
standalone version
Download ComfyUI Manager: https://github.com/ltdrdata/ComfyUI-Manager
Extract it, put it into your ComfyUI directory and run it.
After it’s done you can run ComfyUI by clicking run_nvidia_gpu

Congratulations, you installed ComfyUI! 🥳 To use my workflows you’ll need some extra models and extensions, but it is super easy to install them!

In the next step I’ll show you where to get and put the models. If you’re having issues check if you can just install them via the ComfyUI Manager. Just search for them and when you click “Install” they will be put in the right directory. 

2 Character Sheets with SDXL

Get the workflow here 👉 https://www.patreon.com/posts/free-workflows-113743435
Drag and drop the .json into your ComfyUI Interface.
Go to ComfyUI Manager > Install missing custom nodes > install all of them > Restart ComfyUI

If you have problems with the Flux workflow, make sure you are using the latest version of the workflow! (v05)

Download the Models:

Download these models and put them in the corresponding folders:

Checkpoint: https://civitai.com/models/293331/wildcardx-xl-turbo

📁 ComfyUI_windows_portable\ComfyUI\models\checkpoints

!
You can also use any other SDXL checkpoints for all the workflows. I recommend Turbo or lightning ones though for faster generation time especially for the video workflows. You can find more models on CivitAI.com. Check the example images for the settings and match them in your KSampler!



SDXL CONTROLNET: https://huggingface.co/thibaud/controlnet-openpose-sdxl-1.0/tree/main
(OpenPoseXL2.safetensors)

and: https://huggingface.co/TheMistoAI/MistoLine/tree/main
(mistoLine_rank256.safetensors) <- For the Advanced version! 

📁 ComfyUI_windows_portable\ComfyUI\models\controlnet\sdxl 

UPSCALE MODEL: https://openmodeldb.info/models/4x-ClearRealityV1

📁 \ComfyUI_windows_portable\ComfyUI\models\upscale_models

3 Create Character Sheets with FLUX 

Get the workflow here 👉https://www.patreon.com/posts/free-workflows-113743435

!
Check out the official FLUX Installation guide for ComfyUI here: 
https://comfyanonymous.github.io/ComfyUI_examples/flux/


Drag and drop the .json into your ComfyUI Interface.
Go to ComfyUI Manager > Install missing custom nodes > install all of them > Restart ComfyUI
This should install “ComfyUI-eesahesNodes” from ComfyUI manager (contains InstantXFluxUnionControlNetLoader)

MODEL https://huggingface.co/black-forest-labs/FLUX.1-dev/tree/main
flux1-dev.safetensors or https://huggingface.co/black-forest-labs/FLUX.1-schnell/tree/main

📁 ComfyUI_windows_portable\ComfyUI\models\unet

CLIP  https://huggingface.co/comfyanonymous/flux_text_encoders/blob/main/clip_l.safetensors
and
https://huggingface.co/comfyanonymous/flux_text_encoders/blob/main/t5xxl_fp16.safetensors

📁 ComfyUI_windows_portable\ComfyUI\models\clip

VAE https://huggingface.co/black-forest-labs/FLUX.1-schnell/blob/main/ae.safetensors

📁 ComfyUI_windows_portable\ComfyUI\models\vae

CONTROLNET MODEL: https://huggingface.co/InstantX/FLUX.1-dev-Controlnet-Union/tree/main 

You can get the models via the ComfyUI Manager:


You can also use the ShakkerLabs models, which are meant to be newer and improved versions of InstantX. Though in my testing, I actually got better results with InstantX.

https://huggingface.co/Shakker-Labs/FLUX.1-dev-ControlNet-Union-Pro/tree/main

UPSCALE MODEL: https://openmodeldb.info/models/4x-ClearRealityV1

📁 \ComfyUI_windows_portable\ComfyUI\models\upscale_models

4 Training a LORA

For Training I recommend using FluxGym via Pinokio. 

You can also train Loras online via Replicate for example. Cost 2-5 Dollars for one Lora.
