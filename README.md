# Static-Web-Page-Assignment
Personal Webpage  A lightweight, self‑contained personal information web page built with plain HTML and CSS. It demonstrates local file hosting, styling, and network capture for privacy verification.
# Personal Webpage

A lightweight, self‑contained personal information web page built with plain HTML and CSS. It demonstrates local file hosting, styling, and network capture for privacy verification.

## Project Structure

```
personal_webpage/
├── index.html       # Main HTML file
├── styles.css       # Standalone CSS stylesheet
├── profile.jpg      # Placeholder profile image
└── README.md        # This documentation        # This documentation
```

## Prerequisites

- **Ubuntu WSL (Windows Subsystem for Linux)**
- **Python 3** (for the built‑in HTTP server)
- A modern web browser (Chrome, Firefox, Edge, etc.)
- (Optional) VS Code with the Remote – WSL extension for editing

## Installation & Setup

1. **Clone or download** this repository to your local machine:
   ```bash
   git clone https://github.com/<your‑username>/personal_webpage.git
   cd personal_webpage
   ```
2. **(WSL only)** Ensure Ubuntu WSL is installed and running. Update packages:
   ```bash
   sudo apt update && sudo apt install -y python3 tcpdump
   ```
3. **Edit** the files as desired:
   - `index.html`: Update your name, contact details, and profile image path.
   - `styles.css`: Tweak colors, fonts, and responsive breakpoints.

## Serving Locally

Start the HTTP server on port 8000:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/index.html` in your browser.

## Contributing

Feel free to submit issues or pull requests for enhancements, additional styling, or browser support tests.

## License

This project is released under the MIT Licence. See [LICENSE](LICENSE) for details.

## Author

Rachit Jain
94260

