# Oh-My-Bash Plugins: Enhancing Your Development Experience

"Oh My Bash won't make you a tenfold developer... but it might make you feel like one."

_Embracing a suite of plugins can significantly boost your coding efficiency by automating repetitive tasks, thereby making them less monotonous and easier to execute._

**What is a Plugin?**
A plugin is a type of software that augments the functionality of an existing program or system. These additions can range from simple to complex features and are intended to extend or customize the core functionality without modifying the codebase.

**Plugin Enablement:**
Once you identify the plugins you wish to utilize with Oh My Bash, you'll need to enable them in the `.bashrc` file located in your `$HOME` directory. Open this file with your preferred text editor and specify the plugins you want to load. For instance:

```bash
plugins=(git bundler osx rake ruby)
```

**Conditional Enablement:**
You may wish to control when or how plugins are activated. For instance, to ensure the `tmux-autoattach` plugin runs only in SSH sessions, you can employ a conditional statement checking for the `$SSH_TTY` variable. Make sure to remove the plugin from the main plugin list and use a conditional like this:

```bash
[[ $SSH_TTY ]] && plugins+=(tmux-autoattach)
```

By leveraging these plugins, you can streamline your workflow and tackle coding challenges with greater efficiency.

| Plugin            | Description                                                                                                                 |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------|
| ansible           | Configuration management tool used to automate the provisioning, configuration, and management of computer systems.         |
| [asdf](asdf)      | [asdf](https://asdf-vm.com) is a tool version manager to allow installing different versions of Node.js, Ruby, Golang, etc. |
| aws               | Tools for interacting with Amazon Web Services (AWS)                                                                        |
| bash-preexec      | Tool allowing execution of commands before they are executed in Bash.                                                       |
| bashmarks         | Utility facilitating directory navigation via bookmarks in Bash.                                                            |
| battery           | Plugin related to monitoring and managing battery on computer systems.                                                      |
| brew              | Package manager for macOS and Linux facilitating software installation and management.                                      |
| bu                | Insufficient information provided to give a precise description.                                                            |
| cargo             | Plugin to initialize CARGO_HOME and PATH for cargo                                                                          |
| colored-man-pages | Adds a few colors to `man` pages.                                                                                           |
| chezmoi           | Dotfile management tool enabling management of user environment configuration.                                              |
| dotnet            | This plugin provides completion and useful aliases for .NET Core CLI.                                                       |
| fasd              | Utility easing filesystem navigation through shortcuts and abbreviated commands.                                            |
| fzf               | A command-line fuzzy finder.                                                                                                |
| gcloud            | Command-line tools for interacting with Google Cloud Platform (GCP).                                                        |
| git               | Distributed version control system for managing the history of changes in software projects.                                |
| goenv             | Tool for managing Go versions within a development environment.                                                             |
| golang            | The Go programming language, along with its tools and standard libraries.                                                   |
| jump              | Jump helps you navigate faster by learning your habits.                                                                     |
| kubectl           | Command-line tool for interacting with Kubernetes clusters.                                                                 |
| npm               | Package manager for Node.js facilitating installation and management of project dependencies.                               |
| nvm               | Node.js version manager allowing easy switching between different Node.js versions.                                         |
| progress          | Insufficient information provided to give a precise description.                                                            |
| pyenv             | Tool for managing multiple Python versions within a system.                                                                 |
| rbenv             | Tool for managing your app's Ruby environment.                                                                              |
| sdkman            | Version and package manager for development tools such as Java, Kotlin, and Gradle.                                         |
| sudo              | Utility for executing commands with superuser privileges on Unix and Unix-like systems.                                     |
| tmux-autoattach   | Plugin related to session management in the tmux terminal multiplexer.                                                      |
| vagrant           | Tool for creating and managing virtual development environments.                                                            |
| virtualenvwrapper | A set of extensions to the virtualenv tool.                                                                                 |
| xterm             | Terminal emulator for X Window systems providing a graphical user interface for accessing the command line.                 |
| zellij-autoattach | Plugin related to session management in the zellij terminal multiplexer.                                                      |
| zoxide            | Utility for quickly navigating the filesystem based on visited directory history.                                           |
