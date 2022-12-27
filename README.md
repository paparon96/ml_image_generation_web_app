

<p align = "center" draggable=”false” ><img src="https://user-images.githubusercontent.com/37101144/161836199-fdb0219d-0361-4988-bf26-48b0fad160a3.png" 
     width="200px"
     height="auto"/>
</p>



# <h1 align="center" id="heading">FastAPI for Machine Learning Live Demo</h1>

This repository contains the files to build your very own AI image generation web application! Outlined are the core components of the FastAPI web framework, and application leverage the newly-released Stable Diffusion text-to-image deep learning model.

📺 You can checkout the full video [here](https://www.youtube.com/watch?v=_BZGtifh_gw)!

![Screenshot 2022-12-15 at 11 34 39 AM](https://user-images.githubusercontent.com/37101144/207929696-886ccfe3-6d86-4674-8aca-0844fb795727.png)

![Screenshot 2022-12-15 at 11 35 51 AM](https://user-images.githubusercontent.com/37101144/207929748-afafc036-cbf6-48aa-a7b2-b64d66c32b75.png)

# Running the application
Run the API in your environment: `uvicorn main:app`

# Interactive documentation
The interactive API docs are available locally [here](http://127.0.0.1:8000/docs).


# Usage examples

Below you can find particular code snippets for the various use cases that this API supports (the same could be achieved/tested through the OpenAPI docs page as well).

## Get a new image
```
import requests

prompt = "Sheriff in the woods"

response = requests.get('http://127.0.0.1:8000/generate?prompt={prompt}')
print(response)
```
