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
  ![hover](https://github.com/user-attachments/assets/b62b033a-a7b9-49b2-95b0-adf60192a740)

- **Auto-Completion**:  
  Suggests relevant completions based on the current scope and context.  
  (Needs an improvment in the filtering to match with the vscode filtering)  
  ![auto-complete](https://github.com/user-attachments/assets/782db172-c917-4fcf-bb27-1b06492ba7c8)

- **Go-to Definition**:  
  Quickly navigate to the definition of a variable, function, or other identifiers.  
  (Not working for classes and methods)  
  ![go-to](https://github.com/user-attachments/assets/d782fa57-e927-4bbb-83a9-1a5b0b39a60a)

- **Diagnostics**:  
  You can configure the language diagnostics using the harbour or xHarbour compiler, see this section for more
  ![diagnostics](https://github.com/user-attachments/assets/4acda9d2-78c2-4c4f-a2d7-7f88ce07b4cf)

- **Signature Help**:  
  Shows function, procedures... parameters and details when typing or hovering over function calls.  
  (Working on DocBlock to show params and function documentation)  
  ![signature-help](https://github.com/user-attachments/assets/9bfb22c9-7ab0-41d0-9377-fbfc86172609)

- **Harbour Snippets**:  
  Some snippets for most of the Harbour and xHarbour reserved words, structures and functions with some documentation scanned from the original doc.  
  (In the future i will implement the doc in the hover provider to)  
  ![snippet](https://github.com/user-attachments/assets/bd32522e-f3da-4e97-89db-8d39ab841e89)

- **Formatter**:  
  Some formating patterns for the harbour files  
  (Needs more effort to complete but create a basic pattern in your code, disable the config if you does`t like)  
  ![formatter](https://github.com/user-attachments/assets/fe6bc8ff-c2b6-486b-b16b-7832d4bda833)

- **Document Symbol**:  
  A initial implementation for the document symbol provider, working to improve it.
  ![document-symbol](https://github.com/user-attachments/assets/5fef1c2e-8f1e-4a9e-b87b-fcadf84e7525)

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

If you find any bugs or have suggestions, feel free to open a issue on the public repository:
https://github.com/luan098/harbour-intellisense-public

---

**Enjoy coding with Harbour Intellisense!**
