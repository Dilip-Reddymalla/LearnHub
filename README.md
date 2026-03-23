# LearnHub — Online Learning Platform

A static website built for the **Web Programming (WP)** Assignment-I, IV-Semester CSE4, CBIT Hyderabad.

## 🔗 Live Demo

Hosted via GitHub Pages: *(add your link here)*

---

## 📁 Project Structure

```
wp/
├── home.html          # Home page with hero section, features, course preview
├── courses.html       # Courses page — loads course data from XML, modal for details
├── login.html         # Login page with email + password validation
├── signup.html        # Registration page with full form validation
├── contact.html       # Contact page with info cards and validated inquiry form
├── styles.css         # Main stylesheet (home page)
├── courses.css        # Courses page styles
├── login.css          # Login page styles
├── signup.css         # Signup page styles
├── contact.css        # Contact page styles
├── courses.xml        # Course data stored in XML format
├── courses.xsd        # XML Schema Definition to validate courses.xml
└── README.md          # This file
```

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **HTML5** | Page structure and semantic markup |
| **CSS3** | Styling, layout (CSS Grid), hover effects, animations |
| **JavaScript** | Form validation, XML parsing, DOM manipulation |
| **XML** | Storing course data (title, instructor, price, rating, duration, description) |
| **XSD** | Validating the XML structure and data types |
| **Google Fonts** | Inter font for modern typography |
| **GitHub Pages** | Hosting and deployment |

---

## 📄 Pages Overview

### 1. Home (`home.html`)
- Hero section with gradient background, animated floating particles, and stats
- "Why Choose LearnHub" feature cards using CSS Grid
- Popular courses preview section
- Call-to-action section with gradient background

### 2. Courses (`courses.html`)
- Dynamically loads course data from `courses.xml` using JavaScript `fetch()`
- Validates XML structure before rendering
- Clickable course cards open a modal with full details (description, duration, instructor)
- Enroll button in the modal

### 3. Login (`login.html`)
- Email validation using regex
- Password validation (minimum 6 characters)
- Password visibility toggle
- Error messages displayed in real-time

### 4. Sign Up (`signup.html`)
- Full name validation (min 3 letters, alphabets only)
- Email validation using regex
- Password strength check (min 6 characters)
- Confirm password matching
- Password visibility toggle
- Link to login page

### 5. Contact (`contact.html`)
- Contact info cards (Address, Email, Phone)
- Inquiry form with JavaScript validation
  - Name ≥ 2 characters
  - Email regex validation
  - Message ≥ 10 characters

---

## 🎨 CSS Features

- **External stylesheets** — separate CSS file for each page
- **CSS Custom Properties** (variables) for consistent theming
- **CSS Grid** for card layouts and page structure
- **Hover effects** on buttons, links, and cards
- **CSS animations** — fade-in, float, pulse glow
- **Glassmorphic navbar** with backdrop blur
- **Gradient backgrounds** and accent colors
- **Modern typography** using Google Fonts (Inter)

---

## 📦 XML & XSD

### `courses.xml`
Stores 6 courses with the following fields per course:
- `title`, `instructor`, `price`, `rating`, `duration`, `description`

### `courses.xsd`
Validates that:
- Each `<course>` has a required `id` attribute (integer)
- `price` is an integer, `rating` is a decimal
- `title`, `instructor`, `duration`, `description` are strings

---

## ✅ Form Validation (JavaScript)

| Form | Validations |
|------|-------------|
| **Login** | Email regex, password min 6 chars |
| **Sign Up** | Name (min 3 letters), email regex, password min 6, confirm match |
| **Contact** | Name min 2 chars, email regex, message min 10 chars |

---

## 👤 Author

**Dilip Reddy Malla**
B.E/B.Tech CSE4, IV Semester
CBIT (Autonomous), Hyderabad-75
