Restricted Phrase Highlighter

A Tampermonkey userscript that automatically detects and highlights restricted phrases on Amazon CP Central pages in real time.

🔍 What This Does
Scans page content dynamically
Highlights restricted phrases instantly
Works even with dynamically loaded content
Uses a centralized phrase list (JSON)
Automatically updates for all users

🧠 How It Works
The script fetches a list of restricted phrases from a hosted JSON file
Builds an optimized regex from all phrases
Scans the page content

Highlights matches using visual markers
📁 Project Structure
restricted-phrases/
│
├── restricted_phrases.json   # Master phrase list
├── README.md                 # Documentation


🚀 Setup Guide
1. Install Tampermonkey
Chrome: https://www.tampermonkey.net/
Edge / Firefox supported
2. Add the Script
Open Tampermonkey
Click Create New Script
Paste the provided script

3. Save & Enable
Save the script
Ensure it is enabled
Open CP Central → phrases will highlight automatically
🌐 Supported Pages
https://www.cp-central.catalog.amazon.dev/*
https://www.beta.cp-central.catalog.amazon.dev/*

✏️ Updating Restricted Phrases
Open restricted_phrases.json in GitHub
Click Edit
Add/remove phrases
Commit changes
Changes apply automatically for all users (within cache duration)

⚡ Performance Notes
Uses a single optimized regex for all phrases
Cached locally for faster load
Auto-refreshes every 24 hours

⚠️ Limitations
Requires public access to JSON file
Extremely large phrase sets may impact performance
SharePoint-hosted files may not work due to CORS/auth restrictions

🔒 Security Note
Do not include sensitive or confidential data in the public JSON file
If required, use internal hosting instead of GitHub

🧩 Future Enhancements (Optional)
Violation counter (e.g., “⚠️ 10 matches found”)
Navigation between highlights
Severity-based color coding
Toggle ON/OFF UI

👤 Maintainer
adisba

💬 Final Note
This tool is designed to act as a lightweight, real-time compliance layer inside your workflow.
Keep the phrase list clean and updated — everything else runs automatically.
