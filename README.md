# gh-emergency

`gh-emergency` is a GitHub CLI extension that allows you to quickly add, commit, and push changes to a remote repository in case of an emergency. It simplifies the process of creating a new branch, staging all changes, creating a commit with a default or custom message, and pushing the changes to all configured remotes.

## Installation

To install the `gh-emergency` extension, follow these steps:

1. Make sure you have the GitHub CLI (`gh`) installed on your system. If you haven't installed it yet, you can find installation instructions in the [official GitHub CLI documentation](https://cli.github.com/manual/installation).

2. Install the `gh-emergency` extension by running the following command:

   ```shell
   gh extension install MohamedElashri/gh-emergency
   ```

   This command will download and install the extension from the GitHub repository.

3. Verify the installation by running:

   ```shell
   gh emergency --version
   ```

   If the installation was successful, you should see the version number of the `gh-emergency` extension.

## Usage

To use the `gh-emergency` extension, navigate to your Git repository in the terminal and run the following command:

```shell
gh emergency [<message>]
```

- If you run `gh emergency` without providing a message, it will create an emergency commit with a default message that includes the current branch, user email, and timestamp.
- If you want to provide a custom commit message, you can run `gh emergency <message>`, replacing `<message>` with your desired message.

The extension will perform the following actions:

1. Create a new branch with a name in the format `emergency-<timestamp>-<branch-name>`.
2. Stage all changes in the repository.
3. Create a commit with the default or custom message.
4. Push the changes to all configured remotes.

If any errors occur during the process, they will be logged in the `emergency.log` file in the repository's root directory.

## Contributing

If you have any suggestions, bug reports, or feature requests, please open an issue on the [GitHub repository](https://github.com/MohamedElashri/gh-emergency). Contributions are welcome!

## License

This extension is released under the [MIT License](https://opensource.org/licenses/MIT).

