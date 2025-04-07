# AI Text Editor

AI Text Editor is a modern, feature-rich text editor built with Next.js, TipTap, and TailwindCSS. It leverages AI capabilities to enhance the writing experience, offering features like grammar correction, text rephrasing, and more.

## Features

- **Rich Text Editing**: Supports headings, bold, italic, underline, lists, and more.
- **AI-Powered Enhancements**:
  - Grammar and spelling correction.
  - Text rephrasing for clarity, conciseness, or professionalism.
  - Quick AI actions for selected text.
- **Custom Callouts**: Add callouts for information, best practices, warnings, and errors.
- **Keyboard Shortcuts**: Easily access AI features and callouts with shortcuts.
- **Responsive Design**: Optimized for all screen sizes.
- **Customizable Toolbar**: Add images, links, and code blocks.

## Running the Editor with Callout Node

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/ai-text-editor.git
   cd ai-text-editor
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env.local` file in the root directory.
   - Add your Google Gemini API key:
     ```
     NEXT_PUBLIC_GEMINI_API_KEY=your-api-key
     ```

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

6. Use the toolbar or keyboard shortcuts to add callouts and explore the editor's features.

## Callout Component Demonstration

A short video demonstrating the callout component in use, including custom menus and slash commands, can be found [here](https://drive.google.com/file/d/1m4GPlWWgyb4Q7-uyNSOg83DSrFjAlI7n/view?usp=sharing). (Replace `#` with the actual video link.)

## Keyboard Shortcuts for Callouts

| Shortcut         | Action                     |
|------------------|----------------------------|
| `Alt + C`        | Add an Info Callout       |
| `Alt + B`        | Add a Best Practice Callout |
| `Alt + D`        | Add a Warning Callout     |
| `Alt + E`        | Add an Error Callout      |

## Tech Stack

- **Framework**: [Next.js](https://nextjs.org/)
- **Editor**: [TipTap](https://tiptap.dev/)
- **Styling**: [TailwindCSS](https://tailwindcss.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)
- **AI Integration**: Google Gemini API

## Project Structure

```
.
├── src/
│   ├── app/                # Next.js app directory
│   ├── components/         # Reusable components
│   ├── services/           # API integrations
│   └── styles/             # Global styles
├── public/                 # Static assets
├── .env.local              # Environment variables
├── package.json            # Project dependencies and scripts
├── tailwind.config.ts      # TailwindCSS configuration
└── tsconfig.json           # TypeScript configuration
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- [TipTap](https://tiptap.dev/) for the amazing editor framework.
- [TailwindCSS](https://tailwindcss.com/) for the utility-first CSS framework.
- [Google Gemini API](https://cloud.google.com/generative-ai) for AI capabilities.