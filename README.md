# 🍪 Automated Cookie Clicker Bot (Selenium Python)

A Python automation project that plays the classic Cookie Clicker game (Orteil version) automatically. Using Selenium, the bot clicks the cookie at high speeds and intelligently purchases the most expensive upgrades it can afford every 5 seconds to maximize production.

This project demonstrates browser automation, DOM manipulation, real-time data scraping, and automated decision-making logic.

---
## Images 

<img width="1019" height="643" alt="image" src="https://github.com/user-attachments/assets/a7b16df7-c031-4f62-adcd-08ead761eef8" />


## 🚀 Features

- ⚡ High-speed automated clicking using Selenium
- 💰 Real-time monitoring of cookie balance (money)
- 🛒 Automated store scanning and price parsing
- 🧠 Intelligent purchasing logic (always buys the highest affordable upgrade)
- ⏲️ Timed execution with a 5-minute auto-stop
- 📊 Final performance reporting (Cookies Per Second - CPS)

---

## 🛠 Technologies Used

- Python 3
- Selenium WebDriver
- Chrome WebDriver
- Time Library (Standard Python)

---

## 📂 Project Structure
```bash
cookie/
│
├── main.py           # Main automation script
├── .gitignore        # Git ignored files
│
└── README.md
```
---

## ⚙️ Requirements

Ensure Python is installed:
python --version

Install Selenium:
pip install selenium

Note: You must have Chrome installed and a compatible version of ChromeDriver.

---

## 🚀 How to Run the Project

### Clone the Repository
git clone https://github.com/adebayoadesugba/Bot-with-Selenium.git

### Navigate into the Project Folder
cd cookie

### Run the Script
python main.py

---

## ⚙️ How It Works

1️⃣ The script initializes the Selenium WebDriver and navigates to the game URL.

2️⃣ It identifies the cookie element and the list of available items in the store using CSS selectors.

3️⃣ A "While True" loop executes two main actions:
   - Continuously clicks the cookie to generate currency.
   - Every 5 seconds, it pauses clicking to check the store.

4️⃣ Store Logic:
   - Scrapes all prices from the store sidebar.
   - Compares the current "money" balance to the prices.
   - Selects the upgrade with the highest cost that the bot can currently afford.
   - Clicks the upgrade to increase "Cookies Per Second" (CPS).

5️⃣ After 5 minutes, the bot stops, prints the final CPS to the console, and waits for user input to close the browser.

---

## 📊 Example Output

43500
125000
500000
Cookies per second: 154.6

---

## ⚠️ Security Warning

- Ensure the path to your 'chromedriver.exe' is correctly set in the script.
- Be aware that high-frequency clicking scripts can be resource-intensive for your CPU.
- Never share personal browser profile paths if they contain sensitive session cookies.

---

## 🧠 Key Concepts Demonstrated

- Browser automation (Webdriver)
- Dynamic element locating (ID, CSS Selectors)
- Data parsing (String manipulation and type casting)
- Algorithmic decision making (Max value selection)
- Loop timing and execution control

---

## 🔮 Future Improvements

- Add support for "Golden Cookies" (random screen pop-ups)
- Implement a more complex strategy (e.g., calculating Return on Investment for upgrades)
- Run the browser in "headless" mode for faster performance
- Create a GUI to adjust the check-in intervals

---

## 👨‍💻 Author

Adebayo Adesugba (Dev Bayo)

Full Stack Developer  
Python | JavaScript | React | Node.js | AI Development  

---

## ⭐ Support

If you like this project:
- ⭐ Star the repository
- 🍴 Fork it
- 🧑‍💻 Contribute

---

## 📜 License

This project is open-source and available under the MIT License.
