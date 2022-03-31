# AutoX Code Pilot
---
## Requirements

- You are required to have a Codex API key in your possession. 

---
## How-to-use
As given in the requirements we need a Codex API key for this extension to work. If you have it already we are all ready to go.
1. You will be required to enter the API key only when you open a VSCode instance after boot, or after installing the extension.
2. To enter the API key, open Command Palette by `ctrl+shift+p` for windows, Linux and `cmd+shift+p` for mac
3. Try finding the start session command which might look like `Codex: start session` and press `Enter`. You would be asked to enter your API key here, don't worry it is received in hidden star format, so you can just copy and paste it in front of other people.
4. And even if you forget to start a session and went on to the next command, it verifies if you have added a key before generating any code.
5. Now, you want to use this extension to generate some code right, let's do that.
6. As this is an AI it cannot read your mind, write some code before asking it to generate some code, you can write comments, and some code of your own, just to let the AI understand the objective and the programming language.
7. After that go to the command palette, and find something that looks like this `Codex: Generate Code Completion`, and press `Enter`. The extension will run for a while, so hang on. It will check if the key is correct, it will request the codex API to generate the code that you want, and write it in the currently opened document.

---
## Features

- This is just an abstraction of the underlying Codex API that was implemented by openAI
- [openai-codex](https://openai.com/blog/openai-codex/) <- Check the following link to understand the specification.
---

## Known Issues

- Cannot generate multiple completion for the same piece of code
- The Generated code, is limited by the efficiency of AI
---
## Possible issues
- Even though you have an API Key the extension might reject it
    ```
    // Key not verified error message might be displayed
    Check:
    - If you have access to davinci-codex through the playground
    Fix:
    - If you don't have access: please apply for codex
    - If you do have the access: A simple fix might be to create a new API key from the API keys settings and use that instead
    ```
