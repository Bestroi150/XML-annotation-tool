# Text Annotation Tool

## Overview

The Text Annotation Tool is a desktop application built with Tkinter that enables users to annotate text documents with XML tags. It's designed for creating annotated datasets for NLP tasks, named entity recognition (NER), and other text annotation purposes. The tool supports keyboard shortcuts for rapid annotation and provides real-time color-coded visualization of annotated entities.

## Features

- **Keyboard-Based Annotation:** Quickly annotate text using customizable keyboard shortcuts (a-z, A-Z)
- **XML Tag Support:** Annotate entities with XML-style tags (e.g., `<tag>text</tag>`)
- **Event ID Tracking:** Assign and track event IDs for each annotation
- **Real-Time Visualization:** Color-coded display of annotated entities for easy review
- **Undo Support:** Use Ctrl+Z to undo recent changes
- **File Support:** Open and edit .txt, .ann, and .docx files
- **Export Formats:** Export annotations in multiple formats:
  - `.ann` files (annotation format)
  - HTML format
  - XML format
  - Sequence format (.txs) for NLP models
- **Configurable Shortcuts:** Remap keyboard shortcuts to different annotation labels via the config file
- **Notes Tab:** Built-in notes feature for documentation
- **Nested Entity Support:** Handle overlapping and nested annotations with visual distinction
- **Cross-Platform:** Works on Windows, macOS, and Linux

## Prerequisites

Before using the Text Annotation Tool, ensure you have:

- Python 3.x
- Tkinter (included with most Python installations)
- Additional Python packages:
  - `ttkthemes`
  - `TKinterModernThemes`
  - `pywebview`
  - `aspose-words`
  - `numpy`

## Installation

1. Clone or download this repository to your local machine
2. Navigate to the project directory
3. Install required dependencies:
   ```bash
   pip install ttkthemes TKinterModernThemes pywebview aspose-words numpy
   ```
## Usage

### Starting the Application

```bash
python app.py
```

The tool will open in fullscreen mode with a text editor and annotation controls.

### Basic Annotation Workflow

1. **Open a File:** Use File Operations → Open to load a text file
2. **Select Text:** Highlight the text you want to annotate
3. **Apply Tag:** Press a keyboard shortcut (a-z) to tag the selected text
4. **Assign Event ID:** Enter an event ID number to categorize the annotation
5. **Save:** Right-click or use File Operations → Export to save your work

### Keyboard Shortcuts

- **a-z keys:** Apply configured annotation tags to selected text
- **0-9 keys:** Enter event IDs for annotations
- **Ctrl+Z:** Undo the last action
- **F11:** Toggle fullscreen mode
- **Esc:** Exit fullscreen mode
- **q:** Remove entity label (untag selected text)

### File Operations Menu

- **Open:** Load a text, annotation, or Word document
- **Remap:** Customize keyboard shortcut mappings
- **Export File:** Save annotations as .ann file
- **Export File as HTML:** Convert annotated text to HTML
- **Export File as XML:** Convert annotated text to XML
- **Quit:** Exit the application

### Functions Menu

- **Open notes tab:** Access the notes feature
- **Open Google search:** Launch a web search window
- **Show Keybindings:** Display available keyboard shortcuts
- **Close Keybindings:** Hide the keybindings display

## Configuration

The tool stores keyboard shortcut mappings in a `config` file. Use the **Remap** function to customize which keys map to which annotation labels.

## Output Formats

- **.ann files:** Plain text with XML-style annotations
- **HTML:** Annotated text rendered in HTML with color-coded entities
- **XML:** Properly formatted XML output
- **.txs files:** BIO/BMES-tagged format for machine learning models

## License

This tool is open-source software released under the MIT License.

## Contact

For questions or assistance, please refer to the LICENSE file or contact the project maintainers.
