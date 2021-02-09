# tesseract-docker

## About
This is a simple docker file for Tesseract Optical Character Recognition

This is mainly as a quick experiment with Docker, as well as a means to build alater version of Tesseract than was available for install at the time of writing

## Dependencies
Docker: https://hub.docker.com
Tesseract: https://github.com/tesseract-ocr/tesseract

## Usage Notes
1. Clone from git
2. Build container:
`docker build -t tesseract .`
3. Run test:
`docker run --mount type=bind,source="$(pwd)"/test,target=/test tesseract:latest tesseract /test/Owl.png /test/Owl pdf`