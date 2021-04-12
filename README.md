# SvelteKit Tailwind Adder Keyframe Bug 🦠

1. Once you've cloned the project and installed dependencies with `npm install`, start a development server with `npm run dev`. Take note of the animated marquee of lorem ipsum, translating to the left by way of an `@keyframes` rule. That rule shows up in the page source.

2. Now run the build process with `npm run build`. Follow up with `npm start` to see the output build in the browser. You should notice that the marquee animation does not occur and the `@keyframes` rule does not appear in the page source, indicating that it has incorrectly been purged from the production output.
