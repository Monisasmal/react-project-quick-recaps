# React Increment & Decrement App 🔢

A simple React application that demonstrates **increment and decrement functionality** using **three different React Hooks**:
- `useState`
- `useEffect`
- `useReducer`

This project is built to clearly explain **how different hooks manage state and logic** in React.

---

## ✨ Features

- ➕ Increment counter value
- ➖ Decrement counter value
- ⛔ **Prevents decrement below zero**
- 🔁 **Reset button to reset counter value**
- 🔄 Three separate implementations:
  - useState
  - useEffect
  - useReducer
- ⚛️ Real-time UI updates
- 🎯 Beginner & interview friendly

---

## 📦 Hooks Explanation (Interview Focus)

### 🔹 1. Counter using useState
- Manages counter value using local state
- Direct increment, decrement, and reset logic
- Prevents value from going below zero

**Best for:**  
Simple and independent state management

---

### 🔹 2. Counter using useEffect
- Uses `useState` to store counter value
- Uses `useEffect` to react to value changes
- Example side effects:
  - Console logging
  - Updating document title

**Best for:**  
Handling side effects when state changes

---
