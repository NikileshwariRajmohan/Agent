# Agentic AI 

# Nova AI 🎙️

Nova AI is a voice-controlled AI web application that allows users to interact with different services using simple voice commands.

The application can understand voice commands, generate emails using AI, open the generated email in Gmail, and search and play songs through YouTube.

## 🚀 Features

* 🎙️ Voice command recognition
* 🤖 AI-powered email generation
* ✉️ Automatic recipient, subject, and email body generation
* 📧 Open generated emails in Gmail
* 📝 Review and edit generated emails before opening Gmail
* ▶️ Search and play songs on YouTube
* 🔄 Email generation control
* 🌐 Browser-based application
* 💻 Works on laptop and mobile browsers

## 🎤 Voice Commands

Nova AI supports different types of voice commands.

### 📧 Email Commands

Example:

```text
Create an email for my manager
```

Another example:

```text
Create email for my boss
```

When Nova AI detects an email command, it generates:

```text
Recipient
Subject
Email Body
```

The generated email is displayed in the email editor where the user can review or edit it.

The user can then click:

```text
Open in Gmail
```

to open the Gmail compose page with the generated email details.

### ▶️ YouTube Commands

Example:

```text
Play Believer
```

or:

```text
Song Believer
```

Nova AI detects the YouTube command, searches for the requested song, and opens the result in YouTube.

## 🔄 How Nova AI Works

```text
User Voice Command
        ↓
Speech Recognition
        ↓
Command Detection
        ↓
 ┌───────────────┐
 │               │
 ↓               ↓
Email          YouTube
Command        Command
 │               │
 ↓               ↓
AI Email       Song Search
Generation        │
 │                 ↓
 ↓              YouTube
Gmail
```

## 🧠 Email Generation Flow

```text
Voice Command
      ↓
"Create an email for my manager"
      ↓
Frontend sends command to Flask
      ↓
AI generates email
      ↓
Recipient + Subject + Body
      ↓
Email Editor
      ↓
User reviews/edits email
      ↓
Open in Gmail
```

## ▶️ YouTube Flow

```text
Voice Command
      ↓
"Play Believer"
      ↓
Frontend sends command to Flask
      ↓
YouTube search
      ↓
Song URL
      ↓
YouTube opens
      ↓
Song plays
```

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript
* Web Speech API

### Backend

* Python
* Flask
* Flask-CORS

### AI

* Gemini API

### External Services

* Gmail
* YouTube

## 📁 Project Structure

```text
Nova AI/
│
├── app/
│   ├── gmail.py
│   └── youtube.py
│
├── templates/
│   └── index.html
│
├── app.py
│
├── requirements.txt
│
└── README.md
```

## ⚙️ Installation

### 1. Download or Clone the Project

Open the project folder in your terminal.

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

For Windows:

```bash
venv\Scripts\activate
```

### 4. Install Required Packages

```bash
pip install -r requirements.txt
```

## 🔑 API Configuration

Create a `.env` file in the project folder and add your Gemini API key.

```text
GEMINI_API_KEY=your_api_key
```

Replace:

```text
your_api_key
```

with your actual Gemini API key.

**Do not upload your API key to GitHub or share it publicly.**

## ▶️ Running the Application

After installing the dependencies, run:

```bash
python app.py
```

The Flask server will start.

Open the local URL shown in the terminal in your browser.

For example:

```text
http://127.0.0.1:5000
```

## 📱 Using Nova AI

### Step 1

Open Nova AI in your browser.

### Step 2

Allow microphone permission when requested.

### Step 3

Click the microphone button.

### Step 4

Speak a command.

For example:

```text
Create an email for my manager
```

### Step 5

Nova AI generates the email.

### Step 6

Review or edit:

```text
Recipient
Subject
Email Body
```

### Step 7

Click:

```text
Open in Gmail
```

to open Gmail with the email details.

For YouTube, say:

```text
Play Believer
```

and Nova AI opens the requested song.

## 🌐 Browser Support

Nova AI uses the browser's Web Speech API for voice recognition.

The application requires:

* Microphone permission
* Internet connection
* A browser that supports Speech Recognition

If speech recognition is unavailable, the application displays:

```text
Speech recognition unavailable
```

## 🔐 Security

* Keep API keys inside environment variables.
* Do not commit `.env` files to public repositories.
* Do not expose secret API keys in frontend JavaScript.
* Use appropriate API restrictions when deploying the application.

## 📌 Current Command Detection

### Gmail

Nova AI identifies an email command when the command contains both:

```text
create
```

and:

```text
email
```

Examples:

```text
Create an email for my boss
Create email for my manager
```

### YouTube

Nova AI identifies a YouTube command when the command contains:

```text
play
```

or:

```text
song
```

Examples:

```text
Play Believer
Song Believer
```

## 🔮 Future Enhancements

The following features can be added in future versions:

* 🗣️ Tamil voice command support
* 🌍 Multi-language voice recognition
* 📎 Email attachment support
* 📬 Support for multiple email services
* 🎤 Voice response from Nova AI
* 🤖 More AI-powered commands
* 📅 Google Calendar integration
* 🔔 Reminder and notification features
* 🔎 More advanced natural-language command detection
* 📱 Improved mobile application support

## 🎯 Project Objective

The main objective of Nova AI is to create a simple voice-controlled AI assistant that reduces the need for manual interaction with commonly used services.

Instead of typing commands manually, users can use their voice to perform tasks such as generating emails and playing songs.

## 💡 Advantages

* Easy to use
* Voice-based interaction
* Reduces manual typing
* AI-powered email generation
* Simple user interface
* Supports multiple functionalities
* Can be extended with additional AI features

## 👩‍💻 Author

Developed as an AI-powered voice assistant web application.

## 📄 License

This project is developed for educational and project purposes.


