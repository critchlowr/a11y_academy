# a11y_academy

An interactive learning platform for teaching web developers how to build accessible web technologies, organized around the WCAG 2.xx (3.0 comes out soon?) principles: Perceivable, Operable, Understandable, and Robust. 

This is the general idea: give people a lesson, a live code editor, and a way to actually interact with the webpage content with an open source screen reader. The aim is to illuminate the online experience that people with screen readers experience and also to teach real skills to incorporate into your own projects.

It's part learning tool for developers, part disability simulator.

## What it does

- **Lessons** — structured around WCAG's four principles, covering things like alt text, color contrast, focus order, keyboard navigation, semantic HTML, and correct ARIA usage
- **Live code editor** — write HTML/ARIA markup and see it rendered in real time
- **Accessibility feedback** — automated linting flags issues as you type
- **Screen reader simulation** — hear how assistive tech interprets your markup, so bad code has an immediate, tangible consequence instead of a silent one

## Roadmap

Nothing built yet — this is the current plan.

- [ ] Live editor + render pane
- [ ] Accessibility linting (axe-core) -- I actually don't know if I will use this or not, like this specific tool
- [ ] Color contrast checker (Perceivable)
- [ ] Screen reader simulation (Web Speech API)
- [ ] Lesson curriculum organized by WCAG principle (starting with Perceivable + Operable)
- [ ] Progress tracking

## Tech Stack

- [Svelte](https://svelte.dev/) + [Vite](https://vitejs.dev/)
- [axe-core](https://github.com/dequelabs/axe-core) for accessibility auditing
- Web Speech API for screen reader simulation

## Design Notes

- Lessons that do not have a code edit part to it will utilize full screen real estate for reading the text and displaying any diagrams or images
- Lessons that do have a code edit part will have a split pane layout
- Lessons that feature a webpage will have the full page in view as a demo and be in a scrollytelling format
- Quizzes will follow the lessons
- Maybe completion will send you a pdf saying your name, completion date, and a fun little image. ;)

## Getting Started

\`\`\`bash
npm install
npm run dev
\`\`\`

## License

MIT
