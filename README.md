# LEX
[![build](https://github.com/cmd777/lex/actions/workflows/build_all_os.yml/badge.svg)](https://github.com/cmd777/lex/actions/workflows/build_all_os.yml)

# Table of Contents
**πΊπΈ English**

[**βΉοΈ Information about the project**](#-information-about-the-project)
- [What is Lex?](#what-is-lex)
  - [Why create Lex?](#why-create-lex)
- [How do I use Lex?](#how-do-i-use-lex)
  
[**βοΈ Installation Instructions**](#-installation-instructions)
- [Building Instructions](#building-instructions)
- [Downloading Binaries](#downloading-binaries)

[**π¬ Compatibility**](#-compatibility)

[**π© Bugs, Issues, and other Important Information**](#-bugs-issues-and-other-important-information)

[**π Legal Disclaimer**](#-legal-disclaimer)

[**π§° Technologies that were used to create Lex**](#-technologies-that-were-used-to-create-lex)

[**π Other Information**](#-other-information)
- [Do I need a reddit account to use Lex?](#do-i-need-a-reddit-account-to-use-lex)
- [Can I upvote / comment on posts?](#can-i-upvote--comment-on-posts)

---

**[π­πΊ Magyar README](https://github.com/cmd777/lex/blob/main/README_hu.md)**

---

# βΉοΈ Information about the project

## What is Lex?
LEX (LazerEX) is a lightweight, open source frontend for reddit written in Go.

## Why create Lex?

Reddit can be very slow, and is very bloated, that's no secret. It was really annoying to either wait a super long time for a single post to load, or the UI freezing up for no apparent reason, these were just some of the issues that were common for me in every browser I tried (Chrome, Firefox, Brave, etc.), even more annoying, is that it uses a ton of data, meaning on slower internet connections, getting posts to load can take extremely long. Lex can save up to 60% more bandwidth, while keeping very similar image/video quality, and the time to interactive is about 800ms-1.2s on average (with all images, scripts, stylesheets loaded, note: videos are not preloaded.)

As for the UI, I went for the newer reddit redesign, but with a little tweaking.

## How do I use Lex?

Unfortunately, unlike other open source reddit frontends, **Lex does not provide a demo website**, and there is two ways to build/use Lex.

1. [Downloading a Binary and running it](#downloading-binaries)
2. [Building Lex yourself](#building-instructions)

# βοΈ Installation Instructions

## Building Instructions

The only requirement to build the project is [Go](https://go.dev/dl)

If Go is installed, run the following commands in your terminal
```cmd
git clone https://github.com/cmd777/lex.git
cd lex
cd src
go get -u
go build
```
and, you're pretty much done, all that's left to do is launch the built binary, and navigate to `localhost:9090/r/{subreddit}`

## Downloading Binaries

To install LEX via automatically built binaries, go to the [releases](https://github.com/cmd777/lex/releases/latest) tab, and download the appropriate zip for your OS + ARCH, and extract it.

- For 32 bit Windows machines, download `lex-windows.zip`, then launch lex-i386-windows.exe
- For 64 bit Windows machines, download `lex-windows.zip`, then launch lex-amd64-windows.exe

<br>

- For 32 bit Linux machines, download `lex-linux.zip`, then launch lex-i386-linux
- For 64 bit Linux machines, download `lex-linux.zip`, then launch lex-amd64-linux

<br>

- For Intel MacOS machines, download `lex-osx.zip`, then launch lex-amd64-osx
- For M1 MacOS machines, download `lex-osx.zip`, then launch lex-arm64-osx

After launching, navigate to `localhost:9090/r/{subreddit}`, and you're done.

# π¬ Compatibility
|Chrome  | Edge | Safari | Firefox  | Opera  | IE   |
|:-----: | :--: | :----: | :------: | :---:  | :--: |
| > 41   | > 18 | > 10   |  > 48    | > 28   | β  |

<sub>The table displays the recommended versions for browsers, though older versions *may* be compatible to an extent.</sub>

<sub>Based on [Can I Use](https://caniuse.com) data</sub>

---

| ![](https://raw.githubusercontent.com/cmd777/lex/main/docs/images/windows.svg) Windows | ![](https://raw.githubusercontent.com/cmd777/lex/main/docs/images/linux.svg) Linux | ![](https://raw.githubusercontent.com/cmd777/lex/main/docs/images/macos.svg) macOS |
| :-----: | :---: | :---: |
| Windows 7 and higher | Kernel version 2.6.32 or later | macOS High Sierra 10.13 or newer

<sub>The table displays the **required** minimum versions for operating systems.</sub>

<sub>**LEX does not require administrator, or firewall privileges.**</sub>

<sub>Based on the [Go Documentation](https://github.com/golang/go/wiki/MinimumRequirements)</sub>

# π© Bugs, Issues, and other Important Information

Lex is still in very early stages of development, a lot of features are missing, and it might be prone to bugs, such as text overflowing, gallery buttons acting weird, and more.

I try to fix most of the critical bugs before pushing any changes, but if you find a bug, feel free to [create an issue](https://github.com/cmd777/lex/issues) for it.

For the features that are planned to be added, or the things that need to be fixed, you can refer to the [TODO List](https://github.com/cmd777/lex/blob/main/TODO.md)

<sub>**This list is not complete. Things are added when I find any problems, need to fix something, or from an idea I have.**</sub>

<sub>**The list is not in order of priority.**</sub>

I also work on Lex in my free time as a hobby, so development may be slow, thank you for your patience!

# π Legal Disclaimer

LEX is not affiliated with, sponsored, or endorsed by Reddit.

All content that is displayed on LEX has been sourced from Reddit. LEX does not host any of the content

In case of any issues with a post, such as copyright infringement, trademark infringement, or violation of Reddit's community rules, the reports should be directed to Reddit.

# π§° Technologies that were used to create Lex

- [Go](https://go.dev) β‘οΈ Programming Language
- [Humanize (go-humanize)](https://github.com/dustin/go-humanize) β‘οΈ Formatting time, numbers, etc.. to Human Friendly Units 
- [Fiber](https://github.com/gofiber/fiber) β‘οΈ HTTP Web Framework
- [Go-JSON](https://github.com/goccy/go-json) β‘οΈ Fast JSON Decoder
- [Bluemonday](https://github.com/microcosm-cc/bluemonday) β‘οΈ HTML Sanitizer
- [Blackfriday](https://github.com/russross/blackfriday/tree/v2) β‘οΈ Markdown Processor
- [SASS](https://sass-lang.com) β‘οΈ CSS Extension

<sub>Also used to create LEX:</sub>

- [Josefin Sans](https://fonts.google.com/specimen/Josefin+Sans) β‘οΈ Navbar, index font
- [Open Sans](https://fonts.google.com/specimen/Open+Sans) β‘οΈ Subreddit font
- [SVGRepo](https://www.svgrepo.com) β‘οΈ SVGs
- [Yqnn's SVG Path Editor](https://github.com/Yqnn/svg-path-editor) β‘οΈ Was used to edit almost all SVGs

# π Other Information

## Do I need a reddit account to use Lex?

No, a reddit account is not required to use Lex.

## Can I upvote / comment on posts?

Sorry, there are currently no plans to add support to upvoting and commenting.