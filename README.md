# RemoveBG

Flask application to remove background from an image.

## Introduction

RemoveBG is a Flask application designed to remove the background from images. This application can be used to process images and remove unwanted backgrounds, making it ideal for various applications such as e-commerce, graphic design, and more.

## Demo

[Screencast from 2025-03-30 08-59-21.webm](https://github.com/user-attachments/assets/1a8feace-92fa-40c2-bf58-8a22c1a0147f)

[Watch on Youtube](https://youtu.be/WsU47ba4dfg)
## Features

- Remove background from images
- Easy to use web interface
- Supports multiple image formats
- Docker support for easy deployment

## Installation

### Prerequisites

- Python 3.6 or higher
- Flask
- Docker (optional, for containerized deployment)

### Clone the Repository

```bash
git clone https://github.com/Nithin1729S/RemoveBG.git
cd RemoveBG
```

### Setting Up the Virtual Environment

Create a virtual environment and activate it:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

### Running the Application

Start the Flask application:

```bash
export FLASK_APP=app.py
export FLASK_ENV=development
flask run
```

The application will be accessible at `http://127.0.0.1:5000`.

### Using Docker

If you prefer to use Docker, you can build and run the application using the provided Dockerfile.

Build the Docker image:

```bash
docker build -t removebg .
```

Run the Docker container:

```bash
docker run -p 5000:5000 removebg
```

The application will be accessible at `http://127.0.0.1:5000`.

## Usage

1. Open a web browser and navigate to `http://127.0.0.1:5000`.
2. Drag and Drop an image file.
3. Click the "Remove Background" button.
4. Download the processed image with the background removed.

## Model Download

The model used for background removal can be downloaded from the following link:

[Download U2Net Model](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx)

Make sure to place the downloaded model in the appropriate directory as specified in the application.
