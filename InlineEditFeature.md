# AI-Enabled Inline Edit Feature

## Overview

The AI-enabled inline edit feature allows users to make real-time edits to their text with the assistance of AI. This feature is designed to enhance the editing experience by providing intelligent suggestions, grammar corrections, and rephrasing options directly within the editor.

## Implementation Design

### Key Components

1. **Inline Edit Menu**:
   - A floating menu that appears when text is selected.
   - Provides options for AI-powered actions such as grammar correction, rephrasing, and style adjustments.

2. **AI Integration**:
   - Utilizes the Google Gemini API for natural language processing.
   - Sends selected text to the API and retrieves suggestions or corrections.

3. **Editor Integration**:
   - Built on top of the TipTap editor framework.
   - Custom extensions and commands are added to handle AI actions.

4. **User Interaction**:
   - Users can trigger the inline edit menu by selecting text.
   - Keyboard shortcuts are available for quick access to AI features.

### Workflow

1. **Text Selection**:
   - The user selects a portion of text in the editor.

2. **Menu Activation**:
   - The inline edit menu appears near the selected text.
   - Options for AI actions are displayed.

3. **AI Processing**:
   - When an option is selected, the text is sent to the Google Gemini API.
   - The API processes the text and returns the result.

4. **Text Update**:
   - The editor updates the selected text with the AI-generated suggestion.

### Custom Commands

- **Grammar Correction**:
  - Command: `editor.commands.correctGrammar()`
  - Description: Sends the selected text to the API for grammar correction.

- **Rephrasing**:
  - Command: `editor.commands.rephraseText()`
  - Description: Rephrases the selected text for clarity or conciseness.

- **Style Adjustment**:
  - Command: `editor.commands.adjustStyle()`
  - Description: Adjusts the tone or style of the selected text.

### Keyboard Shortcuts

| Shortcut         | Action                     |
|------------------|----------------------------|
| `Ctrl + G`       | Grammar Correction        |
| `Ctrl + R`       | Rephrase Text             |
| `Ctrl + S`       | Style Adjustment          |

## Benefits

- **Efficiency**: Enables quick edits without leaving the editor.
- **Accuracy**: Improves text quality with AI-powered suggestions.
- **User-Friendly**: Intuitive interface and seamless integration.

## Future Enhancements

- Add support for multilingual text editing.
- Provide more customization options for AI actions.
- Enhance the inline menu with additional AI-powered tools.