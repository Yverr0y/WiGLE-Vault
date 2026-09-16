<div align="center">

<img width="100%" alt="WIGLE VAULT" src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:5C227A&height=220&section=header&text=WIGLE%20VAULT&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Cross-platform%20%7C%20Python%20%7C%20WiGLE%20%7C%20Backup&descSize=16&descAlignY=58"/>

`Cross-platform` [`Python`](https://www.python.org/) [`WiGLE`](https://wigle.net/) `Backup` - Download all your WiGLE wardriving data in one command. Simple Python tool for backing up your WiFi survey history.

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=20&pause=1000&color=5C227A&center=true&vCenter=true&multiline=true&repeat=true&width=950&height=90&lines=Download+all+your+WiGLE+wardriving+data+in+one+command%3BCross-platform+%2F+Python+%2F+WiGLE+%2F+Backup)](https://git.io/typing-svg)

<br>

[![Project](https://img.shields.io/badge/Project-WiGLE--Vault-5C227A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ringmast4r/WiGLE-Vault)
[![Format](https://img.shields.io/badge/Format-Python-000000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ringmast4r/WiGLE-Vault/tree/main)

[![Stars](https://img.shields.io/github/stars/Ringmast4r/WiGLE-Vault?style=flat-square&color=5C227A)](https://github.com/Ringmast4r/WiGLE-Vault/stargazers)
[![Forks](https://img.shields.io/github/forks/Ringmast4r/WiGLE-Vault?style=flat-square&color=5C227A)](https://github.com/Ringmast4r/WiGLE-Vault/network/members)
[![Repo Size](https://img.shields.io/github/repo-size/Ringmast4r/WiGLE-Vault?style=flat-square&color=5C227A)](https://github.com/Ringmast4r/WiGLE-Vault)
[![Last Commit](https://img.shields.io/github/last-commit/Ringmast4r/WiGLE-Vault?style=flat-square&color=5C227A)](https://github.com/Ringmast4r/WiGLE-Vault/commits/main)

</div>

---

# WiGLE Vault 🛰️

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.6+-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)
![Maintenance](https://img.shields.io/badge/maintained-yes-green.svg)

Download ALL your WiGLE wardriving data in one command.

---

<a id="-quick-start-choose-your-method"></a>
## `> quick_start_choose_your_method`

### Option A: Pre-Built Executables (No Coding Required!)

**Perfect for non-technical users!**

#### Windows
1. Download `WiGLE-Vault-Windows.zip` from the [Releases page](https://github.com/Ringmast4r/WiGLE-Vault/releases)
2. Extract the ZIP file
3. Double-click `RUN_ME.bat` (or `WiGLE-Vault.exe`)
4. Paste your WiGLE token when prompted
5. Press ENTER and wait for downloads to complete

#### macOS
1. Download `WiGLE-Vault-macOS.zip` from the [Releases page](https://github.com/Ringmast4r/WiGLE-Vault/releases)
2. Extract the ZIP file
3. Double-click `run.sh` (or run `./WiGLE-Vault` in Terminal)
4. Paste your WiGLE token when prompted
5. Press ENTER and wait for downloads to complete

**Note for macOS users:** First time running, you may need to allow the app in System Preferences > Security & Privacy

**Features:**
- ✅ No Python installation needed
- ✅ Single-click execution
- ✅ Automatic progress tracking
- ✅ Resumes interrupted downloads
- ✅ Complete instructions included
- ✅ Works on Windows and macOS

📖 See the included instructions in the download for detailed help.

---

### Option B: Python Script (For Developers)

<a id="how-to-use-3-steps"></a>
## `> how_to_use_3_steps`

### Step 1: Run the Script

```bash
python wigle_vault.py
```

### Step 2: Get Your Token When Prompted

The script will ask you to:
1. Visit https://wigle.net/account
2. Click **"Show my token"**
3. Copy the **"Encoded for use"** value
4. Paste it into the command prompt

### Step 3: Done!

All your CSVs download to the `vault` folder.

**💡 Download Interrupted or Failed?**
Just run the script again! It automatically skips files that already exist. Only missing files get downloaded.

**Works for:**
- Network timeouts
- Power loss
- Accidentally closing the window
- Large files that timed out

No wasted bandwidth. No duplicate downloads.

---

**Advanced:** You can also provide the token as an argument:
```bash
python wigle_vault.py YOUR_TOKEN_HERE
```

---

<a id="what-you-need"></a>
## `> what_you_need`

- Python 3.6 or newer
- `requests` library (install: `pip install requests`)

---

<a id="what-it-does"></a>
## `> what_it_does`

- Downloads every CSV file you ever uploaded to WiGLE
- Handles files of ANY size (even 100+ MB cross-country logs)
- Skips files that already exist (fully resumable)
- Shows progress as it downloads
- Works on Windows, Mac, Linux
- Streaming downloads for memory efficiency

---

<a id="example-output"></a>
## `> example_output`

```
============================================================
🛰️  WiGLE Vault - Wardriving Data Backup Tool
    Version 1.0.0
============================================================
📂 Download location: C:\Users\You\wigle_backup

📄 Fetching page 1...
   Found 43 transaction(s) on this page
   ⬇️  Downloading 12345678.csv... ✅ (1,234,567 bytes)
   ⬇️  Downloading 12345679.csv... ✅ (987,654 bytes)
   ⏭️  Skipping 12345680.csv (already exists, 2,345,678 bytes)
   ...

============================================================
🎉 Download Complete!
============================================================
📊 Total uploads found:        43
⬇️  Successfully downloaded:   42
⏭️  Skipped (already existed): 1
💾 Total data size:            52,345,678 bytes (49.92 MB)
📂 Location:                   C:\Users\You\wigle_backup

💡 Next Steps:
   • Import these CSVs into your GIS software or analysis tools
   • Backup these files to cloud storage
   • Keep them safe - this is YOUR wardriving history!
```

---

<a id="requirements"></a>
## `> requirements`

- **Python 3.6+**
- **requests library** (install with `pip install requests`)

---

<a id="use-cases"></a>
## `> use_cases`

### 📊 Data Analysis
Import your CSVs into tools like:
- **QGIS** - Geographic information system
- **Excel/Google Sheets** - Spreadsheet analysis
- **Python/R** - Custom data science workflows
- **Wireshark** - Network analysis and mapping

### 💾 Backup Strategy
- Keep local copies of your wardriving history
- Archive data before deleting from WiGLE
- Migrate data to other platforms
- Share datasets with research teams

### 🔒 Privacy & Control
- Your data belongs to you
- No vendor lock-in
- Full offline access
- Complete data portability

---

<a id="installation"></a>
## `> installation`

### Option 1: Direct Download
```bash
# Download the script
curl -O https://raw.githubusercontent.com/Ringmast4r/WiGLE-Vault/main/wigle_vault.py

# Install dependencies
pip install requests

# Run it
python wigle_vault.py <your-token>
```

### Option 2: Clone Repository
```bash
git clone https://github.com/Ringmast4r/WiGLE-Vault.git
cd WiGLE-Vault
pip install -r requirements.txt
python wigle_vault.py <your-token>
```

---

<a id="common-questions"></a>
## `> common_questions`

**Is this safe?**
Yes - uses official WiGLE API, read-only access, open source code.

**Can anyone intercept my data?**
NO! Direct HTTPS connection to WiGLE servers. Your data goes straight from WiGLE to your computer - nobody in between.

**Can I stop and resume?**
YES! Just run it again. It will skip every file that already downloaded and only grab what's missing. Works even if:
- Your internet cuts out
- A large file times out
- You accidentally close the window
- Your computer restarts

**How long does it take?**
Depends on file sizes. Small files = 1-2 seconds. Massive 100+ MB logs might take a few minutes each. 100 uploads usually takes 5-10 minutes total.

**Keep token secret?**
YES! Don't share it, don't commit it to git.

---

<a id="problems"></a>
## `> problems`

**401 Error** - Wrong token. Copy "Encoded for use" (not plain token).

**Network Error** - Check internet connection, try again later.

---

<a id="license"></a>
## `> license`

MIT License

Created by Ringmast4r for the wardriving community.

---

<div align="center">

<img width="100%" alt="WIGLE VAULT footer" src="https://capsule-render.vercel.app/api?type=waving&color=0:5C227A,100:000000&height=120&section=footer&text=RINGMAST4R%20%2F%2F%20BACKUP&fontSize=18&fontColor=ffffff&fontAlignY=65"/>

</div>
