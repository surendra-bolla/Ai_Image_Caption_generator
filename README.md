# AI Image Caption Generator

An AI-powered web application that generates natural language descriptions for uploaded images. The system uses a pretrained vision-language model to analyze images and produce captions automatically.

This project demonstrates how modern **vision-language models** can be integrated into a web application for tasks like accessibility, content description, and social media caption generation.

---

## Features

* Upload an image through a simple web interface
* AI analyzes the image and generates a caption
* FastAPI backend for handling requests
* Hugging Face Transformers for the captioning model
* Lightweight HTML + CSS frontend
* Automatic model download on first run

---

## Tech Stack

**Backend**

* Python
* FastAPI
* Uvicorn

**AI / Machine Learning**

* Hugging Face Transformers
* BLIP Image Captioning Model
* PyTorch

**Frontend**

* HTML
* CSS
* JavaScript

---

## Project Structure

```
ai_image_caption
│
├── main.py                # FastAPI server
├── requirements.txt       # Python dependencies
├── README.md
│
├── templates
│   └── index.html         # Frontend UI
│
├── static
│   └── style.css          # Styling
│
└── venv                   # Virtual environment (not pushed to GitHub)
```

---

## Installation

Clone the repository:

```
git clone https://github.com/yourusername/ai-image-caption-generator.git
cd ai-image-caption-generator
```

Create a virtual environment:

```
python -m venv venv
```

Activate it:

Windows:

```
venv\Scripts\activate
```

Install dependencies:

```
pip install -r requirements.txt
```

---

## Running the Application

Start the FastAPI server:

```
uvicorn main:app --reload
```

Open your browser and go to:

```
http://127.0.0.1:8000
```

Upload an image and the AI model will generate a caption describing the image.

---

## Model Information

This project uses the **BLIP Image Captioning model** from Hugging Face.

Model repository:

https://huggingface.co/Salesforce/blip-image-captioning-base

The model is automatically downloaded the first time the application runs.

Approximate model size:

```
~990 MB
```

After the first download, it is cached locally and reused.

---

## Example

Input Image:

```
Image of a dog running in a field
```

Generated Caption:

```
"A brown dog running through the grass."
```

---

## Use Cases

* Accessibility tools for visually impaired users
* Automatic image descriptions
* Social media caption generation
* Dataset annotation for machine learning
* Content management systems

---

## Future Improvements

Possible enhancements:

* Drag-and-drop image upload
* Multiple caption styles (formal, funny, social media)
* Voice output for accessibility
* React frontend interface
* Smaller optimized models for faster deployment
* Docker containerization

---

## License

This project is released under the MIT License.

---

## Acknowledgements

* Hugging Face Transformers
* Salesforce BLIP research team
* FastAPI framework
