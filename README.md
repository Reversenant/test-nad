![PyPI](https://img.shields.io/pypi/v/ptnad)

🌐 Available languages: [en English](README.en.md) | [🇷🇺 Русский](README.ru.md)

# PT NAD Client

Python library for interacting with the PT NAD API.

### 🚀 Installation
```python
pip install ptnad-client
```
### 📖 Usage
```python
from ptnad import PTNADClient

client = PTNADClient("https://1.3.3.7", verify_ssl=False)
client.set_auth(username="user", password="pass")
# client.set_auth(auth_type="sso", username="user", password="pass", client_id="ptnad", client_secret="11111111-abcd-asdf-12334-0123456789ab", sso_url="https://siem.example.local:3334")
client.login()

query = "SELECT src.ip, dst.ip, proto FROM flow WHERE end > 2025.02.25 and end < 2025.02.26 LIMIT 10"
result = client.bql.execute(query)
print(f"Results: {result}")
```
### ✅ Features

🔐 Authentication
- Local authentication
- IAM (SSO) authentication

📊 BQL Queries
- Execute queries

📡 Monitoring
- Get system status
- Manage triggers

🛡️ Signatures
- Retrieve classes
- Get rules (all/specific)
- Commit/Revert changes

📋 Replists
- Create/Modify basic and dynamic replists
- Retrieve replist info

### 🛠️ Upcoming Features
- Documentation
- Sources management
- Hosts management
- Groups management

## 🧑‍💻 Contributing

Want to contribute? Check out the following:

- [📄 Contributor Guide](CONTRIBUTING.md)
- [🛠 Recommended Best Practices](best_practices.md)

We welcome all ideas, suggestions, and improvements!

## 💬 Community

Join our Telegram community to discuss the project, ask questions, and share your ideas:

👉 [t.me/Сообщество экспертов по безопасности SEC](https://t.me/s3curity_experts_community)


### 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.