import webbrowser
import time

# URL you want to auto-refresh
url = ""

# Settings
refresh_interval = 10    # Set refresh interval in seconds
max_refreshes = 5        # Total number of times to refresh

# Refresh loop
for i in range(max_refreshes):
    print(f"Refresh {i+1} of {max_refreshes}")
    
    # Open the URL in the default web browser
    webbrowser.open(url)
    
    # Wait for the specified interval
    time.sleep(refresh_interval)

print("Auto-refresh complete.")
