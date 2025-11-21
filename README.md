# Test Site

## How to run the site locally

1. Open a terminal and navigate to the `test_site` directory:
   ```bash
   cd /Users/vesko/.gemini/antigravity/scratch/test_site
   ```
2. Start the built‑in Python HTTP server bound to all interfaces (so it can be accessed from other machines on the same network):
   ```bash
   python -m http.server 8000 --bind 0.0.0.0
   ```
   This will serve the site at `http://<your‑machine‑ip>:8000/`.
3. Open a web browser on any device (including other machines on the LAN) and navigate to the address above. You should see the **Welcome to the Test Site** page.
4. To test change detection, edit `page2.html` (for example, change the text inside the `<p>` tag), save the file, and refresh the page in the browser. The changes will be visible immediately.

## Notes
- Ensure that your firewall allows inbound connections on port `8000`.
- The server will continue running until you stop it with `Ctrl+C` in the terminal.
