# Fix: Stacked Modal Focus Restoration

Resolves a focus tracking regression in `modal.js` when opening a second modal from inside an active modal.

## What does this do?
- **Focus Stack:** Replaces the single global `previousFocusedElement` variable with a LIFO focus stack array, guaranteeing focus returns to the correct initiator element when modals are dismissed in reverse order.