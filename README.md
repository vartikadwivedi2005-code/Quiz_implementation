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

---

## 🎨 UI/UX Design & Theme

The interface is crafted with a high emphasis on a clean, modern, and modern digital aesthetic:
* **Color Palette:** Features an angled vibrant backdrop (`linear-gradient(135deg, #f1c4ef 0%, #2a5298 100%)`) paired with a crisp, floating white container to prioritize readability and user focus.
* **Micro-interactions:** Interactive elements utilize fluid properties (`transition: all 0.3s; transform: translateX(5px);`) to shift subtly on hover, providing instant tactile feedback to user movements.
* **State-Driven Styling:** The UI dynamically injects contextual utility classes (`.correct`, `.wrong`, `.hide`) via JavaScript to transition states smoothly without requiring a single page reload.

---

## 📈 Key Technical Implementation Details

* **Anti-Cheat State Guardrail:** The application implements an `answered` boolean flag. Once an option is clicked, this flag instantly flips to `true` and disables all option buttons, preventing a user from multi-clicking or changing their answer after seeing the result.
* **Memory Leak Prevention:** To prevent intervals from stacking up in the browser's background when a user clicks through questions rapidly, the countdown logic ensures that `clearInterval(timerInterval)` is strictly invoked before a new timer instance spin up or when an option is selected.
* **Dynamic DOM Reconstruction:** Instead of hardcoding HTML containers for every possible option, the application leverages native `document.createElement('button')` inside a `forEach` loop. This keeps the initial index file lightweight and allows the application to seamlessly scale to questions with any number of multiple-choice variants.

---

## 🗺️ Roadmap & Future Enhancements

Here are some features planned for future iterations of this application:
- [ ] **Category Selection:** Allow users to choose quiz topics (e.g., HTML, CSS, JavaScript, or General Knowledge) before starting.
- [ ] **Persistent High Scores:** Integrate HTML5 `localStorage` to keep track of a user's personal best scores across sessions.
- [ ] **Dark Mode Toggle:** Implement a CSS variable-driven dark theme switcher for comfortable night-time playing.
- [ ] **Progress Bar:** Replace the text-based question counter with a smooth, animated visual progress bar.

---

## 📸 Screenshots / Preview

```html
<p align="center">
  <img src="C:\Users\Acer\OneDrive\Pictures\Screenshots\Screenshot 2026-05-21 134151.png" alt="Quiz App Screen Preview" width="500">
</p>" alt="Quiz App Screen Preview" width="500">

