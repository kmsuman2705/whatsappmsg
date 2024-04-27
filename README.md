# PyWhatKit Automated WhatsApp Message Sender

This Python script uses the `pywhatkit` library to send automated WhatsApp messages.

## Features

- **Automated Message Sending**: Allows users to send automated WhatsApp messages to a recipient.
- **Scheduled Sending**: Users can schedule messages to be sent at a specific time.

## Requirements

- Python 3.x
- `pywhatkit` library (`pip install pywhatkit`)

## Usage

1. Install the `pywhatkit` library using the following command:

2. Update the script with the recipient's phone number and the message to be sent.

3. Run the script using Python.

## Example

```python
import pywhatkit as kit
from datetime import datetime

# Define the recipient's phone number and message
phone_number = "+916200164517"  # Replace with the recipient's phone number
message = "Hello, this is an automated message!"

# Get the current time
now = datetime.now()
current_hour = 16
current_minute = 47

# Send the message on WhatsApp instantly
kit.sendwhatmsg(phone_number, message, current_hour, current_minute + 1)
