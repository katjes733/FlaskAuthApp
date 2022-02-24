# FlaskAuthApp
Flask Authentication Application

## Prerequisites
* Docker is installed
* A commnd line is available
* *(Optionally) VS Code*

## Instructions to build and run
1. From with the source directory, run the following command to build the docker image
    ```bash
    docker build --tag <TagName> .
    ```
    where \<TagName\> any arbitrary tag to identify the image.
1. Wait for th build to complete, then run the folowing command to run the image we just created
    ```bash
    docker run -d -p 5000:5000 <TagName>
    ```
1. Enter *http://localhost:5000* in your browser to run the application