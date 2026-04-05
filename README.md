# Laboratory Work No. 3 — Web Technologies

**Topic:** Creating dynamic JavaScript elements and form validation  
**Student:** Ciobanu Stanislav, group CR-221fr  
**Professor:** Lect. Univ. Rusu Viorel  
**Year:** 2024 | Faculty of Computers, Informatics and Microelectronics, TUM

---

## 📋 Description

Practical introduction to client-side JavaScript: DOM manipulation, event handling, and form validation.  

The project consists of an HTML page with multiple interactive features implemented exclusively using JavaScript and CSS, without external libraries.

---

## 🗂️ Project Structure

```
exemplu_JS/
├── index.html # Main page with inline JS code
└── style.css # CSS styles for all components
```

---

## ✨ Implemented Features

### 1. Dropdown Menu
Button with an `onClick` handler that calls `toggleDropdown()` — shows/hides the menu. Styled using CSS hover effects and transitions.

![Dropdown Menu](screenshots/dropdown.png)

---

### 2. Horizontal Image Scroll
Section with horizontal scrolling (`overflow-x: auto`) displaying 3 images loaded via CDN, each with a fixed width of 300px.

---

### 3. Real-Time Clock
`Date` object updated every second using `setInterval(displayTime, 1000)`.  
- **Blue text** in the morning (`hours < 12`)  
- **Red text** in the afternoon  

![Real-Time Clock](screenshots/clock.jpg)

---

### 4. Delayed Message (`setTimeout` / `clearTimeout`)
- `delayMessage()` — requests a delay (in seconds) via `prompt()`, validates input using `parseInt` and `isNaN`, then calls `setTimeout`.  
- `cancelMessage()` — cancels the active timeout using `clearTimeout` after confirmation.

---

### 5. Form Validation (`onSubmit`)
The function `validateForm()` checks fields before submission and returns `true`/`false`:

| Field | Validation Rule |
|---|---|
| Name | Letters and spaces only (regex `/^[a-zA-Z]+...$/`) |
| Email | Valid format with `@` and domain (regex) |
| Phone | Exactly 9 digits (regex `/^\d{9}$/`) |
| Message | Minimum 10 characters |

![Form](screenshots/form.jpg)

![Validation Errors](screenshots/validation.jpg)

---

## 🛠️ Technologies Used

- **HTML5** — page structure, `required` and `pattern` attributes  
- **CSS3** — styling, transitions, hover effects, `overflow-x`  
- **JavaScript (ES5)** — DOM API, events, `setTimeout`, `setInterval`, `clearTimeout`, RegEx  

---

## 🚀 Run

No server or dependencies required. Open directly in your browser:

```bash
# Clone the repository
git clone <url-repo>

# Open the page
open exemplu_JS/index.html
