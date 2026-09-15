ARFAT HOST - FIXED

Run locally/Pydroid:
1. Install requirements.txt
2. Run: python app.py
3. Open http://127.0.0.1:5000

Default admin login from the original database initialization:
username: neverexits
password: 1100

Important startup fix:
- Uploaded .py/.js files are stored under storage/instances/<instance>/
- START resolves the startup file inside that instance.
- Old absolute startup paths are converted automatically.
- If main.py is missing, the first .py/.js file in the instance root is selected.
- Python uses the same interpreter that runs the panel (important for Pydroid/Android).
