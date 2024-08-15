# Keylogger Script

## Overview

This Python script is designed to act as a keylogger that records keystrokes, captures screenshots, records microphone input, and logs system information. It periodically sends these reports via email. The script utilizes various Python modules to achieve its functionalities and attempts to install any missing modules automatically.

## Features

- **Keylogging:** Captures and logs all keystrokes.
- **Screenshot Capture:** Takes screenshots of the desktop.
- **Microphone Recording:** Records audio from the microphone.
- **System Information:** Logs details about the system such as hostname, IP address, and system specs.
- **Email Reporting:** Sends periodic reports via email.

## Dependencies

The script requires the following Python modules:

- `logging`
- `os`
- `platform`
- `smtplib`
- `socket`
- `threading`
- `wave`
- `pyscreenshot`
- `sounddevice`
- `pynput`
- `glob`

If any of these modules are not installed, the script will attempt to install them automatically.

## Installation

1. Clone the repository or download the script file.

2. Ensure you have Python 3.x installed on your system.

3. Install the required dependencies by running:
    ```bash
    pip install pyscreenshot sounddevice pynput
    ```

## Configuration

1. Open the script and update the following placeholders with your email credentials:

    ```python
    EMAIL_ADDRESS = "YOUR_USERNAME"
    EMAIL_PASSWORD = "YOUR_PASSWORD"
    ```

2. Set the desired interval for sending email reports by adjusting the `SEND_REPORT_EVERY` variable:

    ```python
    SEND_REPORT_EVERY = 60 # in seconds
    ```

## Usage

1. Run the script using Python:

    ```bash
    python keylogger_script.py
    ```

2. The script will start logging keystrokes, capturing screenshots, recording audio, and collecting system information. Reports will be sent to the specified email address at the interval you set.

## File Cleanup

- **Windows:** The script will attempt to terminate itself and delete the file after execution.
- **Unix-like systems:** The script will attempt to kill any associated editor processes and remove the file.

## Important Notes

- **Privacy and Legality:** Use this script responsibly and ensure you have the necessary permissions. Unauthorized use of keyloggers may violate privacy laws and regulations.
- **Ethical Use:** This script is intended for educational purposes only. Always respect privacy and legal boundaries.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

The authors and contributors of this script are not responsible for any misuse or legal consequences that may arise from using this script. It is your responsibility to ensure that your use complies with all applicable laws and regulations.

