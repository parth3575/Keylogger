# Keylogger

This Python-based keylogger script demonstrates the functionality of logging keyboard inputs and provides two reporting methods: email and file. It uses the `pynput` library to monitor keyboard events and logs them, allowing you to choose between sending logs via email or saving them to a file.

**Note:** The use of keyloggers for unauthorized monitoring of keystrokes is illegal and unethical. This script is provided for educational purposes only, and it should only be used with explicit consent and for legitimate purposes.

## Features

- Logs keyboard inputs, including key presses and special keys.
- Offers two reporting methods: email and file.
- Customizable reporting interval.
- Designed for educational and informational purposes.

## Configuration

Before running the script, you should configure the following variables in the script according to your requirements:

- `SEND_REPORT_EVERY`: The interval (in seconds) at which logs should be reported.
- `EMAIL_ADDRESS`: Your email address for the email reporting method.
- `EMAIL_PASSWORD`: Your email password for the email reporting method.

## Usage

1. Clone the repository or download the source code.

2. Run the `keylogger.py` script.

3. Depending on the reporting method you want to use, uncomment either of the following lines:
   
   For email reporting:
   ```python
   keylogger = Keylogger(interval=SEND_REPORT_EVERY, report_method="email")
   ```

   For file reporting:
   ```python
   keylogger = Keylogger(interval=SEND_REPORT_EVERY, report_method="file")
   ```

4. Start logging by executing `keylogger.start()`.

5. The script will start logging keyboard inputs. To stop the keylogger, press the 'Esc' key.

## Reporting Methods

### Email Reporting

When using the email reporting method, the keylogger will periodically send logged keystrokes to the specified email address. This method requires you to provide your email address and password.

**Note:** Use a disposable or testing email address for security reasons. Avoid using your primary email account.

### File Reporting

When using the file reporting method, the keylogger will save logged keystrokes to a text file in the same directory as the script. Each session of keylogging will result in a new file with a timestamp in its name.

## Disclaimer

This keylogger script is intended for educational and informational purposes only. The author does not condone or endorse any unethical or illegal use of this script. It is the user's responsibility to use this script in compliance with applicable laws and regulations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
