# 🌦 A Weather Bot using Python 🌦

A Python script that emails daily weather details for a specified city and reminds you to bring an umbrella if rain is forecasted.

---

## 📋 Features
- **🌞 Daily Weather Update**: Receives a daily email with the weather update for your chosen city.
- **🌧️ Umbrella Reminder**: Adds a reminder to bring an umbrella if rain or showers are forecasted.
- **🕰️ Scheduling**: Automatically schedules the notification to be sent every day at a specified time (6:00 AM by default).

---

## 🚀 Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/daily-weather-notifier.git
    cd daily-weather-notifier
    ```

2. **Install Required Packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Update Email Credentials**:
    - Open `send_weather_email.py`.
    - Replace `"YOUR EMAIL"` and `"PASSWORD"` with your email credentials.
    - Replace `"FROM EMAIL"` and `"TO EMAIL"` with the sender and recipient emails respectively.
    - Make sure your email account settings allow access to third-party applications.

---

## 💻 Usage

- **Run the Script**:
    ```bash
    python send_weather_email.py
    ```
- The script will run in the background and automatically send a daily weather email at 6:00 AM, with a reminder to bring an umbrella if rain is forecasted.

---

## ⚙️ Customization

- **🌆 Change the City**:
  - Update the `city` variable in `send_weather_email()` with your preferred city.

- **⏰ Change the Schedule Time**:
  - Modify the line `schedule.every().day.at("06:00").do(send_weather_email)` to set a different time.

---

## 📦 Dependencies

- `schedule` - for setting up daily reminders
- `smtplib` - (pre-installed with Python) for email functionality
- `requests` - for fetching weather data from Google search results
- `BeautifulSoup` (from `bs4`) - for parsing HTML to extract weather information

---

## 🙏 Acknowledgments

This project was inspired by the need for quick and easy daily weather updates. Special thanks to:

- The developers and maintainers of **BeautifulSoup** and **Requests**, for making web scraping in Python efficient and user-friendly.
- The creators of **Schedule**, for simplifying task scheduling in Python.
- The open-source community, for their continuous support, resources, and contributions.
- And lastly @vinayedula from GEEKSFORGEEKS for a [step by step](https://www.geeksforgeeks.org/user/vinayedula/contributions/?itm_source=geeksforgeeks&itm_medium=article_author&itm_campaign=auth_user) guide.

This project wouldn’t be possible without the support of these tools and the valuable resources available in the developer community.

---
