<div align="center">
  <img src="assets/banner.svg" alt="Reach GitHub Contributors Banner" width="800">

  # 🚀 Reach GitHub Contributors

  [![GitHub license](https://img.shields.io/github/license/ishandutta2007/reach-github-contributors?style=for-the-badge)](https://github.com/ishandutta2007/reach-github-contributors/blob/master/LICENSE)
  [![GitHub stars](https://img.shields.io/github/stars/ishandutta2007/reach-github-contributors?style=for-the-badge)](https://github.com/ishandutta2007/reach-github-contributors/stargazers)
  [![GitHub forks](https://img.shields.io/github/forks/ishandutta2007/reach-github-contributors?style=for-the-badge)](https://github.com/ishandutta2007/reach-github-contributors/network)
  [![Python Version](https://img.shields.io/badge/python-3.6%2B-blue?style=for-the-badge&logo=python)](https://www.python.org/)
  [![Gmail API](https://img.shields.io/badge/Gmail-API-red?style=for-the-badge&logo=gmail)](https://developers.google.com/gmail/api)

  **Automated Contributor Discovery and Personalized Email Outreach Tool**

  [Report Bug](https://github.com/ishandutta2007/reach-github-contributors/issues) · [Request Feature](https://github.com/ishandutta2007/reach-github-contributors/issues)

</div>

---

## 📖 Overview

**Reach GitHub Contributors** is a powerful Python-based automation tool designed to help developers, recruiters, and community managers connect with project contributors. It seamlessly crawls GitHub repository data, extracts contributor information (including verified emails), and automates personalized outreach via the Gmail API.

### 🎯 Why use this?
- **Community Building**: Engage with people who have already shown interest in your project.
- **Talent Sourcing**: Find and contact talented developers based on their contributions.
- **Feedback Collection**: Reach out to forkers and contributors for valuable insights.

---

## ✨ Features

- 🔍 **Smart Crawling**: Automatically extracts usernames, full names, and organizations from GitHub contributors.
- 📧 **Email Extraction**: Sophisticated scraping and API usage to retrieve public email addresses.
- 📩 **Gmail Integration**: Securely send personalized emails using the official Google Gmail API.
- 📋 **CSV Export**: Generates a clean `email-list.csv` for easy data management and CRM integration.
- 🎨 **HTML Templates**: Use customizable HTML email templates with dynamic placeholders.
- 🛠 **Customizable**: Easily modify templates and sender details to fit your brand.

---

## 🛠 Tech Stack

- **Language**: Python 3.6+
- **APIs**: GitHub API, Gmail API
- **Libraries**: BeautifulSoup4, Requests, LXML, OAuth2Client

---

## 🚀 Getting Started

### 📋 Prerequisites

1.  **Python 3**: Ensure you have Python 3.x installed.
2.  **Gmail API Credentials**: 
    - Follow the [Setup Guide](https://github.com/shankarj67/python-gmail-api/blob/563c7bf722c69be4fed2204e2829d0ab843d8729/README.md#install) to get your `client_secret.json`.
3.  **GitHub Token**: Generate a Personal Access Token from GitHub for higher API rate limits.

### ⚙️ Installation

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/ishandutta2007/reach-github-contributors.git
    cd reach-github-contributors
    ```

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Configure Environment**:
    - Update `constants.py` with your GitHub credentials and API token.
    - Place your `client_secret.json` in the root directory.

---

## 📖 Usage

### 1. Crawl Contributors 🕵️‍♂️
Run the crawler to collect contributor details and save them to `email-list.csv`.
```bash
python3 contributors-crawler.py --repo GITHUB_REPO_FULL_URL
```

### 2. Prepare Your Email 📝
- Modify `request_mail.html` to customize your message.
- Use placeholders like `[fullname]`, `[repo]`, and `[sender]` for personalization.

### 3. Send Emails ✉️
Execute the mailer script to start the outreach process.
```bash
python3 send_mail.py
```

---

## 🤝 Support & Contribution

We love contributions! If you have ideas for improvements or find bugs, feel free to open an issue or submit a pull request.

### ❤️ Support the Project

If you find this tool helpful, consider supporting the developer:

*   [**Paypal**](https://www.paypal.me/ishandutta2007)
*   **Bitcoin**: `3LZazKXG18Hxa3LLNAeKYZNtLzCxpv1LyD`

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHYyeGN5ZjQyeHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/3o7TKMGpxx6D8Yv2ZG/giphy.gif" width="150" alt="Automation Robot">
  <p>Made with ❤️ for the Open Source Community</p>
</div>
