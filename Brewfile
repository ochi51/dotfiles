# Brewfile 2022/02/01
cask_args appdir: '/Applications'

# Alternate versions of Casks
tap 'homebrew/cask-versions'
# Integrates Homebrew formulae with macOS' `launchctl` manager
tap 'homebrew/services'
# A CLI tool upgrading every outdated app installed by Homebrew Cask
# INFO: brew cu
tap 'buo/cask-upgrade'
# Fonts
tap 'homebrew/cask-fonts'
# AWS
tap 'aws/tap'

### System {{{
  # Core application library for C
  brew 'glib'
  # Image manipulation library
  brew 'jpeg'
  # Library for manipulating PNG images
  brew 'libpng'
  # TIFF library and utilities
  brew 'libtiff'
  # Software library to render fonts
  brew 'freetype'
  # Generic library support script
  # INFO: In order to prevent conflicts with Apple's own libtool we have prepended a "g"
  brew 'libtool'
  # SSL/TLS cryptography library
  brew 'openssl'
  # Simple tool for making locally-trusted development certificates.
  brew 'mkcert'

  ## Monitoring
  # macOS system monitor in your menu bar
  cask 'stats'

  ## Mac OS X
  # Mac App Store command line interface
  brew 'mas'

### Terminal {{{
  ## Terminal Emulator
  # Terminal Emulator for macOS
  cask 'iterm2'
  # A terminal multiplexer, allowing to access multiple separate terminal sessions
  brew 'tmux'
  # Reattach process (e.g., tmux) to background
  brew 'reattach-to-user-namespace'

  ## Shell: Bash
  # Bourne-Again SHell, a UNIX command interpreter
  brew 'bash'
  # Programmable completion for Bash 4.1+
  brew 'bash-completion@2'

  ## Shell: Zsh
  # UNIX shell (command interpreter)
  # INFO: Need to add `/usr/local/bin/zsh` to `/etc/shells`
  brew 'zsh'
  # Tips, tricks, and examples for zsh
  brew 'zsh-lovers'
  # Completion for zsh
  brew 'zsh-completions'
  # Fish-like autosuggestions for zsh
  brew 'zsh-autosuggestions'
  # Fish shell like syntax highlighting for Zsh.
  brew 'zsh-syntax-highlighting'
  # Zsh theme
  # brew 'romkatv/powerlevel10k/powerlevel10k'
  # Flexible and fast Zsh plugin manager
  # brew 'zinit' # sh -c "$(curl -fsSL https://git.io/zinit-install)"
#}}}


### Utility {{{
  # Internet file retriever
  brew 'wget'

  ## Compress/Uncompress
  # 7-Zip (high compression file archiver) implementation
  brew 'p7zip'
  # General-purpose data compression with high compression ratio
  brew 'xz'
  # The Unarchiver is a small and easy to use program that can unarchive many different kinds of archive files.
  cask 'the-unarchiver'

  # Display directories as trees
  brew 'tree'
  # Executes a program periodically, showing output fullscreen
  brew 'watch'
  # Simplified and community-driven man pages
  brew 'tldr'
  # Clone of cat with syntax highlighting and Git integration  brew 'bat'
  # Simple, fast and user-friendly alternative to find
  brew 'fd'
### }}}

### Image {{{
  ## Utility
  # Perl lib for reading and writing EXIF metadata
  brew 'exiftool'
  # Tools and libraries to manipulate images in many formats
  brew 'imagemagick'
### }}}

### Video {{{
  ## Converter
  # ffmpeg
  brew 'ffmpeg'
### }}}

### Keyboard & Mouse {{{
  # Customize various input devices on your Mac
  cask 'bettertouchtool'
  # Know your short cuts
  cask 'keyclu'
### }}}

### Font {{{
  # XML-based font configuration API for X Windows
  brew 'fontconfig'

  ## Font Family: Icons
  # Most popular icon toolkit
  cask 'homebrew/cask-fonts/font-fontawesome'
  # Font Family: プログラミングフォント 白源 (はくげん／HackGen)
  cask 'font-hackgen'
  cask 'font-hackgen-nerd'
