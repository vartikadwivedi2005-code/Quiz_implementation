```markdown
# 🧠 Interactive Quiz Web Application

A sleek, responsive, and interactive frontend Quiz Application built using vanilla **HTML5**, **CSS3**, and **Modern JavaScript (ES6+)**. The application features an integrated countdown timer per question, real-time score tracking, dynamic UI updates, and an automated feedback summary screen based on completion performance.

---

## 🚀 Features

* **Dynamic Question Rendering:** Questions and response choices are injected dynamically using JavaScript DOM manipulation methods.
* **Active Countdown Timer:** Gives players exactly 15 seconds per question. Automates a "Time's Up" transition to show correct options if the countdown hits zero.
* **Instant Visual Feedback:** Highlights selected responses in Green (`correct`) or Red (`wrong`) immediately upon clicking, while automatically illuminating the correct option if the user guesses incorrectly.
* **State Protection:** Prevents multi-clicking or changing answers once a choice has been finalized.
* **Adaptive Performance Evaluation:** Summarizes final scores and displays unique, encouraging contextual messages based on the final percentage achieved.
* **Fully Responsive Stylesheet:** Features clean typography, geometric hover micro-interactions, smooth layouts, and beautiful linear-gradient design elements tailored across universal desktop and mobile screen resolutions.

---

## 📂 File Architecture

The codebase contains a clean separation of concerns spread across 3 primary workspace files:

```bash
├── index.html       # Structural layout, UI views, and DOM container elements
├── styles.css       # Layout styles, absolute center positioning, feedback animations (embedded)
└── quiz.js          # Main engine handling application state, timer intervals, and quiz data arrays
