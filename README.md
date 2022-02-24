# FlaskAuthApp
Flask Authentication Application

## Prerequisites
* Docker is installed
* A commnd line is available
* VS Code

## Instructions to setup workspace
1. Install python virtual environment using the terminal. *It is recommended to use Command Prompt over the default Powershell.*
    ```bash
    python -m venv .venv
    ```
1. Kill any terminal windows and create a new Terminal. *It is recommended to use Command Prompt over the default Powershell.*
    The prompt should be prefixed by *(.venv)* indicating the virutal environment being activated.
1. Install the requirements
    ```bash
    pip install -r requirements.txt
    ```

## Instructions to build and run container
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