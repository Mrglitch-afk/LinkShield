LinkShield
Free, instant URL safety scanner. Paste any link to detect phishing, spoofing, and malicious patterns before you click.

100% client-side. No data leaves your browser. No sign-up required.

https://linkshield-app.netlify.app


<img width="96" height="20" alt="image" src="https://github.com/user-attachments/assets/6ed8f7fd-cc30-44bc-b2d5-7275f103f489" />
<img width="88" height="20" alt="Status-Active-brightgreen" src="https://github.com/user-attachments/assets/3b136024-e287-4c69-80b7-0bd62ee93942" />
<img width="124" height="20" alt="image" src="https://github.com/user-attachments/assets/84dee9ec-b82b-4f0c-866d-eac67cdb5449" />
<img width="82" height="20" alt="image" src="https://github.com/user-attachments/assets/9ea1bdd6-b0dd-4cd0-9c6b-2a61a14fe694" />

StatusPrivacyZero BackendSize

Why LinkShield?
Most "is this link safe" tools send your URLs to a backend server for analysis. That means the service provider sees every link you check. LinkShield does all analysis locally using JavaScript heuristics.

It is designed to be a fast, private first-line filter, especially useful for checking links that contain sensitive tokens, internal company URLs, or when you simply don't want your browsing habits logged.

Detection Heuristics
LinkShield runs 16 structural checks against the URL:

Identity & Spoofing

Brand Impersonation: Catches leetspeak variants (e.g., g00gle, payp4l)
Punycode/Homograph Attacks: Flags xn-- encoded domains used to spoof characters
Credential Stuffing: Detects the user@host trick to hide real destinations
Structural Analysis

Suspicious TLDs: Scores high-risk extensions (.xyz, .tk, .top, .click)
Subdomain Depth: Flags obfuscation via excessive subdomains (secure.login.fake.xyz)
URL Shorteners: Identifies bit.ly, tinyurl (where the destination is hidden)
URL Length: Flags abnormally long, obfuscated URLs
Domain Hygiene: Scores excessive hyphens and numbers in the domain name
Double File Extensions: Flags .pdf.exe or .doc.bat malware delivery
Security & Privacy

Protocol Check: Flags unencrypted HTTP connections
Non-Standard Ports: Flags custom ports rarely used by legitimate sites
Sensitive Parameters: Flags tokens, passwords, and API keys exposed in query strings
Character Encoding: Flags excessive %XX encoding used to disguise text
Data URI Check: Detects data: scheme script execution risks
Suspicious Keywords: Flags urgency words ("verify", "suspend", "refund")
IP Host Check: Flags raw IP addresses instead of domain names
Output
Every scan generates:
<img width="1214" height="560" alt="Screenshot 2026-07-02 141911" src="https://github.com/user-attachments/assets/2e2d5b01-c22b-4e6d-b92b-2e8562c29af1" />
<img width="1220" height="565" alt="Screenshot 2026-07-02 141946" src="https://github.com/user-attachments/assets/fd08108c-a3b6-4cf0-8958-c16047f0c754" />
<img width="1207" height="470" alt="Screenshot 2026-07-02 142007" src="https://github.com/user-attachments/assets/81f18211-97fb-4ca0-b5a8-3b457538f1aa" />
A 0-100 Safety Score with a color-coded gauge
A URL Anatomy Breakdown (color-coded protocol, subdomain, domain, TLD, path, query)
Detailed Findings explaining exactly why each flag was raised
Usage
Because it is a single HTML file with zero dependencies, you don't need Node.js, Python, or a web server.

Online:Just visit the Live Demo and paste a URL.

Locally (Works Offline):

Download index.html from this repository.
Double-click the file to open it in any modern browser.
It runs entirely offline.

Tech Stack
Vanilla HTML5 / CSS3 / JavaScript
Zero external dependencies
Zero backend / Zero database
Total size: ~15KB

License
This project is open source and available under the MIT License.


