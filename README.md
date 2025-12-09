# curl-python
Convert any curl command into clean, ready-to-run Python requests code. Free online curl-to-Python converter with headers, JSON, auth, and session support.
# cURL → Python Requests Converter 🐍

Instantly convert any `curl` command into clean Python code using the `requests` library — no manual translation needed.

## ❤️ Acknowledgments

This project powers the online cURL → Python Requests Converter available at:  
https://flipperfile.com/developer-tools/curl-to-python-requests-converter/


## 🚀 What It Is

This tool takes a `curl` command (including HTTP method, headers, body, auth, and common flags) and produces runnable Python `requests` code. Perfect for developers migrating shell-based API calls into Python automation or backend integrations.

## ✅ Key Features

- Supports all major HTTP methods  
- Handles JSON, form data, multipart, and raw payloads  
- Parses headers, tokens, and authentication  
- Interprets common `curl` flags (`-X`, `-H`, `-d`, `--data-raw`, etc.)  
- Optional `requests.Session()` output  
- Generates well-formatted, copy-ready code  

## 📥 How to Use

1. Paste your `curl` command into the input box  
2. Adjust options if desired  
3. Copy the auto-generated Python code  
4. Drop it into your script and run

Example:

```shell
curl -X POST https://api.example.com/login \
     -H "Content-Type: application/json" \
     -d '{ "username": "user", "password": "pass" }'

Becomes:

import requests

response = requests.post(
    "https://api.example.com/login",
    headers={ "Content-Type": "application/json" },
    json={ "username": "user", "password": "pass" }
)

print(response.status_code, response.text)

🎯 Why Use This Tool

Translating complex curl commands by hand is tedious and error-prone. This converter automates the process and produces consistent, reliable Python code — especially useful for:

API testing → automation

Migrating command line workflows to Python

Rapid prototyping

Teaching & documentation

🔧 Contributing

Contributions are welcome!

Fork the repo

Create a feature branch (feat/...)

Submit a pull request

Please keep code clean and documented.

📝 License

Distributed under the MIT License.
