# ESFM
ESFM is a OS-Like enviroment for your ESP32-WROOM-32
🛠️ How to Install ESFM (Espian) on Your ESP32-WROOM-32
✅ Tested only on Thonny. Other tools may work, but use at your own risk.

🧰 Requirements:
- ESP32-WROOM-32 board

- [Thonny IDE](https://thonny.org/)

- [esptool.py](https://github.com/espressif/esptool) installed

- MicroPython firmware from here

📦 Install Steps:
1. Flash MicroPython firmware using esptool:

      esptool.py --chip esp32 --port COMx erase_flash
      esptool.py --chip esp32 --port COMx --baud 460800 write_flash -z 0x1000 esp32-xxxxxx.bin

      Replace **COMx** with your actual port (e.g., COM3)
      Replace **esp32-xxxxxx.bin** with your downloaded MicroPython firmware.

2. Download the latest ESFM release ZIP
       👉 [Go to Releases](https://github.com/KADARNALPHA/ESFM/releases)

3. Extract the archive

4. Open Thonny IDE

5. Select MicroPython (ESP32) as interpreter

6. Connect your ESP32 board

7. Upload all extracted files

8. Drag and drop the files into the root of your ESP32 using Thonny’s file browser.

9. Configure your account

     Open /usr/.usrs

     You’ll see a line like:
         acc:acc

     Change it to:
         your_username:your_password

10. Set up sudo access

     Open /etc/sudoers

     Replace adam with your username from step 9

     Reboot the board

     Login screen will appear

     Enter your username

     Enter your password
