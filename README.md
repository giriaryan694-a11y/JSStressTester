JSStressTester - README.txt
----------------------------

JSStressTester
--------------
A lightweight, browser-based educational request simulator for authorized load testing.
Runs purely client-side (no installation). Ideal for demos, labs, and learning how repeated
requests affect server logs and behavior.

Key points
----------
- 100% client-side HTML/JS (open index.html in a browser or host on GitHub Pages).
- Uses browser-friendly techniques (image requests) so each hit shows up in server logs.
- No backend required. No installation. Works from GitHub Pages: https://giriaryan694-a11y.github.io/JSStressTester/

Features
--------
- Target URL input
- Number of requests
- Adjustable delay (ms) between requests
- Start / Stop controls
- Live request log in the browser
- Footer credit + legal warning

Usage (quick)
-------------
1. Host `index.html` on GitHub Pages or open it locally in a browser.
2. Enter the target URL (only systems you own or are authorized to test).
3. Set "Number of Requests" and "Delay (ms)".
4. Click START. Monitor server logs to see incoming requests.
5. Click STOP to halt the test.

Important technical notes
-------------------------
- The tool uses dynamic image requests (new Image()) with unique query strings
  (e.g., ?req=1&ts=...). This makes the browser send a real HTTP request each time
  even when CORS would block fetch/XHR.
- Browsers will NOT allow spoofing the User-Agent header from client JS.
- Results may be affected by browser caching, CDN/WAF protections, or the target's server config.

Legal & Ethical Warning (READ CAREFULLY)
----------------------------------------
⚠️ THIS TOOL IS FOR EDUCATIONAL PURPOSES AND AUTHORIZED TESTING ONLY.
Do NOT use JSStressTester against any system, network, or service you do NOT own
or do not have explicit written permission to test. Misuse (including generating
fake traffic, ad/analytics fraud, or denial-of-service) is ILLEGAL and can result
in criminal charges, civil liability, and law enforcement action.
The developer (Aryan Giri) is NOT RESPONSIBLE for any misuse.

Hosting note
------------
Recommended: host on GitHub Pages for easy access:
https://giriaryan694-a11y.github.io/JSStressTester/
License
-------
MIT License (see LICENSE file if included).

Credits
-------
Developed by: Aryan Giri

----------------------------
Made by Aryan Giri | Use responsibly
----------------------------
