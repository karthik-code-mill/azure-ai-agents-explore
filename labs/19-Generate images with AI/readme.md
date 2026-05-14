# Image generation with AI using Model  FLUX-1.1-pro

This product show cases the capability to use azure congnitive server to be able to deploy LLm model & image-generation client for the Azure OpenAI / OpenAI Images API.

The main script, `image-client.py`, prompts the user for text input, sends that prompt to the deployed image generation model, decodes the returned base64 image payload, and saves the resulting PNG file to the `images/` directory.

## Key features

- Uses `dotenv` to load `ENDPOINT` and `MODEL_DEPLOYMENT` from environment settings.
- Authenticates via Azure AD using `DefaultAzureCredential` and a bearer token provider.
- Generates one image per prompt and stores it locally as `image_1.png`, `image_2.png`, etc.

## Environment

This project is shown running with:

```
Python 3.13.12
```

## Folder contents

```
images
labenv
env
image-client.py
readme.md
requirements.txt
```

## Usage

1. Install the required packages from `requirements.txt`.
2. Set the `ENDPOINT` and `MODEL_DEPLOYMENT` variables in a `.env` file.
3. Run `python image-client.py` and enter prompts to generate images.

<img width="1024" height="1024" alt="image_1" src="https://github.com/user-attachments/assets/cfdf48ba-5385-4809-b10a-a7e01681ce68" />
<img width="1024" height="1024" alt="image_3" src="https://github.com/user-attachments/assets/c1d1235f-30bd-4e78-84b9-fbd68e29716f" />
