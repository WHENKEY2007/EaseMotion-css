# Fix: Dynamic Reduced Motion Listener

Resolves a limitation in `reveal.js` where the scroll reveal script does not respond if the user's `prefers-reduced-motion` preference changes dynamically during a page session.

## What does this do?
- **Live Query Listeners:** Adds a change event listener to the media query result, instantly revealing hidden content components if the motion setting is toggled on.