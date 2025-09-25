## 🔐 Password Checker Project (Have I Been Pwned API)

This is a Python command-line tool that checks if your password has been exposed in known data breaches using the [HaveIBeenPwned](https://haveibeenpwned.com/API/v3#SearchingPwnedPasswordsByRange) API. It uses SHA-1 hashing and k-anonymity to ensure your password is never fully sent to the API.

### ✅ Features
- Secure password hash checking using k-anonymity
- Real-time breach count using HIBP API
- Command-line interface
- No password logging or storage

### 🧪 How It Works
1. Takes the password input.
2. Hashes it using SHA-1.
3. Sends the **first 5 characters** of the hash to the API.
4. Compares the tail of the hash with the API results locally.
5. Displays how many times the password has been found.

### 📦 Requirements
```bash
pip install requests
pip install sys

🚀 How to Run
python passchecker.py yourpassword here
python passchecker.py yourpassword here





