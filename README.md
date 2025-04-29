# video-conferencing
Project for building a real-time video conferencing solution.
# Simple Video Conferencing Application

This project implements a basic video conferencing application using Python and the `vidstream` library. It allows for video and audio streaming, as well as screen sharing, between two connected parties. The application provides both client and server functionalities and uses a simple Flask web interface to initiate connections.

## Features

* **Video and Audio Streaming:** Real-time transmission of camera and microphone feeds.
* **Screen Sharing:** Ability to share the contents of the user's screen.
* **Client/Server Architecture:** Supports both client and server roles for establishing connections.
* **Simple User Interface:** Uses `tkinter` for basic desktop application windows.
* **Web-based Initiation:** A Flask web application provides an easy way to start client or server instances.

## Prerequisites

* Python 3.x
* `pip` (Python package installer)

## Installation

1.  **Clone the repository:**
    ```bash
    git clone <your_repository_url>
    cd <your_repository_directory>
    ```

2.  **Install the required Python packages:**
    ```bash
    pip install Flask vidstream 
    ```

## Usage

1.  **Start the Flask web application:**
    ```bash
    python app.py
    ```
    This will start a web server at `http://0.0.0.0:5000/`.

2.  **Open the web interface in your browser:**
    Navigate to `http://0.0.0.0:5000/`.

3.  **Choose to connect as either Client or Server:**
    * Click "Connect as Server" to start the server application. The server needs to be started first so that the client can connect to it.
    * Click "Connect as Client" to start the client application.  You'll need to provide the server's IP address in the client application's window.

4.  **In the Client or Server window:**
    * Enter the "Target IP" (the IP address of the other party).
    * Click the buttons to start listening for connections, and to start camera, screen sharing, or audio streams as needed.

## File Structure

* `app.py`:  Flask application to launch the client and server.
* `client.py`:  Client-side application for video conferencing.
* `index.html`:  HTML page for the Flask application.
* `server.py`:  Server-side application for video conferencing.

## Important Notes

* **Network Configuration:** Ensure that your network allows communication between the client and server (firewall settings, etc.). Both the server and the client must be on the same network or have appropriate port forwarding configured.
* **IP Addresses:** You will need to know the IP address of the machine running the server to connect from the client.
* **Error Handling:** This is a basic implementation and may lack robust error handling.
* **Security:** This project does not include security features like encryption.  Do not use it for sensitive communications without adding appropriate security measures.

## Disclaimer

This project is intended for educational or demonstration purposes.  It is not production-ready.
