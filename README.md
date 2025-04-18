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

## Code Overview

### `index.html`

- **DOCTYPE & meta**: HTML5 document with UTF-8 charset for wide character support.
- **Link to CSS**: `<link rel="stylesheet" href="styles.css">` ensures separation of concerns.
- **Header Section**: Contains `<h1>` with the page title.
- **Profile Image**: Wrapped in a `<section>` with an `<img>` tag sourcing `profile.jpg`.
- **Contact Info**: Uses `<section>` and semantic `<h2>` and `<p>` tags; includes address, phone, email, and Matrix ID.

Example snippet:
```html
<section id="contact-info">
  <h2>Contact Information</h2>
  <p><strong>Address:</strong> 123 Main Street, Berlin, Germany</p>
  <p><strong>Phone:</strong> +49 30 1234567</p>
  <p><strong>Email:</strong> jane.doe@example.com</p>
  <p><strong>Matrix ID:</strong> @janedoe:matrix.org</p>
</section>
```

### `styles.css`

- **Global Styles**: Defines font stack, background gradient, and base color.
- **Header Styling**: Background color, text centering, shadows, and typography enhancements.
- **Image Effects**: Circular cropping, border, shadow, and scale-on-hover transitions.
- **Contact Card**: Centered container with padding, rounded corners, hover shadow effect, and responsive width.
- **Responsive Breakpoints**: Adjusts header font size and padding for screens ≤600px.

Example snippet:
```css
#profile-pic img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    transition: transform 0.3s ease;
}

#profile-pic img:hover {
    transform: scale(1.05);
}
```

## Installation & Setup & Setup

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

