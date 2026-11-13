<div>
  <h1>reFloof</h1>
  <div>
    <a href="https://github.com/C6Yfd-dfY6C/reFloof/releases">
      <img src="https://img.shields.io/github/v/release/C6Yfd-dfY6C/reFloof?label=version&style=flat-square" alt="Releases">
    </a>
    <a href="https://github.com/C6Yfd-dfY6C/reFloof/issues">
      <img src="https://img.shields.io/github/issues/C6Yfd-dfY6C/reFloof?&style=flat-square" alt="Issues">
    </a>
    <a href="https://github.com/C6Yfd-dfY6C/reFloof/pulls">
      <img src="https://img.shields.io/github/issues-pr/C6Yfd-dfY6C/reFloof?style=flat-square" alt="Pull Requests">
    </a>
    <a href="https://github.com/C6Yfd-dfY6C/reFloof/releases/latest/download/script.user.js">
      <img src="https://img.shields.io/github/downloads/C6Yfd-dfY6C/reFloof/total?style=flat-square" alt="Download">
    </a>
  </div>
</div>

reFloof is a compatibility conversion of [re621](https://github.com/re621/re621.Legacy) to bring over its features and experience to floofgens.net. The vast majority of the conversion was handled by an AI model, specifically Qwen 3.8 27B running locally on my PC.

I don't really have long-term goals for this. At best I may keep it in sync with re621 updates without adding any exotic features of my own, as I didn't want to "step outside my bounds" so to speak. Essentially, trying to keep it as "vanilla" as possible.

## Installation

The project is delivered via a userscript. This means that you need a script manager, such as [Tampermonkey](https://tampermonkey.net/), [Violentmonkey](https://violentmonkey.github.io/), or otherwise.  
With a script manager installed, click on the following link and follow the instructions on the new page.

<a href="https://github.com/C6Yfd-dfY6C/reFloof/releases/latest/download/script.user.js">
  <img src="https://img.shields.io/github/v/release/C6Yfd-dfY6C/reFloof?label=Install&style=for-the-badge">
</a>

## Features

For a complete feature overview, visit the original re621 website found at [re621.app](https://re621.app/).

## Contributing

Issues experienced may be bugs carried over from re621. I encourage you to test whatever bugs you encounter here with re621 as well and [open an issue on the re621 GitHub page](https://github.com/re621/re621.Legacy/issues) if the bug is present there as well.

## Building the Script

Start by cloning the repo as normal.  
Run `bun i` to install dependencies, then run `bun run build:prod` to start the build process.

Build artifacts are placed in the `/build/` folder. This process produces both the userscript and the extension version.

For development purposes, you may also wish to create an injector userscript by running `bun run injector:chrome` or `bun run injector:firefox`, which references the local file, removing the need to reload the script. Note that the firefox version requires running a [TamperDAV server](https://github.com/Tampermonkey/tamperdav).
