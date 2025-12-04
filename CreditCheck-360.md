# ✅ CreditCheck-360 — Project Summary

🌐 **Live Demo:**  👉 [View App](https://credit-check-360-manaswini-sasmals-projects.vercel.app/) 

## Tech Stack Used:
React + Vite, JavaScript, CSS, plus the npm package validator

## Summary:
CreditCheck-360 is a React + Vite based credit-card validator tool: the user enters card details and gets instant validation, card-brand detection, and a live card preview with CVV flip animation. I used the validator npm library for reliable validation logic, React for UI & state handling, and custom CSS for styling. Everything runs client-side — no backend — and provides a smooth, responsive, accessible user experience.

## Key Features:
- Credit-card number validation (via validator library)
- Card brand detection (Visa, MasterCard, Amex, Discover etc.)
- Live preview / UI representation of card number, expiry, CVV, and cardholder name
- Animated card-flip effect when focusing on CVV field
- CVV length check (3 or 4 digits depending on card type)
- Accessible markup (using aria labels and htmlFor) for better UX / accessibility
- Responsive layout — works across screen sizes / device types.
- Instant feedback for valid / invalid card data — no page reload needed.

## Why These Technologies / Approach:
- React + Vite → for lightweight, fast development and modern JS tooling.
- validator library — to leverage existing, tested validation logic instead of writing from scratch.
- Custom CSS + manual UI → gives full styling control, lightweight design, and avoids overhead of big UI libraries.
- Client-side validation & preview → instant feedback and UI responsiveness without backend dependencies.

## Challenges & Solutions:

- **Challenge**: Validating various card formats (different brands, CVV length, expiry, user mistakes)

  **Solution**: Used validator package + custom logic + real-time feedback to ensure correctness.
  
- **Challenge**: Building card preview & animated flip with correct UI and responsiveness

  **Solution**: Custom React components + CSS + state handling + careful UI layout.
  
- **Challenge** : Keeping UI light and dependency-free while maintaining good UX

  **Solution**: Manual CSS styling + minimal dependencies (only validator + React + Vite).
  
