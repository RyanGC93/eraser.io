

# Erasor Clone

A modern clone of [eraser.io](https://eraser.io) built with a powerful stack of modern web technologies. This project leverages Next.js, React, Editor.js, Excalidraw, Tailwind CSS, and more to deliver an interactive, rich editing experience with drawing, authentication, and collaborative features.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Development](#development)
- [Production](#production)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Rich Text Editing:** Built with [Editor.js](https://editorjs.io) and extensions (header, list, checklist, paragraph, and warning) to provide a block-based editing experience.
- **Interactive Drawing:** Integrated with [Excalidraw](https://github.com/excalidraw/excalidraw) for creating sketches and diagrams.
- **Authentication:** Uses [Kinde Auth for Next.js](https://github.com/kinde-oss/kinde-auth-nextjs) to handle secure user authentication.
- **UI Components:** Utilizes [Radix UI](https://www.radix-ui.com) primitives for dialogs, dropdown menus, popovers, and more to build an accessible interface.
- **Styling & Animations:** Styled with [Tailwind CSS](https://tailwindcss.com) and extended with [tailwindcss-animate](https://github.com/wobsoriano/tailwindcss-animate) for smooth UI animations.
- **Theming:** Implements [next-themes](https://github.com/pacocoursey/next-themes) for dark/light mode support.
- **Backend & Data:** Integrated with [Convex](https://docs.convex.dev) for backend operations and data management.
- **Icons & Utilities:** Uses [lucide-react](https://github.com/lucide-icons/lucide) for iconography, along with utility libraries like `clsx` and `tailwind-merge` for clean class management.

## Tech Stack

- **Framework:** [Next.js 14.1.0](https://nextjs.org)
- **Language:** [TypeScript](https://www.typescriptlang.org)
- **UI Library:** React 18
- **Styling:** Tailwind CSS
- **Rich Editor:** Editor.js and associated plugins
- **Drawing:** Excalidraw
- **Authentication:** Kinde Auth for Next.js
- **UI Components:** Radix UI (Dialog, Dropdown Menu, Popover, Separator, Slot)
- **Animations:** tailwindcss-animate
- **Backend:** Convex
- **Utilities:** clsx, class-variance-authority, tailwind-merge, moment, sonner

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/erasor_clone.git
   cd erasor_clone
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

   or if you prefer using Yarn:

   ```bash
   yarn install
   ```

3. **Configure Environment Variables:**

   Create a `.env.local` file at the root of your project and add any necessary environment variables (e.g., authentication keys, Convex configuration, etc.). Check the project documentation or your provider's docs for details.

   ```env
   NEXT_PUBLIC_API_URL=your_api_url
   KIND_AUTH_CLIENT_ID=your_client_id
   KIND_AUTH_CLIENT_SECRET=your_client_secret
   # Add other required variables...
   ```

## Development

To start the development server, run:

```bash
npm run dev
```

This command starts Next.js in development mode, enabling hot reloading and detailed error reporting. Open [http://localhost:3000](http://localhost:3000) to view the application in your browser.

## Production

### Build

To create an optimized production build:

```bash
npm run build
```

### Start

After building, you can start the production server with:

```bash
npm run start
```

> **Note:** Ensure that all environment variables are correctly configured for the production environment.

## Project Structure

A typical project structure might look like this:

```
erasor_clone/
├── components/         # Reusable UI components (e.g., Editor, Excalidraw canvas, dialogs)
├── pages/              # Next.js pages and API routes
├── public/             # Static assets (images, fonts, etc.)
├── styles/             # Global and component-specific styles (Tailwind CSS configuration)
├── utils/              # Utility functions and helpers
├── .env.local          # Environment configuration file (not committed)
├── package.json        # Project manifest and scripts
└── README.md           # This file
```

Customize this structure as your project evolves.

## Contributing

Contributions are welcome! If you have suggestions, bug fixes, or improvements:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Commit your changes.
4. Open a pull request with a detailed description of your changes.

Please ensure your code follows the project's coding guidelines and include tests where applicable.

## License

This project is licensed under the [MIT License](LICENSE).

