# SDOG Syntax Highlighting for VS Code

This extension provides syntax highlighting and custom file icons for SDOG (Sea Dog Overseeing Guide) and SDOGX files in Visual Studio Code.

## Features

- **Syntax Highlighting**: Highlighting for SDOG-specific tags and comments.
- **Custom File Icons**: Unique icons for `.sdog` and `.sdogx` files.

## Installation

To install the SDOG Syntax Highlighting extension, follow these steps:

1. Clone the repository or download the source code.
2. Open the folder in Visual Studio Code.
3. Run `npm install` to install dependencies.
4. Press `F5` to open a new VS Code window with the extension loaded.

## Usage

Once installed, any file with the `.sdog` or `.sdogx` extension will be highlighted according to SDOG syntax rules.

### Supported Tags

The extension supports the following SDOG tags:

- `<boat>`
- `<crowsnest>`
- `<deck>`
- `<parley>`
- `<cap>`
- `<mate>`
- `<crew>`
- `<cm>` (Ordered list item)
- `<cl>` (Unordered list item)
- `<painting>`
- `<foot>`
- `<shiplog>`

### Comments

SDOG uses `//` for line comments.

### Sample SDOG File

```html
<boat>
  <crowsnest>
    // This is the header
  </crowsnest>
  <deck>
    <parley>
      <cap>Welcome to SDOG!</cap>
      <mate>Let's build a pirate-themed document.</mate>
    </parley>
    <crew>
      <cm>Ordered list item 1</cm>
      <cm>Ordered list item 2</cm>
    </crew>
    <crew>
      <cl>Unordered list item 1</cl>
      <cl>Unordered list item 2</cl>
    </crew>
    <painting src="image.jpg" />
    <foot href="http://example.com">Link</foot>
  </deck>
  <shiplog>
    // Footer content
  </shiplog>
</boat>
