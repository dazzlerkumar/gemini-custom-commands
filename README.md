# Gemini Custom Commands

This repository contains a collection of custom slash commands for the Gemini CLI, designed to streamline your development workflow.

## Features

- **Git Commit Message Generation**: The `/commit` command generates a Git commit message based on your staged changes, following conventional commit standards.
- **TypeScript Type Generation**: The `/types` command generates and adds TypeScript types to your files with intelligent placement and deduplication.

## Installation

To use these custom commands, you need to add them to your Gemini CLI configuration.

1.  Clone this repository:
    ```bash
    git clone https://github.com/your-username/gemini-custom-commands.git
    ```
2.  Follow the Gemini CLI documentation to add the commands from the `commands` directory to your setup.

## Usage

### `/commit`

When you have staged changes in your Git repository, you can use the `/commit` command to generate a commit message.

```
/commit
```

This will generate a commit message based on the output of `git diff --staged`.

### `/types`

To generate and add types to a TypeScript file, use the `/types` command followed by the file path and the type to generate.

```
/types <file-path> <type-to-generate>
```

For example:

```
/types src/components/Button.tsx ButtonProps
```

This will analyze `src/components/Button.tsx`, generate a `ButtonProps` type, and add it to the file.

## Contributing

Contributions are welcome! If you have a custom command you'd like to add, please open a pull request.