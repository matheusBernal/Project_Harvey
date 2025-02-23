# Harvey - Virtual Assistant

## Description
Harvey is a virtual assistant that recognizes voice commands in Portuguese and executes specific actions, such as opening YouTube in a browser or launching desktop applications like Excel, Word, and PowerPoint.

## Technologies Used
- Python
- Selenium
- SpeechRecognition
- pyttsx4
- subprocess

## Requirements
Before running the project, make sure to install the necessary libraries. You can install them with the following command:

```sh
pip install selenium SpeechRecognition pyttsx4
```

Additionally, for proper voice recognition functionality, you need to have **PyAudio** installed:

```sh
pip install pyaudio
```
If you encounter errors installing PyAudio, try installing it using your system's package manager:
- **Windows:** Download the appropriate binary from [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio) and install it with:
  ```sh
  pip install filename.whl
  ```
- **Linux:**
  ```sh
  sudo apt-get install portaudio19-dev && pip install pyaudio
  ```

## Setting Up the Environment
To ensure smooth execution, create a virtual environment before installing dependencies:

```sh
python -m venv .venv
source .venv/bin/activate  # For Linux/macOS
.venv\Scripts\activate    # For Windows
pip install -r requirements.txt
```
Alternatively, you can use **Anaconda**:

```sh
conda create --name harvey-env python=3.9
conda activate harvey-env
pip install selenium SpeechRecognition pyttsx4 pyaudio
```

## How to Run

1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/PROJECT_HARVEY.git
   ```
2. Navigate to the project folder:
   ```sh
   cd PROJECT_HARVEY
   ```
3. Run the main script:
   ```sh
   python virtualAssistent.ipynb
   ```

## Features
- Harvey starts with a welcome message using text-to-speech.
- It listens for voice commands in Portuguese and executes one of the following actions:
  - **Open YouTube:** Say "YouTube".
  - **Open Excel:** Say "Excel".
  - **Open Word:** Say "Word".
  - **Open PowerPoint:** Say "PowerPoint".

## Possible Issues and Solutions
- **Voice recognition not working:** Check if your microphone is functional and if `pyaudio` is installed correctly.
- **Selenium does not open the browser:** Ensure you have the appropriate WebDriver installed for Microsoft Edge.
- **Office applications do not open:** Check if the commands `start excel`, `start word`, `start powerpnt` work in the Command Prompt.

## Author
Developed by Matheus Santhiago Bernal Jorge de Oliveira Borges.

