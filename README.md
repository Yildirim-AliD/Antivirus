# 🛡️ PyQt5-Based Antivirus Application

This project is a simple **GUI-based antivirus scanner** built with Python and PyQt5. It can scan files, directories, or the entire system and displays the scan results in a user-friendly list format. The detection mechanism uses a file called `virus_signatures.txt`, which contains known virus MD5 hashes.

---

## 📁 Project Structure

- `main.py`: Main application logic including the PyQt5 user interface.
- `virus_signatures.txt`: A list of known virus signatures (MD5 hashes).
- `icon.ico`: (Optional) Icon file used in the GUI window.

---

## ⚙️ Requirements

- Python 3.6 or above
- PyQt5

Install dependencies using:

```bash
pip install PyQt5
```

---

## 🚀 Running the Application

Open a terminal in the project directory and run:

```bash
python main.py
```

Once the app is launched, you can:

- **Scan File**: Scan a single file.
- **Scan Directory**: Scan all files in a selected directory.
- **Scan Entire System**: Perform a full system scan starting from the root directory `/`.
- **Schedule Daily Scan**: Set a daily scan time and scan type.

---

## 🧪 Virus Detection

The application calculates the MD5 hash of each scanned file and compares it against entries in the `virus_signatures.txt` file.

**Example entries:**

```
01234c0e41fc23bb5e1946f69e6c6221
018d3c34a296edd32e1b39b7276dcf7f
...
```

Each scan result is listed as either:

- `Dangerous file found: /path/to/file`
- `Clean File: /path/to/file`

---

## ⏰ Daily Scheduled Scans

You can set a specific time and scan type (Full or Directory) for daily scanning. Once configured, the application will automatically trigger the scan every 24 hours at the specified time.

---

## 🖥️ Interface Features

- Dark-themed modern PyQt5 UI
- Scan progress bar
- Result list widget
- Scheduled scan display list
- Popup notifications on completion

---

## ⚠️ Notes

- This is **not a real-time antivirus**.
- MD5 hashing is a simplistic method and should not be relied upon for real-world security.
- Full system scans may require admin privileges and can take a long time.

---

## 👨‍💻 Developer

This project is developed as a personal learning exercise.
