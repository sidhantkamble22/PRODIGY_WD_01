# 🚀 Interactive Navigation Menu — Prodigy InfoTech Task 01

A modern and responsive **Interactive Navigation Menu** developed as part of my **Web Development Internship at Prodigy InfoTech**.

The project demonstrates a fixed navigation bar that dynamically changes its appearance when the user scrolls and provides interactive hover effects on navigation items.

---

## 📌 Task Objective

> Create an interactive navigation menu that changes color or style when scrolled or when hovering over a menu item.

The navigation menu should:

* Remain fixed at the top of the page.
* Stay visible while scrolling.
* Change its style when the page is scrolled.
* Provide hover effects on navigation links.
* Use HTML for structure.
* Use CSS for styling.
* Use JavaScript for interactivity.
* Work across different screen sizes.

---

## ✨ Features

### 🧭 Interactive Navigation

* Fixed navigation bar
* Transparent navbar at the top
* Navbar background changes when scrolling
* Smooth transition effects
* Hover effects on menu items
* Active navigation link indicator

### 📱 Responsive Design

* Desktop navigation menu
* Mobile-friendly hamburger menu
* Responsive layout
* Works on mobile, tablet and desktop screens

### ⚡ JavaScript Interactivity

* Detects page scrolling
* Dynamically adds/removes navbar styles
* Opens and closes mobile navigation
* Updates active navigation section
* Automatically closes the mobile menu after selecting a link

### 🎨 Modern UI

* Dark modern interface
* Responsive typography
* Hover animations
* Interactive cards
* Smooth scrolling
* Clean spacing and layout

---

## 🛠️ Technologies Used

| Technology | Purpose                                      |
| ---------- | -------------------------------------------- |
| HTML5      | Page structure and semantic elements         |
| CSS3       | Styling, responsiveness and animations       |
| JavaScript | Navigation interactions and scroll detection |

---

## 📂 Project Structure

text
PRODIGY_WD_01/
│
├── index.html
├── style.css
├── script.js
└── README.md


### `index.html`

Contains the complete structure of the webpage including:

* Navigation bar
* Hero section
* About section
* Services section
* Projects section
* Contact section
* Footer

### `style.css`

Contains:

* Navbar styling
* Responsive design
* Hover effects
* Animations
* Cards
* Hero section
* Mobile navigation styles

### `script.js`

Handles:

* Navbar scroll effect
* Mobile menu toggle
* Active navigation link
* Closing mobile menu
* Scroll-based section detection

---

## 🧠 How It Works

### 1. Fixed Navigation

The navigation bar uses CSS:

css
position: fixed;
top: 0;
width: 100%;


This keeps the navigation menu visible even when the user scrolls down the page.

---

### 2. Scroll Effect

JavaScript detects the user's scroll position:

window.addEventListener("scroll", () => {
  if (window.scrollY > 50) {
    navbar.classList.add("scrolled");
  } else {
    navbar.classList.remove("scrolled");
  }
});


When the user scrolls more than 50 pixels, the `scrolled` class is added to the navbar.

CSS then changes its appearance:

.navbar.scrolled {
  background: rgba(15, 15, 20, 0.92);
  backdrop-filter: blur(12px);
}


---

### 3. Hover Effect

Navigation links use CSS pseudo-elements to create an animated underline:

css
.nav-link::after {
  transform: scaleX(0);
  transition: transform 0.3s ease;
}

.nav-link:hover::after {
  transform: scaleX(1);
}


This provides visual feedback when the user hovers over a navigation item.

---

### 4. Mobile Navigation

On smaller screens, the normal navigation menu is replaced with a hamburger button.

JavaScript controls the menu:

javascript
menuToggle.addEventListener("click", () => {
  navMenu.classList.toggle("open");
});


This makes the navigation responsive and easy to use on mobile devices.

---

## 📱 Responsive Breakpoint

The project uses a CSS media query for smaller screens:

css
@media (max-width: 768px) {
  /* Mobile styles */
}


The navigation automatically switches to a mobile-friendly menu below this breakpoint.

---

## 🎯 Learning Outcomes

Through this task, I learned and practiced:

* Creating fixed navigation menus
* CSS positioning
* CSS transitions and hover effects
* JavaScript DOM manipulation
* Handling scroll events
* Creating responsive layouts
* Implementing mobile navigation
* Managing active navigation states
* Creating smooth scrolling experiences
* Combining HTML, CSS and JavaScript to build interactive UI

---

## 🚀 How to Run the Project

### 1. Clone the repository

bash
git clone https://github.com/YOUR-USERNAME/PRODIGY_WD_01.git


### 2. Open the project

Navigate to the project folder:

bash
cd PRODIGY_WD_01


### 3. Run the project

Simply open:

text
index.html


in your web browser.

You can also use **VS Code Live Server** for a better development experience.

---

## 🌐 Live Demo

🔗 **Live Demo:**


Example:

text
https://your-project.vercel.app/


---

## 📦 GitHub Repository

🔗 **Repository:**




text
https://github.com/sidhantkamble22/PRODIGY_WD_01


---



## 🏆 Internship Task

**Internship:** Prodigy InfoTech
**Track:** Web Development
**Task:** Task 01
**Repository:** `PRODIGY_WD_01`

---

## 👨‍💻 Author

**Sidhant Kamble**

Web Developer | JavaScript | React.js | Next.js

---

## 📄 License

This project was created for educational and internship purposes as part of the Prodigy InfoTech Web Development Internship.
