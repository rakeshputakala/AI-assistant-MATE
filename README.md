# AI-assistant-MATE
MATE is a sleek and interactive web-based personal assistant designed to simplify user interactions. With a dynamic gradient background and microphone-enabled functionality, MATE provides an engaging experience for users. Built with HTML, CSS, and Font Awesome, this project highlights clean design and responsiveness, making it accessible on various devices.

[**Live Demo**](https://rakeshputakala.github.io/AI-assistant-MATE)

Features

Dynamic Gradient Background: A visually appealing animated gradient that changes over time.
User Interaction: A microphone button to capture user input.
Responsive Design: Ensures compatibility across various screen sizes.

Files

- **index.html**: The main structure of the web application.
- **style.css**: The stylesheet for styling the interface.
- **MATE.js**: Script file for handling the functionality.

Features:
1.   Speech Synthesis (Voice Output)  : 
                 - script uses the `SpeechSynthesisUtterance` API to speak text using a pre-selected female voice, adjusting the rate, volume, and pitch of the voice output.

2.   Speech Recognition (Voice Input)  : 
                 - The `SpeechRecognition` API is used to capture voice input when the user clicks on the microphone button. It listens for commands and transcribes them to text.

3.   Greeting & Time-Based Wishes  : 
                 - Upon initialization or page load, the assistant greets the user with "Good Morning," "Good Afternoon," or "Good Evening" based on the current time.

4.   Command Processing  : 
- It listens for specific commands (e.g., "open google," "what is," "time," etc.) and performs corresponding actions:
   - Opens websites like Google, YouTube, Facebook, and Wikipedia.
   - Searches for information on Google when commands like "what is" or "who is" are detected.
   - Retrieves the current time and date and responds verbally.
   - Opens system apps like the calculator, camera, or WhatsApp.


Here's a short code breakdown  of the key parts in  JavaScript  :

    1.   Voice Initialization  :
   - `window.speechSynthesis.onvoiceschanged`: This listens for when voices are available and calls `populateVoiceList()` to populate the voice options in the dropdown.
   - `populateVoiceList()`: This function populates the dropdown with available voices and sets the initial voice (female by default).

    2.   Voice Selection  :
   - `setVoice()`: When the user selects a voice from the dropdown, this function updates the `selectedVoice` variable with the chosen voice and notifies the user by speaking the name of the selected voice.

    3.   Speech Synthesis  :
   - `speak(text)`: Converts text to speech using the selected voice. The rate, volume, and pitch are customizable.

    4.   Speech Recognition  :
   - `recognition.onresult`: This listens for voice input when the user clicks the microphone button. It transcribes the speech into text and processes it using the `takeCommand()` function.
   
    5.   Command Processing  :
   - `takeCommand(message)`: Based on the recognized speech, it checks for specific commands (e.g., "open google," "time," "date") and performs actions like opening websites, telling the time, or searching Google.

    6.   Event Listeners  :
   - The `btn.addEventListener('click', ...)` starts voice recognition when the microphone button is clicked.
   - `voiceSelector.addEventListener('change', ...)` listens for voice selection changes and updates the voice accordingly.

# DEMO
<img width="926" alt="image" src="https://github.com/user-attachments/assets/ee73fbe8-be23-4ee8-8fd7-1c42fd5db020">






