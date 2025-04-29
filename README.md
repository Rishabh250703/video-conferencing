# video-conferencing
Project for building a real-time video conferencing solution.
# Simple Video Conferencing Application
This project provides a basic video conferencing application using Python and the `vidstream` library. It allows for video and audio streaming, as well as screen sharing.
## Table of Contents
1.  [Setup and Run](#setup-and-run)
2.  [Dependencies](#dependencies)
3.  [Configuration](#configuration)
4.  [Screenshots/Demo](#screenshotsdemo)
## 1. Setup and Run
**Prerequisites:**
* Python 3.x installed
* `pip` (Python's package installer) installed
**Steps:**
1.  **Clone the repository (or download the files):**
    ```bash
    # If using Git:
    git clone <repository_url>
    # Or download the files directly and extract them
    ```
2.  **Install Dependencies:**
    Navigate to the project directory in your terminal and install the required Python packages:
    ```bash
    pip install Flask vidstream
    ```
3.  **Run the Application:**
    * Start the main application using Flask:
        ```bash
        python app.py
        ```
    * This will start a Flask development server. Open your web browser and go to `http://0.0.0.0:5000/`
4.  **Connect Clients and Servers:**
    * The web page provides two buttons: "Connect as Client" and "Connect as Server".
    * Clicking these buttons will start the respective client or server scripts.
    * **Important:** You'll need to provide the "Target IP" in the client and server windows to establish a connection.  Ensure the server's IP address is entered into the client, and if you have multiple clients, they would generally connect to the same server IP.
## 2. Dependencies
* **Flask:** A web framework for Python (used for the initial web interface).
    ```bash
    pip install Flask
    ```
* **vidstream:** A library for easy video streaming in Python.
    ```bash
    pip install vidstream
    ```
* **tkinter:** Python's standard GUI library (used for the client and server interfaces).  This usually comes with Python, so you might not need to install it separately.
## 3. Configuration
* **IP Addresses:** The most crucial configuration is the correct IP address.
    * Find the IP address of the machine you want to act as the server. You can use commands like `ipconfig` (Windows) or `ifconfig` (Linux/macOS).
    * Enter this IP address into the "Target IP" field in both the client and server windows as needed.
* **Ports:** The application uses specific ports for different streams:
    * Server Streaming Port: 9999
    * Server Audio Receive Port: 8888
    * Client Streaming Port: 7777
    * Client Audio Receive Port: 6666
    * Camera Stream Port: 9999 (Client sends to Server)
    * Screen Share Port: 8888 (Client sends to Server)
    * Audio Stream Port: 6666 (Both directions)
    * Ensure these ports are not blocked by your firewall.
## 4. Screenshots/Demo
**(Please add screenshots or a link to a demo video here to show the application in action.)**
* **Screenshot 1:** Main page with "Connect as Client" and "Connect as Server" buttons.
    ``` ```
* **Screenshot 2:** Client window with the Target IP input and buttons.
    ``` ```
* **Screenshot 3:** Server window with the Target IP input and buttons.
    ``` ```
**Note:** This is a basic implementation and may require further development for production use (e.g., error handling, security, scalability).
