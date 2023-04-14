# Set Up

The tooling I use on my day-to-day.

## Operating System

<img src="images/microsoft.svg" width="23px" height="23px" /> Windows 11

_Yes, I use Windows for software development as my primary workstation_ 🙄.

I have been using Windows since XP, and have become very comfortable with it. I tried my hand at Ubuntu, Lubuntu, Mint, Raspberry PiOS, and MacOS, but I always come back to Windows as my primary workstation.

## File System

<img src="images/ubuntu.svg" width="18px" height="18px" /> Ubuntu 22.04

> What? I thought you said you use Windows? 🤔

Oh, right 😅. Did I forget to mention... I use WSL 2 on Windows 11 for my day-to-day development.

Windows Subsystem for Linux (WSL) is a compatibility layer for running Linux binary executables (in ELF format) natively on Windows 10 and Windows Server 2019. WSL provides a Linux-compatible kernel interface developed by Microsoft, which can then run Linux distributions in user mode on Windows [^1].

## Terminal

<img src="images/windows-terminal.png" width="18px" /> Windows Terminal [^2]

Powershell is useful and all, but it is difficult to use most developer tools with it; the software world has just leant towards using UNIX-like shells. I have found connecting to WSL though Windows Terminal to be convinient, as Windows Terminal allows mulitple terminal sessions in tabs.

![split terminals](images/split-terminals.png)

<img src="images/ohmybash.png" alt="Oh My Bash" width="23px" /> Oh-My-Bash [^3]

I use Oh-My-Bash, which is a bash shell with a bunch of useful plugins and themes. Here is my current config: <https://gist.github.com/ShaunSHamilton/afe0f6c79fa10fcb5ea83436f98fa5b0>

The only custom bits are:

- The timestamp shown in the prompt
- The terminal tab title is set based on the directory I am in
- The prompt includes my silly emojis letting me know what kind of project I am working on

![my terminal](images/terminal-1.png)

## Tools

### Node.js

Fortunately/Unfortunately, I have the luxury of being able to use Node.js for a lot of my work.

I install Node.js using Node Version Manager (nvm) [^4]:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

Once installed, I can install any versions of Node.js I want (except for `v999`):

```bash
nvm install 1
nvm use 1
```

> [!NOTE]
> Do not actually install Node.js version `1`. It is just an example.

### Rust

#### `rustup`

#### `cargo`

#### `rustc`

### Docker Desktop

### MongoDB

[^1]: [WSL Documentation](https://learn.microsoft.com/en-us/windows/wsl/)

\

[^2]: [Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701)

\

[^3]: [Oh My Bash](https://ohmybash.nntoan.com/)

\

[^4]: [Node Version Manager](https://github.com/nvm-sh/nvm)
