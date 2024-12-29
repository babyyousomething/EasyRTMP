# RTMP Server Manager

RTMP Server Manager is a user-friendly application for setting up and managing your own RTMP server using NGINX with the RTMP module. This tool is designed to simplify the live streaming process, even for non-technical users.

---

## Features

- **Easy Configuration**: Set the server port and stream directory effortlessly.
- **Precompiled Application**: No need for Python or additional dependencies.
- **Stream Management**:
  - Enable or disable bandwidth limits.
  - Toggle stream recording.
  - Require authentication for streaming.
- **NGINX RTMP Integration**: Automatically downloads and configures NGINX with RTMP support.
- **One-Click Control**:
  - Start and stop the RTMP server.
  - Monitor server activity via real-time logs.
- **Persistent Configurations**: Save and load your server settings.

---

## System Requirements

1. **Operating Systems**: Windows (precompiled for Windows).
2. **Disk Space**: Minimum 50MB for the application and NGINX setup.

---

## Installation

1. **Download the Precompiled Application**:
   - Download it here

3. **Extract the Files**:
   - Extract the downloaded `.zip` file to a desired location on your computer.

4. **Run the Application**:
   - Double-click `RTMPServerManager.exe` to launch the application.

---

## Usage

1. **Launch the Application**:
   - Open `RTMPServerManager.exe`.

2. **Configure the Server**:
   - Set the server port and specify the stream directory.
   - Adjust additional settings (e.g., bandwidth limits, recording, authentication).

3. **Download NGINX**:
   - Use the "Download NGINX RTMP" button to fetch and configure NGINX automatically.

4. **Start the Server**:
   - Click "Start Server" to launch the RTMP server.

5. **Stream Content**:
   - Use a tool like OBS or FFmpeg to publish streams to:
     ```
     rtmp://<your_server_ip>:<port>/live/
     ```

6. **Watch the Stream**:
   - Use VLC or a compatible player to view the stream at:
     ```
     rtmp://<your_server_ip>:<port>/live/
     ```

7. **Stop the Server**:
   - Click "Stop Server" when finished.

---

## Troubleshooting

- **Server Fails to Start**:
  - Ensure NGINX is downloaded and configured correctly.
  - Verify that the specified port is not in use by another application.

- **Cannot View Stream in VLC**:
  - Double-check the RTMP URL and ensure the server is running.
  - Confirm that your firewall allows RTMP traffic.

- **File Not Found Errors**:
  - Make sure the necessary directories (`logs`) and files (`mime.types`) exist in the stream directory.

---

## License

This application is licensed under the MIT License. See the `LICENSE` file for details.

---

## Credits

- Developed using:
  - [NGINX RTMP Module]([https://github.com/arut/nginx-rtmp-module](https://github.com/illuspas/nginx-rtmp-win32/archive/refs/tags/v1.2.1.zip))
  - [PyQt5](https://riverbankcomputing.com/software/pyqt/intro)

For support or inquiries, contact: koarik622@gmail.com

