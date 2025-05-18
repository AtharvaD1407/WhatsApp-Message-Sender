# WhatsApp Message Sender using Python

This repository contains multiple Python scripts for automating WhatsApp messages. It demonstrates two different methods to send WhatsApp messages to a specific phone number at a scheduled time.

## Methods Available

### 1. **Send WhatsApp Messages using `pywhatkit`**

`pywhatkit` is a simple Python library that automates WhatsApp message sending. This method works by opening WhatsApp Web in your default browser at the scheduled time and sending a message to the specified phone number.

#### Key Features:
- Simple and easy to use.
- Requires an active WhatsApp Web session in your browser.
- Schedule the message by specifying the recipient's number, message content, and the time (hour and minute) to send it.

#### Use Case:
- Great for personal use or one-off messages that need to be sent at a specific time.

### 2. **Send WhatsApp Messages using `Twilio API`**

The Twilio API provides a more advanced solution for sending WhatsApp messages programmatically. With Twilio, you can send WhatsApp messages from a registered Twilio number or the Twilio sandbox, and you can also schedule messages to be sent at a specific date and time.

#### Key Features:
- Requires a Twilio account and WhatsApp sandbox configuration.
- More flexible than `pywhatkit` (can send messages programmatically and integrates easily with other systems).
- The script calculates the time difference between the current time and the scheduled time and waits for that time before sending the message.

#### Use Case:
- Ideal for sending messages to multiple recipients, integrating into larger applications, or scheduling messages for recurring events.

## Repository Structure

This repository contains the following main components:

- **pywhatkit.ipynb**: A script to send WhatsApp messages using the `pywhatkit` library.
- **twilio.ipynb**: A script to send WhatsApp messages using the Twilio API, including setup instructions for your Twilio account and WhatsApp sandbox configuration.

## How to Use

### 1. **Using `pywhatkit` Method**:
- Install the `pywhatkit` library.
- Set the recipient's phone number, message, and time you want the message to be sent.
- Run the script, and it will open WhatsApp Web at the scheduled time to send the message.

### 2. **Using `Twilio API` Method**:
- Set up a **Twilio account** at [Twilio](https://www.twilio.com/).
- Activate your **Twilio WhatsApp Sandbox**.
- Install the `twilio` Python library.
- Configure the `account_sid`, `auth_token`, and your Twilio WhatsApp sandbox number in the script.
- Enter the scheduled time and the recipient’s number in the script.
- Run the script, and it will send the message at the specified time.

## Prerequisites

- Python 3.x
- Active WhatsApp Web session (for `pywhatkit`)
- **Twilio account** and **WhatsApp Sandbox** configuration (for Twilio API)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AtharvaD1407/WhatsApp-Message-Sender.git
   ```
