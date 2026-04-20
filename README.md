# Lumina

## AI Art Generator

Lumina is a voice-controlled AI art generator built using a Raspberry Pi 5. The system listens to a user’s spoken prompt, converts the prompt into text, sends it to DALL-E 3 for image generation, and displays the generated artwork on a connected TV or monitor through HDMI.

## Project Overview

Lumina allows users to generate artwork using only their voice. Instead of typing prompts manually, the user speaks a request into a USB microphone connected to the Raspberry Pi. The system processes the voice input, generates an AI image, and displays the final result on the screen.

Example prompts include:

- Lady in city walking by a park
- Boy kicking around a blue football
- Professor teaching computer architecture in university

## How It Works

The system follows this basic workflow:

1. The user speaks a prompt into the USB microphone.
2. A Python program captures and processes the voice input.
3. Picovoice is used to detect and understand the spoken command.
4. The recognized prompt is sent to DALL-E 3 using OpenAI’s Python library.
5. DALL-E 3 generates an image from the prompt.
6. The image is displayed on a TV or monitor connected through HDMI.
7. The program automatically adapts to the connected screen ratio.

## Hardware Used

### Raspberry Pi 5

The Raspberry Pi 5 acts as the main processing unit for Lumina. It runs the software application, processes user input, communicates with the AI image generation service, and controls the display output.

### USB Microphone

The USB microphone captures the user’s voice commands. It is connected directly to one of the Raspberry Pi’s USB ports.

### Micro HDMI to HDMI Cable

The Micro HDMI to HDMI cable connects the Raspberry Pi 5 to a TV or monitor. This allows the generated artwork to be displayed directly on the screen.

### Power Supply Cable

The power supply provides power to the Raspberry Pi 5 and allows the system to run independently.

## Software and Libraries

Lumina uses the following technologies:

- Python
- Picovoice
- OpenAI Python Library
- DALL-E 3
- Tkinter

## Features

- Voice-controlled prompt input
- AI-generated artwork using DALL-E 3
- HDMI output to TV or monitor
- Automatic screen ratio adjustment
- Simple user interface built with Tkinter
- Raspberry Pi-based standalone setup

## Challenges Faced

The main challenge was not the coding itself, but setting up and connecting the Raspberry Pi 5 for development. Since the Raspberry Pi 5 was relatively new, there were issues related to the operating system build, USB microphone drivers, and shell environment setup.

These issues were solved by:

- Making changes to the Raspberry Pi `.bashrc` file
- Customizing the shell environment
- Updating drivers for the USB microphone
- Fixing Raspberry Pi connection and setup issues

After resolving these setup problems, the remaining development process was straightforward.

## Final Implementation

Once the Raspberry Pi setup was completed, the project was implemented using:

- Picovoice for voice command recognition
- OpenAI libraries for image generation
- Tkinter for the user interface
- HDMI output for displaying generated images

## Future Improvements

Possible future improvements include:

- Adding support for multiple languages
- Improving voice recognition accuracy
- Adding a gallery to save previously generated images
- Supporting different image styles
- Adding a physical button or wake word for activation
- Improving the user interface
- Making the device fully portable

## Conclusion

Lumina demonstrates how voice recognition, AI image generation, and Raspberry Pi hardware can be combined into a practical creative tool. The project allows users to generate artwork through natural speech and display it instantly on a screen.
