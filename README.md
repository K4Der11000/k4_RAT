# k4_RAT
# kader11000 Android RAT Panel (For Educational Purposes Only)

## How to Run:

1. Make sure you have Python 3 installed.
2. Install Flask if not already installed:
   pip install flask

3. Run the app:
   python app.py

4. Open your browser and go to:
   http://127.0.0.1:5000

5. Login using the default password:
   kader11000

## Features:

- Web control panel for Android RAT connections.
- Stores each victim's session under sessions/victim_<id>/
- Allows live editing of host and port from settings page.
- Displays connected victims in a dashboard.
- Custom hacking-style design with a banner showing your name: "kader11000".

## Notes:

- Victim device should send JSON data to:
  http://<your_ip>:<port>/api/report

- Example JSON structure from victim device:
  {
    "device_id": "abc123",
    "device_name": "Samsung A12",
    "android_version": "11",
    "battery": "87%",
    "ip": "192.168.1.5",
    "timestamp": "2025-04-12 21:55"
  }

- You can modify or extend the API to include more actions like file upload, screenshot, mic, camera, etc.

## Default Configuration:
- Host: 127.0.0.1
- Port: 5000

You can change these from the web panel under Settings.
