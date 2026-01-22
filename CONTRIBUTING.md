# Contributing to Calliope IDE

First off, thanks for taking the time to contribute! ❤️

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. It will make it a lot easier for us maintainers and smooth out the experience for all involved. The community looks forward to your contributions.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [I Want To Contribute](#i-want-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
  - [Improving The Documentation](#improving-the-documentation)
- [Styleguides](#styleguides)
  - [Commit Messages](#commit-messages)

## Code of Conduct

This project and everyone participating in it is governed by the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).
By participating, you are expected to uphold this code. Please report unacceptable behavior to [insert-email@example.com](mailto:insert-email@example.com).

## I Have a Question

If you want to ask a question, we assume that you have read the available [Documentation](README.md).

Before you ask a question, it is best to search for existing [Issues](https://github.com/aludyalu/chatterji/issues) that might help you. In case you have found a suitable issue and still need clarification, you can write your question in this issue. It is also advisable to search the internet for answers first.

If you then still feel the need to ask a question and need clarification, we recommend the following:

- Open an [Issue](https://github.com/aludyalu/chatterji/issues/new).
- Provide as much context as you can about what you're running into.
- Provide project and platform versions (nodejs, npm, etc), depending on what seems relevant.

We will then take care of the issue as soon as possible.

## I Want To Contribute

### Reporting Bugs

- **Use a clear and descriptive title** for the issue to identify the problem.
- **Describe the steps to reproduce the exact steps which reproduce the issue** in as many details as possible.
- **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples. If you're providing snippets in the issue, use [Markdown code blocks](https://help.github.com/articles/markdown-basics/#code-formatting).
- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
- **Explain which behavior you expected to see instead and why.**
- **Include screenshots and animated GIFs** which show you following the described steps and demonstrate the problem. 

### Suggesting Enhancements

- **Use a clear and descriptive title** for the issue to identify the suggestion.
- **Provide a step-by-step description of the suggested enhancement** in as many details as possible.
- **Provide specific examples to demonstrate the steps**.
- **Describe the current behavior** and **explain which behavior you expected to see instead** and why.

### Your First Code Contribution

Unsure where to begin contributing? You can start by looking through these `good-first-issue` and `help-wanted` issues:

- [Good First Issues](https://github.com/aludyalu/chatterji/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22)
- [Help Wanted](https://github.com/aludyalu/chatterji/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22)

#### Local Development Setup

Calliope IDE consists of a Next.js frontend and a Python Flask backend.

1.  **Clone the repository**
    ```bash
    git clone https://github.com/aludyalu/chatterji.git
    cd chatterji
    ```

2.  **Frontend Setup**
    Ensure you have Node.js (v18+) installed.
    ```bash
    npm install
    npm run dev
    ```
    The frontend will start at `http://localhost:3000`.

3.  **Backend Setup**
    Ensure you have Python 3.8+ installed.
    ```bash
    # Create a virtual environment (recommended)
    python3 -m venv venv
    source venv/bin/activate

    # Install dependencies (assuming requirements.txt exists, otherwise install flask google-generativeai)
    pip install flask google-generativeai

    # Set your Gemini API Key
    export GEMINI_API_KEY="your_api_key_here"

    # Start the server
    python3 server/start.py
    ```
    The backend usually starts on a random port or as configured in the scripts.

### Improving The Documentation

Documentation improvements are always welcome! You can find the documentation in the `README.md` file and standard markdown files throughout the repository.

## Styleguides

### Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters or less
- Reference issues and pull requests liberally after the first line
