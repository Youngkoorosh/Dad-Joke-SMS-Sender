# Dad Joke SMS Sender

---

## 🚀 Overview

This is a simple Python script that fetches a random "dad joke" from `icanhazdadjoke.com/slack` and sends it to a specified phone number via SMS using the Kavenegar API. It's a fun little project to practice working with external APIs and SMS services.

## ✨ Features

* Fetches a random joke from `icanhazdadjoke.com`.
* Sends the joke as an SMS using the Kavenegar API.
* Uses environment variables for secure API key management.

## 🛠️ Installation

1.  **Clone the repository (or download the script):**
    ```bash
    git clone [https://your-github-repo-link.git](https://your-github-repo-link.git)
    cd dad-joke-sms-sender
    ```
    (Replace `https://your-github-repo-link.git` with your actual repository URL)

2.  **Install the required Python libraries:**
    ```bash
    pip install requests kavenegar
    ```

## ⚙️ Configuration

To run this script, you need to set up your Kavenegar API key and the recipient's phone number. It's highly recommended to use **environment variables** for sensitive information.

1.  **Get your Kavenegar API Key:** Sign up or log in to your Kavenegar account at [kavenegar.com](https://kavenegar.com/) and find your API key.
2.  **Set Environment Variables:**
    * **`KAVENEGAR_API_KEY`**: Your unique Kavenegar API key.
    * **`RECEIVER_PHONE_NUMBER`**: The phone number to which the SMS will be sent (e.g., `989123456789`). Make sure it's in the correct international format without `+` or `0` prefix.
    * **`SENDER_NUMBER`**: (Optional) Your Kavenegar sender number (e.g., `10008663`). If not set, the script will use a default.

    **Example (Linux/macOS):**
    ```bash
    export KAVENEGAR_API_KEY="YOUR_ACTUAL_KAVENEGAR_API_KEY"
    export RECEIVER_PHONE_NUMBER="989123456789"
    # export SENDER_NUMBER="10008663" # Optional, if you have a specific sender number
    ```
    **Example (Windows - Command Prompt):**
    ```cmd
    set KAVENEGAR_API_KEY="YOUR_ACTUAL_KAVENEGAR_API_KEY"
    set RECEIVER_PHONE_NUMBER="989123456789"
    # set SENDER_NUMBER="10008663" # Optional
    ```
    **Example (Windows - PowerShell):**
    ```powershell
    $env:KAVENEGAR_API_KEY="YOUR_ACTUAL_KAVENEGAR_API_KEY"
    $env:RECEIVER_PHONE_NUMBER="989123456789"
    # $env:SENDER_NUMBER="10008663" # Optional
    ```

    *Remember to replace placeholder values with your actual information.*

## 🚀 Usage

After setting up the environment variables, simply run the Python script:

```bash
python dad_joke_sms.py
