📌 Phone Call Monitor & DTMF Analyzer
A Python-based GUI application that automates phone call operations using ADB, monitors call status using OCR, plays audio responses, and analyzes recorded calls to detect DTMF tones. This tool is designed for telecom testing, automation, and IVR system validation.
🚀 Features
📞 Call Automation

Initiates phone calls using ADB (Android Debug Bridge)
Reads phone numbers from an Excel file
Automatically dials numbers sequentially

🧠 Smart Call Monitoring

Captures live screenshots from the connected Android device
Uses OCR (Tesseract) to detect call status (ringing, calling, busy, ended)
Automatically reacts based on detected screen text

🔊 Audio Playback

Plays a predefined audio file during calls
Stops playback and disconnects calls automatically

🎯 DTMF Tone Detection

Extracts recorded calls from the device
Converts MP3 recordings to WAV using FFmpeg
Implements Goertzel Algorithm for detecting DTMF tones
Detects keypad tones (e.g., 1, 2) from call recordings

📊 Result Export

Saves detected DTMF tones into Excel files
Separate sheets/files for different tones
Directly opens results from the GUI

🖥️ GUI Interface

Built with Tkinter
Easy configuration of:
ADB path
Audio file
Phone number list
Monitoring parameters

🛠️ Tech Stack

Python
Tkinter (GUI)
OpenCV / PIL (image processing)
pytesseract (OCR)
pandas (Excel handling)
pygame (audio playback)
ADB (Android Debug Bridge)
FFmpeg (audio conversion)

📂 Workflow

Load phone numbers from Excel
Initiate calls via ADB
Capture screenshots and analyze text using OCR
Play audio when conditions are met
End calls automatically
Pull recorded calls from device
Convert audio and detect DTMF tones
Save results into Excel files

⚙️ Setup

Install Dependencies
   
pip install pytesseract pandas pillow pygame

Install Required Tools

Install ADB (Android Debug Bridge)

Install FFmpeg

Install Tesseract OCR

Configure Paths

Update paths in the script:

ADB executable

FFmpeg path

Audio file

Excel file with phone numbers

Run the Application

python main.py

📊 Use Cases

Telecom automation testing
IVR system validation
Call center workflow testing
DTMF tone analysis
Automated call monitoring systems

⚠️ Notes

Requires USB debugging enabled on Android device
Device must allow ADB call permissions
OCR accuracy depends on screen quality
Supports limited DTMF tones (can be extended)

🚀 Future Improvements

Support all DTMF tones (0–9, *, #)

Real-time waveform visualization
Multi-device support
Cloud-based logging system
Better OCR optimization using deep learning
🧾 Conclusion

This project integrates automation, OCR, audio processing, and signal analysis into a single system, making it a powerful tool for telecom and embedded system testing workflows.
