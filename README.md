# A Harbour and xHarbour Powerful Intellisense **Alpha**

**Harbour-Intellisense** provides powerful language support for Harbour, including syntax analysis, scope detection, intelligent code completion, and more. This extension is tailored for developers working with Harbour and xHarbour codebases, enhancing productivity with in-depth insights into your project structure.

**Please note**: This extension is in **Alpha** and still under active development. It has some limitations, which currently works only for functions and procedures, all the features have a disable config if you want to use a finished version from other extension.

---

## Features

- Harbour language support for `.prg`, `.ch` files.

- **Scope Detection**:  
  Dynamically parses your Harbour code to generate a recursive scope tree, including support for nested functions, variables, and parameters.  
  (Currently working on classes, methods, and codeblocks scope detection.)

- **Hover Support**:  
  Displays tooltips with scope and type information for identifiers under the cursor.  
  (Working to add more information)  
  ![Demo hover](./images/gifs/hover.gif)

- **Auto-Completion**:  
  Suggests relevant completions based on the current scope and context.  
  (Needs an improvment in the filtering to match with the vscode filtering)  
  ![Demo auto-completion](./images/gifs/auto-complete.gif)

- **Go-to Definition**:  
  Quickly navigate to the definition of a variable, function, or other identifiers.  
  (Not working for classes and methods)  
  ![Demo go-to](./images/gifs/go-to.gif)

- **Diagnostics**:  
  You can configure the language diagnostics using the harbour or xHarbour compiler, see this section for more
  ![Demo diagnostics](./images/gifs/diagnostics.gif)

- **Signature Help**:  
  Shows function, procedures... parameters and details when typing or hovering over function calls.  
  (Working on DocBlock to show params and function documentation)  
  ![Demo signature-helper](./images/gifs/signature-help.gif)

- **Harbour Snippets**:  
  Some snippets for most of the Harbour and xHarbour reserved words, structures and functions with some documentation scanned from the original doc.  
  (In the future i will implement the doc in the hover provider to)  
  ![Demo snippets](./images/gifs/snippet.gif)

- **Formatter**:  
  Some formating patterns for the harbour files  
  (Needs more effort to complete but create a basic pattern in your code, disable the config if you does`t like)  
  ![Demo formatter](./images/gifs/formatter.gif)

- **Document Symbol**:  
  A initial implementation for the document symbol provider, working to improve it.
  
---

## Requirements

- Visual Studio Code 1.70.0 or higher.
- No additional dependencies.

---

## Known Issues

- **Suport For Classes and Methods**:  
  Currently, scope analysis needs an implementation for classes and methods (this will work for all the other features to).

- **References Provider Don`t Work**:  
  I need to develop this feature ;-;.

---

## Why Lowercase for Reserved Words?

I`ve chosen to use a lowercase pattern for reserved words in Harbour to align with common conventions in modern programming languages. This approach aims to improve code readability, especially for new developers coming from other languages. While Harbour itself is case-insensitive, establishing a consistent pattern can greatly enhance the clarity of code and make it easier to follow. I believe this small adjustment will help maintain a clean and understandable codebase for both new and experienced developers alike.

---

## Contact

If you find any bugs or have suggestions, feel free to reach out to me at:

**Email**: [luan.nc@hotmail.com](mailto:luan.nc@hotmail.com)

---

**Enjoy coding with Harbour Intellisense!**