### }}}

### Code Editor & IDE {{{
  ## Editor: Vim
  # Vi 'workalike' with many additional features
  brew 'vim'
  # Ambitious Vim-fork focused on extensibility and agility
  brew 'neovim'

  ## Editor: Microsoft Visual Studio Code
  cask 'visual-studio-code'

  ## Intellij IDE toolbox
  cask 'jetbrains-toolbox'
### }}}

### VCS {{{
  ## Git & GitHub
  # Distributed revision control system
  brew 'git'
  # Git extension for versioning large files
  brew 'git-lfs'
  # Small git utilities
  brew 'git-extras'
  # Extensions to follow Vincent Driessen's branching model
  brew 'git-flow'
  # Prevents you from committing sensitive information to a git repo
  brew 'git-secrets'
  # Remove crazy big files, passwords, credentials and other private data
  brew 'bfg'
  # Text interface for Git repositories
  brew 'tig'
  # A simple terminal UI for git commands
  brew 'lazygit'
  # GitHub command-line tool
  brew 'gh'
  # A framework for managing and maintaining multi-language pre-commit hooks
  brew 'pre-commit'
  # Graphical client for Git version control
  cask 'sourcetree'
  # Run your GitHub Actions locally
  brew 'act'
### }}}

### Programming Language {{{
  # All in one for **env
  brew 'anyenv'

  ## Node.js
  # Platform built on V8 to build network applications
  brew 'node'
  # JavaScript package manager
  brew 'yarn'
  # AST-based pattern checker for JavaScript
  brew 'eslint'
  # Code formatter for JavaScript, CSS, JSON, GraphQL, Markdown, YAML
  brew 'prettier'
  # Standard Tooling for Vue.js Development
  brew 'vue-cli'

  # Local server
  brew 'http-server'
  brew 'nss'

  ## PHP
  brew 'php'
  # Dependency Manager for PHP
  brew 'composer'
  # Symphony CLI
  brew 'symfony-cli/tap/symfony-cli'

  ## Python
  # Python3
  brew 'python'
  # Python dependency management tool
  brew 'pipenv'

  ## Ruby
  # Powerful, clean, object-oriented scripting language
  brew 'ruby'
  # Compile and install Ruby for rbenv
  brew 'ruby-build'

  ## Golang
  # Open source programming language to build simple/reliable/efficient software
  brew 'go'
  # The world’s fastest framework for building websites
  brew 'hugo'

  ## C Family
  # GNU compiler collection
  brew 'gcc'

  ## YAML
  # Linter for YAML files
  brew 'yamllint'
### }}}

### Virtualization {{{
  ## Container
  # Docker
  cask 'docker'
### }}}

### Database {{{
  ## SQL
  # SQLite
  brew 'sqlite'
  # MySQL
  brew 'mysql'
  # PostgreSQL
  brew 'postgresql@16'

  ## Key-Value DB
  # Persistent key-value database, with built-in net interface
  brew 'redis'
### }}}

### DevOps {{{
  ## AWS
  # Universal Command Line Interface for AWS
  brew 'awscli'
  # A vault for securely storing and accessing AWS credentials in development environments
  cask 'aws-vault'
  # AWS SAM CLI is a tool for lcal development and testing of Severless applications
  brew 'aws-sam-cli'
  # AWS DynamoDB Local tool
  cask 'dynamodb-local'

  # Tool to build, change, and version infrastructure
  #brew 'terraform'

  # Enables you to reproduce the CircleCI environment locally
  #brew 'circleci'
### }}}

### Web {{{
  ## Web Browser
  cask 'google-chrome'
  cask 'firefox'
  cask 'microsoft-edge'
### }}}

### Messaging {{{
  mas 'Slack', id: 803453959
### }}}

### Other {{{
  # Google Japanese IME
  cask 'google-japanese-ime'
  # Zoom
  cask 'zoom'
  # Display Menu
  mas 'Display Menu', id: 549083868
### }}}}
