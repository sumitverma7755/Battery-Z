# Battery-Z ![image](https://github.com/sumitverma7755/Battery-Z/blob/main/logo.ico)

![image](https://github.com/user-attachments/assets/1078d85f-667a-492f-bb17-3b595c37a30d)
 <!-- Placeholder for your screenshot -->

**Battery-Z: Your Laptop’s Battery Companion, Built with Precision and Care**  
Battery-Z is an open-source, cross-platform battery monitoring and optimization tool designed to empower users with deep insights into their laptop’s battery health and performance. Crafted with ❤️ by [Sumit Kumar Verma](https://github.com/sumitverma7755), Battery-Z combines advanced diagnostics, intuitive visualizations, and actionable tips to extend battery life and enhance user experience. Whether you’re a casual user, a developer, or a power enthusiast, Battery-Z is your go-to solution for keeping your laptop’s battery in top shape! 🌟
---

## 🚀 Features

Battery-Z offers a robust suite of features to monitor, analyze, and optimize your laptop’s battery:

### 📊 Comprehensive Battery Monitoring
- **Real-Time Stats**: Tracks battery percentage, charging state, estimated time remaining, and power consumption with precision. ⚡
- **Detailed Hardware Info**: Retrieves critical battery details, including manufacturer, serial number, chemistry, design capacity, and full charge capacity. 🛠️
- **Cycle Count Analysis**: Accurately measures battery cycle counts using multiple methods (WMIC, WMI, Powercfg, ACPI, and charge log estimation). 🔄
- **Health Assessment**: Calculates battery health based on cycle count and capacity retention, with clear visual indicators (Good, Moderate, Poor). 📈

### 🖥️ Intuitive User Interface
- **Modern Design**: Sleek, customizable UI with Dark and Light themes for a personalized experience. 🌙☀️
- **Animated Visuals**: Dynamic battery health and charge level widgets with glowing effects for real-time feedback. ✨
- **System Tray Integration**: Stay informed with system tray notifications for low battery, poor health, or high temperatures. 🔔
- **Battery History Visualization**: Interactive graphs to track battery percentage over time using Matplotlib. 📉

### 🛠️ Advanced Diagnostics
- **Multi-Source Data Collection**: Combines data from Powercfg, WMI, ACPI, and system registry for unparalleled accuracy. 🔍
- **Cycle Count Calibration**: Manual calibration option for users when automatic detection is uncertain. ⚙️
- **Temperature Monitoring**: Tracks battery temperature to prevent overheating, with alerts for critical thresholds. 🌡️
- **Charge Log Analysis**: Logs charge events to estimate cycle counts and predict battery lifespan. 📝

### 💡 Optimization Tips
- **Actionable Advice**: Curated tips to extend battery life, such as avoiding full discharges and optimizing charge cycles. 🧠
- **Dynamic Suggestions**: Rotates through practical recommendations tailored to your battery usage patterns. 🔄

### 📂 Data Persistence
- **Local Storage**: Saves battery history, charge logs, and cycle count data in the user’s AppData directory for long-term tracking. 💾
- **Efficient Logging**: Uses rotating file handlers to manage log files, ensuring minimal disk usage. 🗂️

---

## 🎯 Why Battery-Z?

Battery-Z stands out as a powerful, user-friendly tool designed to demystify battery management:

- **Precision-Driven**: Leverages multiple data sources (Powercfg, WMI, ACPI, and more) to ensure accurate and reliable battery insights. ✅
- **User-Centric**: Crafted with a focus on ease of use, featuring a polished UI and heartfelt messages to engage users. ❤️
- **Open Source**: Freely available for community contributions, with a clear structure for developers to enhance and extend. 🌍
- **Cross-Platform Ready**: Built with Python and PyQt5, ensuring compatibility with Windows (with plans for future platform support). 🖥️

---

## 🛠️ Technical Details

Battery-Z is built with a modular architecture, ensuring maintainability and scalability:

### 🔧 Core Components
- **BatteryIntelligence Class**: The backbone of battery data collection, processing, and analysis. It consolidates data from multiple sources and provides robust fallback mechanisms. 🧠
- **BatteryWidget**: Custom PyQt5 widget for visualizing battery health and charge levels with animated, glowing effects. 🎨
- **System Tray Integration**: Uses QSystemTrayIcon for real-time notifications and quick access to app features. 🔔
- **History Visualization**: Integrates Pandas and Matplotlib for plotting battery percentage trends over time. 📊

### 🧑‍💻 Technologies Used
- **Python 3.x**: Core programming language for logic and data processing. 🐍
- **PyQt5**: For building a responsive, cross-platform GUI with advanced animations. 🖼️
- **psutil**: For real-time battery status monitoring. ⚡
- **wmi**: For accessing Windows Management Instrumentation data. 🛠️
- **ctypes**: For low-level ACPI queries to retrieve detailed battery information. 🔌
- **Pandas & Matplotlib**: For data analysis and visualization of battery history. 📈
- **BeautifulSoup**: For parsing Powercfg HTML reports as a fallback data source. 📜
- **Logging**: Comprehensive logging with rotating file handlers for debugging and monitoring. 📝

### 📋 System Requirements
- **OS**: Windows 10 or later (admin privileges required for full functionality). 🖥️
- **Dependencies**: Install via `requirements.txt` (see Installation section). 📦
- **Hardware**: Laptop with a supported battery (most modern laptops are compatible). 🔋

---

## 📦 Installation

 ### Method 1: 
  ---- > Just download and open the [.EXE File](https://github.com/sumitverma7755/Battery-Z/releases/download/Laptop-Battery-Tool/Battery-Z.exe) from Github.

 ### Method 2 [ Manual ]:
 Get Battery-Z up and running in just a few steps:

 1. **Clone the Repository**:
    ```bash
    git clone https://github.com/sumitverma7755/Battery-Z.git
    cd Battery-Z
    ```

2. **Install Dependencies**:
   Ensure you have Python 3.x installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   ```bash
   python battery_z.py
   ```

4. **Optional**: Build an executable using PyInstaller for standalone distribution:
   ```bash
   pyinstaller --onefile --icon=logo.ico battery_z.py
   ```

> **Note**: Battery-Z requires administrative privileges for certain low-level operations (e.g., ACPI queries). Run the app as an administrator for full functionality. 🛡️

---

## 🖱️ Usage

Battery-Z is intuitive and packed with features to make battery management a breeze:

1. **Launch the App**: Start Battery-Z to see a sleek dashboard with real-time battery stats. 🚀
2. **Monitor Health**: View battery health, cycle count, and estimated lifespan in the Health Check section. 📊
3. **Check History**: Open the Battery History dialog to visualize percentage trends over time. 📉
4. **Apply Tips**: Browse optimization tips to extend your battery’s life. 💡
5. **Customize**: Switch between Dark and Light themes via the View menu. 🌙☀️
6. **Calibrate**: Use the Cycle Count Calibration dialog if automatic cycle detection is uncertain. ⚙️
7. **Stay Notified**: Receive system tray alerts for low battery, poor health, or high temperatures. 🔔

---

## 🌟 Contributing

Battery-Z is an open-source project, and we welcome contributions from the community! Here’s how you can help:

- **Report Bugs**: Found an issue? Open a detailed bug report on the [Issues](https://github.com/sumitverma7755/Battery-Z/issues) page. 🐞
- **Suggest Features**: Have an idea to make Battery-Z even better? Share it in the Issues section. 💡
- **Submit Pull Requests**: Fork the repo, make your changes, and submit a pull request. Ensure your code follows PEP 8 guidelines and includes tests. 🛠️
- **Improve Documentation**: Help enhance this README or add in-code documentation for better clarity. 📝

### Contribution Guidelines
1. Fork the repository and create a new branch (`feature/your-feature-name` or `bugfix/issue-number`).
2. Ensure your changes are well-documented and tested.
3. Submit a pull request with a clear description of your changes and their purpose.
4. Follow the [Code of Conduct](CODE_OF_CONDUCT.md) to maintain a respectful and inclusive community. 🤝


## 🙌 Acknowledgments

- **Sumit Kumar Verma**: The creator and lead developer, pouring ❤️ into every line of code.  
- **Open-Source Community**: For inspiring tools and libraries that made Battery-Z possible. 🌍
- **Users**: For trusting Battery-Z to care for your laptop’s battery. You’re the reason we keep going! 😊

---

## 📬 Contact

Have questions or want to connect? Reach out to the creator:  
- **GitHub**: [sumitverma7755](https://github.com/sumitverma7755)  
- **LinkedIn**: [Sumit Kumar Verma](https://www.linkedin.com/in/sumit-kumar-verma-a24a7a184/)  
- **Support**: Open an issue or join the [Discussions](https://github.com/sumitverma7755/Battery-Z/discussions) page. 📩

Want to show some love? [Buy me a coffee ☕](https://github.com/sumitverma7755/Battery-Z) to support the project! 

---

**Battery-Z: Powering your laptop with insights and care. Let’s keep your battery thriving!** ![image](https://github.com/sumitverma7755/Battery-Z/blob/main/logo.ico)✨
