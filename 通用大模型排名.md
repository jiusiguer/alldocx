# Home | aider



## [https://aider.chat/#main-content](https://aider.chat/#main-content)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/docs/install.html](https://aider.chat/docs/install.html)

[](#installation)Installation
=============================

[](#get-started-quickly-with-aider-install)Get started quickly with aider-install
---------------------------------------------------------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

This will install aider in its own separate python environment. If needed, aider-install will also install a separate version of python 3.12 to use with aider.

Once aider is installed, there are also some [optional install steps](/docs/install/optional.html).

See the [usage instructions](https://aider.chat/docs/usage.html) to start coding with aider.

[](#one-liners)One-liners
-------------------------

These one-liners will install aider, along with python 3.12 if needed. They are based on the [uv installers](https://docs.astral.sh/uv/getting-started/installation/).

#### [](#windows)Windows

    powershell -ExecutionPolicy ByPass -c "irm https://aider.chat/install.ps1 | iex"
    

#### [](#mac--linux)Mac & Linux

Use curl to download the script and execute it with sh:

    curl -LsSf https://aider.chat/install.sh | sh
    

If your system doesn’t have curl, you can use wget:

    wget -qO- https://aider.chat/install.sh | sh
    

[](#install-with-uv)Install with uv
-----------------------------------

You can install aider with uv:

    python -m pip install uv  # If you need to install uv
    uv tool install --force --python python3.12 aider-chat@latest
    

This will install uv using your existing python version 3.8-3.13, and use it to install aider. If needed, uv will automatically install a separate python 3.12 to use with aider.

Also see the [docs on other methods for installing uv itself](https://docs.astral.sh/uv/getting-started/installation/).

[](#install-with-pipx)Install with pipx
---------------------------------------

You can install aider with pipx:

    python -m pip install pipx  # If you need to install pipx
    pipx install aider-chat
    

You can use pipx to install aider with python versions 3.9-3.12.

Also see the [docs on other methods for installing pipx itself](https://pipx.pypa.io/stable/installation/).

[](#other-install-methods)Other install methods
-----------------------------------------------

You can install aider with the methods described below, but one of the above methods is usually safer.

#### [](#install-with-pip)Install with pip

If you install with pip, you should consider using a [virtual environment](https://docs.python.org/3/library/venv.html) to keep aider’s dependencies separated.

You can use pip to install aider with python versions 3.9-3.12.

    # Install aider
    python -m pip install -U --upgrade-strategy only-if-needed aider-chat
    
    # To work with GPT-4o:
    aider --4o --openai-api-key sk-xxx...
    
    # To work with Claude 3.5 Sonnet:
    aider --sonnet --anthropic-api-key sk-xxx...
    

In some environments you may get “aider command not found” errors. You can try `python -m aider` or [see here for more info](/docs/troubleshooting/aider-not-found.html).

#### [](#installing-with-package-managers)Installing with package managers

It’s best to install aider using one of methods recommended above. While aider is available in a number of system package managers, they often install aider with incorrect dependencies.

[](#next-steps)Next steps…
--------------------------

There are some [optional install steps](/docs/install/optional.html) you could consider. See the [usage instructions](https://aider.chat/docs/usage.html) to start coding with aider.

* * *

Table of contents
-----------------

*   [Optional steps](/docs/install/optional.html)
*   [Aider with docker](/docs/install/docker.html)
*   [GitHub Codespaces](/docs/install/codespaces.html)
*   [Replit](/docs/install/replit.html)

---



## [https://aider.chat/docs/install/optional.html](https://aider.chat/docs/install/optional.html)

[](#optional-steps)Optional steps
=================================

The steps below are completely optional.

*   [Install git](#install-git)
*   [Get your API key](#get-your-api-key)
    *   [Working with other LLMs](#working-with-other-llms)
    *   [Store your api keys](#store-your-api-keys)
*   [Enable Playwright](#enable-playwright)
*   [Enable voice coding](#enable-voice-coding)
*   [Add aider to your IDE/editor](#add-aider-to-your-ideeditor)
    *   [NeoVim](#neovim)
    *   [VS Code](#vs-code)
    *   [Other editors](#other-editors)
*   [Install the development version of aider](#install-the-development-version-of-aider)

[](#install-git)Install git
---------------------------

Aider works best if you have git installed. Here are [instructions for installing git in various environments](https://github.com/git-guides/install-git).

[](#get-your-api-key)Get your API key
-------------------------------------

To work with OpenAI’s models like GPT-4o or o1-preview you need a paid [OpenAI API key](https://help.openai.com/en/articles/4936850-where-do-i-find-my-secret-api-key). Note that this is different than being a “ChatGPT Plus” subscriber.

To work with Anthropic’s models like Claude 3.5 Sonnet you need a paid [Anthropic API key](https://docs.anthropic.com/claude/reference/getting-started-with-the-api).

### [](#working-with-other-llms)Working with other LLMs

Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

### [](#store-your-api-keys)Store your api keys

You can [store your api keys in configuration or env files](/docs/config/api-keys.html) and they will be loaded automatically whenever you run aider.

[](#enable-playwright)Enable Playwright
---------------------------------------

Aider supports adding web pages to the chat with the `/web <url>` command. When you add a url to the chat, aider fetches the page and scrapes its content.

By default, aider uses the `httpx` library to scrape web pages, but this only works on a subset of web pages. Some sites explicitly block requests from tools like httpx. Others rely heavily on javascript to render the page content, which isn’t possible using only httpx.

Aider works best with all web pages if you install Playwright’s chromium browser and its dependencies:

    playwright install --with-deps chromium
    

See the [Playwright for Python documentation](https://playwright.dev/python/docs/browsers#install-system-dependencies) for additional information.

[](#enable-voice-coding)Enable voice coding
-------------------------------------------

Aider supports [coding with your voice](https://aider.chat/docs/usage/voice.html) using the in-chat `/voice` command. Aider uses the [PortAudio](http://www.portaudio.com) library to capture audio. Installing PortAudio is completely optional, but can usually be accomplished like this:

*   For Windows, there is no need to install PortAudio.
*   For Mac, do `brew install portaudio`
*   For Linux, do `sudo apt-get install libportaudio2`
    *   Some linux environments may also need `sudo apt install libasound2-plugins`

[](#add-aider-to-your-ideeditor)Add aider to your IDE/editor
------------------------------------------------------------

You can use [aider’s `--watch-files` mode](https://aider.chat/docs/usage/watch.html) to integrate with any IDE or editor.

There are a number of 3rd party aider plugins for various IDE/editors. It’s not clear how well they are tracking the latest versions of aider, so it may be best to just run the latest aider in a terminal alongside your editor and use `--watch-files`.

### [](#neovim)NeoVim

[joshuavial](https://github.com/joshuavial) provided a NeoVim plugin for aider:

[https://github.com/joshuavial/aider.nvim](https://github.com/joshuavial/aider.nvim)

### [](#vs-code)VS Code

You can run aider inside a VS Code terminal window. There are a number of 3rd party [aider plugins for VSCode](https://marketplace.visualstudio.com/search?term=aider%20-kodu&target=VSCode&category=All%20categories&sortBy=Relevance).

### [](#other-editors)Other editors

If you are interested in creating an aider plugin for your favorite editor, please let us know by opening a [GitHub issue](https://github.com/Aider-AI/aider/issues).

[](#install-the-development-version-of-aider)Install the development version of aider
-------------------------------------------------------------------------------------

If you want the very latest development version of aider you can install it like this:

    aider --install-main-branch

---



## [https://aider.chat/docs/install/docker.html](https://aider.chat/docs/install/docker.html)

[](#aider-with-docker)Aider with docker
=======================================

Aider is available as 2 docker images:

*   `paulgauthier/aider` installs the aider core, a smaller image that’s good to get started quickly.
*   `paulgauthier/aider-full` installs aider will all the optional extras.

The full image has support for features like interactive help, the browser GUI and support for using Playwright to scrape web pages. The core image can still use these features, but they will need to be installed the first time you access them. Since containers are ephemeral, the extras will need to be reinstalled the next time you launch the aider core container.

### [](#aider-core)Aider core

    docker pull paulgauthier/aider
    docker run -it --user $(id -u):$(id -g) --volume $(pwd):/app paulgauthier/aider --openai-api-key $OPENAI_API_KEY [...other aider args...]
    

### [](#full-version)Full version

    docker pull paulgauthier/aider-full
    docker run -it --user $(id -u):$(id -g) --volume $(pwd):/app paulgauthier/aider-full --openai-api-key $OPENAI_API_KEY [...other aider args...]
    

[](#how-to-use-it)How to use it
-------------------------------

You should run the above commands from the root of your git repo, since the `--volume` arg maps your current directory into the docker container. Given that, you need to be in the root of your git repo for aider to be able to see the repo and all its files.

You should be sure your that git repo config contains your user name and email, since the docker container won’t have your global git config. Run these commands while in your git repo, before you do the `docker run` command:

    git config user.email "you@example.com"
    git config user.name "Your Name"
    

[](#limitations)Limitations
---------------------------

*   When you use the in-chat `/run` command, it will be running shell commands _inside the docker container_. So those commands won’t be running in your local environment, which may make it tricky to `/run` tests, etc for your project.
*   The `/voice` command won’t work unless you can figure out how to give the docker container access to your host audio device. The container has libportaudio2 installed, so it should work if you can do that.

---



## [https://aider.chat/docs/install/codespaces.html](https://aider.chat/docs/install/codespaces.html)

[](#github-codespaces)GitHub Codespaces
=======================================

You can use aider in GitHub Codespaces via the built-in Terminal pane. See below for an example, but you can just follow the [main install instructions](/docs/install.html) inside your codespace terminal.

 [Install aider in GitHub Codespaces](/assets/codespaces.mp4)

---



## [https://aider.chat/docs/install/replit.html](https://aider.chat/docs/install/replit.html)

### [](#replit)Replit

To use aider with pipx on replit, you can run these commands in the replit shell:

    pip install pipx
    pipx run aider-chat ...normal aider args...
    

If you install aider with pipx on replit and try and run it as just `aider` it will crash with a missing `libstdc++.so.6` library.

---



## [https://aider.chat/docs/usage.html](https://aider.chat/docs/usage.html)

[](#usage)Usage
===============

Run `aider` with the source code files you want to edit. These files will be “added to the chat session”, so that aider can see their contents and edit them for you. They can be existing files or the name of files you want aider to create for you.

    aider <file1> <file2> ...
    

At the aider `>` prompt, ask for code changes and aider will edit those files to accomplish your request.

    $ aider factorial.py
    
    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 258 files
    Repo-map: using 1024 tokens
    Use /help to see in-chat commands, run with --help to see cmd line args
    ───────────────────────────────────────────────────────────────────────
    > Make a program that asks for a number and prints its factorial
    
    ...
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

[](#adding-files)Adding files
-----------------------------

To edit files, you need to “add them to the chat”. Do this by naming them on the aider command line. Or, you can use the in-chat `/add` command to add files.

Only add the files that need to be edited for your task. Don’t add a bunch of extra files. If you add too many files, the LLM can get overwhelmed and confused (and it costs more tokens). Aider will automatically pull in content from related files so that it can [understand the rest of your code base](https://aider.chat/docs/repomap.html).

You can use aider without adding any files, and it will try to figure out which files need to be edited based on your requests.

You’ll get the best results if you think about which files need to be edited. Add **just** those files to the chat. Aider will include relevant context from the rest of your repo.

[](#llms)LLMs
-------------

Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

    # GPT-4o
    $ aider --4o
    
    # Claude 3.5 Sonnet
    $ aider --sonnet
    

Or you can run `aider --model XXX` to launch aider with another model. During your chat you can switch models with the in-chat `/model` command.

[](#making-changes)Making changes
---------------------------------

Ask aider to make changes to your code. It will show you some diffs of the changes it is making to complete you request. [Aider will git commit all of its changes](/docs/git.html), so they are easy to track and undo.

You can always use the `/undo` command to undo AI changes that you don’t like.

* * *

Table of contents
-----------------

*   [Tips](/docs/usage/tips.html)
*   [In-chat commands](/docs/usage/commands.html)
*   [Chat modes](/docs/usage/modes.html)
*   [Tutorial videos](/docs/usage/tutorials.html)
*   [Voice-to-code with aider](/docs/usage/voice.html)
*   [Images & web pages](/docs/usage/images-urls.html)
*   [Prompt caching](/docs/usage/caching.html)
*   [Aider in your IDE](/docs/usage/watch.html)
*   [Aider in your browser](/docs/usage/browser.html)
*   [Specifying coding conventions](/docs/usage/conventions.html)
*   [Copy/paste with web chat](/docs/usage/copypaste.html)
*   [Linting and testing](/docs/usage/lint-test.html)
*   [Editing config & text files](/docs/usage/not-code.html)

---



## [https://aider.chat/docs/usage/tips.html](https://aider.chat/docs/usage/tips.html)

[](#tips)Tips
=============

[](#just-add-the-files-that-need-to-be-changed-to-the-chat)Just add the files that need to be changed to the chat
-----------------------------------------------------------------------------------------------------------------

Take a moment and think about which files will need to be changed. Aider can often figure out which files to edit all by itself, but the most efficient approach is for you to add the files to the chat.

[](#dont-add-lots-of-files-to-the-chat)Don’t add lots of files to the chat
--------------------------------------------------------------------------

Just add the files you think need to be edited. Too much irrelevant code will distract and confuse the LLM. Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html) so is usually aware of relevant classes/functions/methods elsewhere in your code base. It’s ok to add 1-2 highly relevant files that don’t need to be edited, but be selective.

[](#break-your-goal-down-into-bite-sized-steps)Break your goal down into bite sized steps
-----------------------------------------------------------------------------------------

Do them one at a time. Adjust the files added to the chat as you go: `/drop` files that don’t need any more changes, `/add` files that need changes for the next step.

[](#for-complex-changes-discuss-a-plan-first)For complex changes, discuss a plan first
--------------------------------------------------------------------------------------

Use the [`/ask` command](modes.html) to make a plan with aider. Once you are happy with the approach, just say “go ahead” without the `/ask` prefix.

[](#if-aider-gets-stuck)If aider gets stuck
-------------------------------------------

*   Use `/clear` to discard the chat history and make a fresh start.
*   Can you `/drop` any extra files?
*   Use `/ask` to discuss a plan before aider starts editing code.
*   Use the [`/model` command](commands.html) to switch to a different model and try again. Switching between GPT-4o and Sonnet will often get past problems.
*   If aider is hopelessly stuck, just code the next step yourself and try having aider code some more after that. Take turns and pair program with aider.

[](#creating-new-files)Creating new files
-----------------------------------------

If you want aider to create a new file, add it to the repository first with `/add <file>`. This way aider knows this file exists and will write to it. Otherwise, aider might write the changes to an existing file. This can happen even if you ask for a new file, as LLMs tend to focus a lot on the existing information in their contexts.

[](#fixing-bugs-and-errors)Fixing bugs and errors
-------------------------------------------------

If your code is throwing an error, use the [`/run` command](commands.html) to share the error output with the aider. Or just paste the errors into the chat. Let the aider figure out how to fix the bug.

If test are failing, use the [`/test` command](lint-test.html) to run tests and share the error output with the aider.

[](#providing-docs)Providing docs
---------------------------------

LLMs know about a lot of standard tools and libraries, but may get some of the fine details wrong about API versions and function arguments.

You can provide up-to-date documentation in a few ways:

*   Paste doc snippets into the chat.
*   Include a URL to docs in your chat message and aider will scrape and read it. For example: `Add a submit button like this https://ui.shadcn.com/docs/components/button`.
*   Use the [`/read` command](commands.html) to read doc files into the chat from anywhere on your filesystem.
*   If you have coding conventions or standing instructions you want aider to follow, consider using a [conventions file](conventions.html).

[](#interrupting--inputting)Interrupting & inputting
----------------------------------------------------

Use Control-C to interrupt aider if it isn’t providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply with more information or direction.

You can send long, multi-line messages in the chat in a few ways:

*   Paste a multi-line message directly into the chat.
*   Enter `{` alone on the first line to start a multiline message and `}` alone on the last line to end it.
    *   Or, start with `{tag` (where “tag” is any sequence of letters/numbers) and end with `tag}`. This is useful when you need to include closing braces `}` in your message.
*   Use Meta-ENTER to start a new line without sending the message (Esc+ENTER in some environments).
*   Use `/paste` to paste text from the clipboard into the chat.
*   Use the `/editor` command to open your editor to create the next chat message. See [editor configuration docs](/docs/config/editor.html) for more info.
*   Use multiline-mode, which swaps the function of Meta-Enter and Enter, so that Enter inserts a newline, and Meta-Enter submits your command. To enable multiline mode:
    *   Use the `/multiline-mode` command to toggle it during a session.
    *   Use the `--multiline` switch.

Example with a tag:

    {python
    def hello():
        print("Hello}")  # Note: contains a brace
    python}
    

People often ask for SHIFT-ENTER to be a soft-newline. Unfortunately there is no portable way to detect that keystroke in terminals.

---



## [https://aider.chat/docs/usage/commands.html](https://aider.chat/docs/usage/commands.html)

[](#in-chat-commands)In-chat commands
=====================================

*   [Slash commands](#slash-commands)
*   [Entering multi-line chat messages](#entering-multi-line-chat-messages)
*   [Interrupting with CONTROL-C](#interrupting-with-control-c)
*   [Keybindings](#keybindings)
    *   [Emacs](#emacs)
    *   [Vi](#vi)

[](#slash-commands)Slash commands
---------------------------------

Aider supports commands from within the chat, which all start with `/`.

Command

Description

**/add**

Add files to the chat so aider can edit them or review them in detail

**/architect**

Enter architect/editor mode using 2 different models. If no prompt provided, switches to architect/editor mode.

**/ask**

Ask questions about the code base without editing any files. If no prompt provided, switches to ask mode.

**/chat-mode**

Switch to a new chat mode

**/clear**

Clear the chat history

**/code**

Ask for changes to your code. If no prompt provided, switches to code mode.

**/commit**

Commit edits to the repo made outside the chat (commit message optional)

**/copy**

Copy the last assistant message to the clipboard

**/copy-context**

Copy the current chat context as markdown, suitable to paste into a web UI

**/diff**

Display the diff of changes since the last message

**/drop**

Remove files from the chat session to free up context space

**/editor**

Open an editor to write a prompt

**/exit**

Exit the application

**/git**

Run a git command (output excluded from chat)

**/help**

Ask questions about aider

**/lint**

Lint and fix in-chat files or all dirty files if none in chat

**/load**

Load and execute commands from a file

**/ls**

List all known files and indicate which are included in the chat session

**/map**

Print out the current repository map

**/map-refresh**

Force a refresh of the repository map

**/model**

Switch to a new LLM

**/models**

Search the list of available models

**/multiline-mode**

Toggle multiline mode (swaps behavior of Enter and Meta+Enter)

**/paste**

Paste image/text from the clipboard into the chat. Optionally provide a name for the image.

**/quit**

Exit the application

**/read-only**

Add files to the chat that are for reference only, or turn added files to read-only

**/report**

Report a problem by opening a GitHub Issue

**/reset**

Drop all files and clear the chat history

**/run**

Run a shell command and optionally add the output to the chat (alias: !)

**/save**

Save commands to a file that can reconstruct the current chat session’s files

**/settings**

Print out the current settings

**/test**

Run a shell command and add the output to the chat on non-zero exit code

**/tokens**

Report on the number of tokens used by the current chat context

**/undo**

Undo the last git commit if it was done by aider

**/voice**

Record and transcribe voice input

**/web**

Scrape a webpage, convert to markdown and send in a message

You can easily re-send commands or messages. Use the up arrow ⬆ to scroll back or CONTROL-R to search your message history.

[](#entering-multi-line-chat-messages)Entering multi-line chat messages
-----------------------------------------------------------------------

You can send long, multi-line messages in the chat in a few ways:

*   Paste a multi-line message directly into the chat.
*   Enter `{` alone on the first line to start a multiline message and `}` alone on the last line to end it.
    *   Or, start with `{tag` (where “tag” is any sequence of letters/numbers) and end with `tag}`. This is useful when you need to include closing braces `}` in your message.
*   Use Meta-ENTER to start a new line without sending the message (Esc+ENTER in some environments).
*   Use `/paste` to paste text from the clipboard into the chat.
*   Use the `/editor` command to open your editor to create the next chat message. See [editor configuration docs](/docs/config/editor.html) for more info.
*   Use multiline-mode, which swaps the function of Meta-Enter and Enter, so that Enter inserts a newline, and Meta-Enter submits your command. To enable multiline mode:
    *   Use the `/multiline-mode` command to toggle it during a session.
    *   Use the `--multiline` switch.

Example with a tag:

    {python
    def hello():
        print("Hello}")  # Note: contains a brace
    python}
    

People often ask for SHIFT-ENTER to be a soft-newline. Unfortunately there is no portable way to detect that keystroke in terminals.

[](#interrupting-with-control-c)Interrupting with CONTROL-C
-----------------------------------------------------------

It’s always safe to use Control-C to interrupt aider if it isn’t providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to the LLM with more information or direction.

[](#keybindings)Keybindings
---------------------------

The interactive prompt is built with [prompt-toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) which provides emacs and vi keybindings.

### [](#emacs)Emacs

*   `Up Arrow` : Move up one line in the current message.
*   `Down Arrow` : Move down one line in the current message.
*   `Ctrl-Up` : Scroll back through previously sent messages.
*   `Ctrl-Down` : Scroll forward through previously sent messages.
*   `Ctrl-A` : Move cursor to the start of the line.
*   `Ctrl-B` : Move cursor back one character.
*   `Ctrl-D` : Delete the character under the cursor.
*   `Ctrl-E` : Move cursor to the end of the line.
*   `Ctrl-F` : Move cursor forward one character.
*   `Ctrl-K` : Delete from the cursor to the end of the line.
*   `Ctrl-L` : Clear the screen.
*   `Ctrl-N` : Move down to the next history entry.
*   `Ctrl-P` : Move up to the previous history entry.
*   `Ctrl-R` : Reverse search in command history.

### [](#vi)Vi

To use vi/vim keybindings, run aider with the `--vim` switch.

*   `Up Arrow` : Move up one line in the current message.
*   `Down Arrow` : Move down one line in the current message.
*   `Ctrl-Up` : Scroll back through previously sent messages.
*   `Ctrl-Down` : Scroll forward through previously sent messages.
*   `Esc` : Switch to command mode.
*   `i` : Switch to insert mode.
*   `a` : Move cursor one character to the right and switch to insert mode.
*   `A` : Move cursor to the end of the line and switch to insert mode.
*   `I` : Move cursor to the beginning of the line and switch to insert mode.
*   `h` : Move cursor one character to the left.
*   `j` : Move cursor down one line.
*   `k` : Move cursor up one line.
*   `l` : Move cursor one character to the right.
*   `w` : Move cursor forward one word.
*   `b` : Move cursor backward one word.
*   `0` : Move cursor to the beginning of the line.
*   `$` : Move cursor to the end of the line.
*   `x` : Delete the character under the cursor.
*   `dd` : Delete the current line.
*   `u` : Undo the last change.
*   `Ctrl-R` : Redo the last undone change.

---



## [https://aider.chat/docs/usage/modes.html](https://aider.chat/docs/usage/modes.html)

[](#chat-modes)Chat modes
=========================

Aider has a few different chat modes:

*   `code` - Aider will make changes to your code to satisfy your requests.
*   `architect` - Aider will first propose a solution, then ask if you want it to turn that proposal into edits to your files.
*   `ask` - Aider will answer questions about your code, but never edit it.
*   `help` - Aider will answer questions about using aider, configuring, troubleshooting, etc.

By default, aider starts in “code” mode. As you are talking, you can send individual messages in a specific mode using `/code`, `/architect`, `/ask`, and `/help` commands: Using these `/`\-commands applies just to that particular message. Your next message will go back to the active mode (usually “code” mode by default).

You can switch the active mode in a sticky way with the `/chat-mode <mode>` command:

    /chat-mode code
    /chat-mode architect
    /chat-mode ask
    /chat-mode help
    

Or you can switch between coding modes using these commands without arguments:

    /code
    /architect
    /ask
    

Or you can launch aider in one of the modes with the `--chat-mode <mode>` switch. There is also a special shortcut `--architect` to launch in `--chat-mode architect`.

[](#architect-mode-and-the-editor-model)Architect mode and the editor model
---------------------------------------------------------------------------

When you are in architect mode, aider sends your request to two models:

1.  First, it sends your request to the main active model. The main model is configured with `/model`, `--model` or the shortcut switches like `--sonnet`. After the main model replies, aider will offer to edit the files based on the response.
    
2.  To edit the files, aider sends a second LLM request asking for specific code editing instructions. This request goes to the “editor” model. Aider has built in defaults to select an editor model based on your main model. Or, you can choose an editor model yourself with `--editor-model <model>`.
    

Architect mode produces better results than code mode, but uses two LLM requests. This probably makes it slower and more expensive than using code mode.

Architect mode is especially useful with OpenAI’s o1 models, which are strong at reasoning but less capable at editing files. Pairing an o1 architect with an editor model like GPT-4o or Sonnet will give the best results.

But architect mode is also quite helpful when you use GPT-4o or Sonnet at both the architect and the editor. Allowing the model two requests to solve the problem and edit the files usually provides a better result.

The editor model uses one of aider’s edit formats to let the LLM edit source files. Aider will pick a suitable edit format by default, but you can customize it with `--editor-edit-format <format>`. The [“editor-diff” and “editor-whole” edit formats](/docs/more/edit-formats.html#editor-diff-and-editor-whole) are the recommended edit formats when using architect mode. See this article on [aider’s architect/editor mode](/2024/09/26/architect.html) for more details.

[](#examples)Examples
---------------------

> Aider v0.47.1-dev  
> Models: claude-3-5-sonnet-20240620 with diff edit format  
> Git repo: .git with 298 files  
> Repo-map: using 1024 tokens  
> Use /help to see in-chat commands, run with –help to see cmd line args

#### [](#ask-what-is-this-repo)/ask What is this repo?

This is the source code to the popular django package.

#### [](#help-how-do-i-use-ollama)/help How do I use ollama?

Run `aider --model ollama/<ollama-model>`. See these docs for more info: https://aider.chat/docs/llms/ollama.html

#### [](#code-add-a-function-to-calculate-the-factorial-of-a-number)/code Add a function to calculate the factorial of a number

Certainly! I’ll add a function to calculate the factorial of a number. Here’s the change:

    def factorial(n):
        if n == 0 or n == 1:
            return 1
        else:
            return n * factorial(n - 1)
    
    # Example usage
    print(factorial(5))  # Output: 120
    

This function uses recursion to calculate the factorial. It’s been added to your code.

#### [](#architect-can-we-make-this-simpler)/architect Can we make this simpler?

Yes, you could replace the `factorial()` function with a call to the `math.factorial()` builtin. This way you don’t have to maintain a custom factorial implementation, and the builtin function is well optimized.

> Edit the files? (Y)es/(N)o \[Yes\]: Yes

    <<<<<<< SEARCH
    def factorial(n):
        if n == 0 or n == 1:
            return 1
        else:
            return n * factorial(n - 1)
    =======
    from math import factorial
    >>>>>>> REPLACE

---



## [https://aider.chat/docs/usage/tutorials.html](https://aider.chat/docs/usage/tutorials.html)

[](#tutorial-videos)Tutorial videos
===================================

Here are some tutorial videos made by aider users:

*   [Using Architect/Editor mode](https://www.youtube.com/watch?v=OPXslklVBZc) – AICodeKing
*   [Using aider to incrementally build a non-trivial app](https://youtu.be/QlUt06XLbJE) – IndyDevDan
*   [Aider and Replit on mobile with your voice](https://x.com/itsPaulAi/status/1830987090617831810) – Paul Couvert
*   [Aider is the OG AI Coding King (Mermaid Diagram AI Agent)](https://www.youtube.com/watch?v=ag-KxYS8Vuw) – IndyDevDan
*   [Installing aider in replit and making a Trello clone](https://x.com/itspaulai/status/1828834199597633724) – Paul Couvert
*   [Step-by-Step Development Environment Setup for AI-Assisted Coding](https://www.youtube.com/watch?v=DnBVgfe6ZQM) – Coding the Future With AI
*   [Generate FULL-STACK Apps with Claude 3.5 Sonnet](https://youtu.be/sKeIZGW8xzg) – AICodeKing
*   [Creating Games with AI from Start-To-End](https://youtu.be/sOd2YYZFMUs) – AICodeKing
*   [Claude 3.5 and aider: Use AI Assistants to Build AI Apps](https://youtu.be/0hIisJ3xAdU) – Coding the Future With AI
*   [Develop a Full-stack App Without Writing ANY Code](https://youtu.be/dzOWn8TI738) – WorldofAI
*   [Generate Games with AI (w/ Local LLMs)](https://youtu.be/DjVJpGzQbSA) – AICodeKing
*   [Aider tips and Example use](https://www.youtube.com/watch?v=OsChkvGGDgw) – techfren
*   [Aider and Claude 3.5: Develop a Full-stack App Without Writing ANY Code!](https://www.youtube.com/watch?v=BtAqHsySdSY) – Coding the Future With AI
*   [Generate application with just one prompt using Aider](https://www.youtube.com/watch?v=Y-_0VkMUiPc&t=78s) – AICodeKing
*   [Aider : the production ready AI coding assistant you’ve been waiting for](https://www.youtube.com/watch?v=zddJofosJuM) – Learn Code With JV
*   [Holy Grail: FREE Coding Assistant That Can Build From EXISTING CODE BASE](https://www.youtube.com/watch?v=df8afeb1FY8) – Matthew Berman
*   [Aider: This AI Coder Can Create AND Update Git Codebases](https://www.youtube.com/watch?v=EqLyFT78Sig) – Ian Wootten

Thanks to all these great creators for taking the time to share their experiences coding with aider!

---



## [https://aider.chat/docs/usage/voice.html](https://aider.chat/docs/usage/voice.html)

[](#voice-to-code-with-aider)Voice-to-code with aider
=====================================================

Speak with aider about your code! Request new features, test cases or bug fixes using your voice and let aider do the work of editing the files in your local git repo. As with all of aider’s capabilities, you can use voice-to-code with an existing repo or to start a new project.

Voice support fits quite naturally into aider’s AI pair programming chat interface. Now you can fluidly switch between voice and text chat when you ask aider to edit your code.

[](#how-to-use-voice-to-code)How to use voice-to-code
-----------------------------------------------------

Use the in-chat `/voice` command to start recording, and press `ENTER` when you’re done speaking. Your voice coding instructions will be transcribed, as if you had typed them into the aider chat session.

See the [installation instructions](https://aider.chat/docs/install/optional.html#enable-voice-coding) for information on how to enable the `/voice` command.

  

> Aider v0.11.2-dev  
> Added app.py to the chat.

#### [](#voice)/voice

> Recording, press ENTER when done... 3.5sec

“ add a factorial endpoint that uses math factorial ”

#### [](#add-a-factorial-endpoint-that-uses-mathfactorial)Add a factorial endpoint that uses math.factorial.

To add a factorial endpoint to the Flask application, we need to modify the `app.py` file.

Here are the steps:

1.  Add a new route `/fact/<int:x>` to the Flask application.
2.  In the function for this route, call `math.factorial(x)` and return the result as a string.

Here is the _edit block_ for these changes:

    app.py
    <<<<<<< HEAD
    if __name__ == '__main__':
        print("Starting...")
        app.run()
    =======
    @app.route('/fact/<int:x>')
    def factorial(x):
        result = math.factorial(x)
        return str(result)
    
    if __name__ == '__main__':
        print("Starting...")
        app.run()
    >>>>>>> updated
    

> Applied edit to app.py  
> Commit ef9e3e7 aider: Add a factorial endpoint that uses math.factorial.

---



## [https://aider.chat/docs/usage/images-urls.html](https://aider.chat/docs/usage/images-urls.html)

[](#images--web-pages)Images & web pages
========================================

You can add images and URLs to the aider chat.

[](#images)Images
-----------------

Aider supports working with image files for many vision-capable models like GPT-4o and Claude 3.5 Sonnet. Adding images to a chat can be helpful in many situations:

*   Add screenshots of web pages or UIs that you want aider to build or modify.
*   Show aider a mockup of a UI you want to build.
*   Screenshot an error message that is otherwise hard to copy & paste as text.
*   Etc.

You can add images to the chat just like you would add any other file:

*   Use `/add <image-filename>` from within the chat
*   Use `/paste` to paste an image from your clipboard into the chat.
*   Launch aider with image filenames on the command line: `aider <image-filename>` along with any other command line arguments you need.

[](#web-pages)Web pages
-----------------------

Aider can scrape the text from URLs and add it to the chat. This can be helpful to:

*   Include documentation pages for less popular APIs.
*   Include the latest docs for libraries or packages that are newer than the model’s training cutoff date.
*   Etc.

To add URLs to the chat:

*   Use `/web <url>`
*   Just paste the URL into the chat and aider will ask if you want to add it.

You can also scrape web pages from the command line to see the markdown version that aider produces:

    python -m aider.scrape https://aider.chat/docs/usage/tips.html

---



## [https://aider.chat/docs/usage/caching.html](https://aider.chat/docs/usage/caching.html)

[](#prompt-caching)Prompt caching
=================================

Aider supports prompt caching for cost savings and faster coding. Currently Anthropic provides caching for Sonnet and Haiku, and DeepSeek provides caching for Coder.

Aider organizes the chat history to try and cache:

*   The system prompt.
*   Read only files added with `--read` or `/read-only`.
*   The repository map.
*   The editable files that have been added to the chat.

[](#usage)Usage
---------------

Run aider with `--cache-prompts` or add that setting to your [configuration files](/docs/config.html).

Due to limitations in the provider APIs, caching statistics and costs are not available when streaming responses. To turn off streaming, use `--no-stream`.

When caching is enabled, it will be noted for the main model when aider launches:

    Main model: claude-3-5-sonnet-20240620 with diff edit format, prompt cache, infinite output
    

[](#preventing-cache-expiration)Preventing cache expiration
-----------------------------------------------------------

Aider can ping the provider to keep your prompt cache warm and prevent it from expiring. By default, Anthropic keeps your cache for 5 minutes. Use `--cache-keepalive-pings N` to tell aider to ping every 5 minutes to keep the cache warm. Aider will ping up to `N` times over a period of `N*5` minutes after each message you send.

---



## [https://aider.chat/docs/usage/watch.html](https://aider.chat/docs/usage/watch.html)

[](#aider-in-your-ide)Aider in your IDE
=======================================

 [Aider browser UI demo video](/assets/watch.mp4)

[](#ai-comments)AI comments
---------------------------

If you run aider with `--watch-files`, it will watch all files in your repo and look for any AI coding instructions you add using your favorite IDE or text editor.

Specifically, aider looks for one-liner comments (# … or // …) that either start or end with `AI`, `AI!` or `AI?` like these:

    # Make a snake game. AI!
    # What is the purpose of this method AI?
    

Or in `//` comment languages…

    // Write a protein folding prediction engine. AI!
    

Aider will take note of all the comments that start or end with `AI`. Comments that include `AI!` with an exclamation point or `AI?` with a question mark are special. They triggers aider to take action to collect _all_ the AI comments and use them as your instructions.

*   `AI!` triggers aider to make changes to your code.
*   `AI?` triggers aider to answer your question.

See the demo video above that shows aider working with AI comments in VSCode.

[](#example)Example
-------------------

For example, if you included this AI comment in your code:

    function factorial(n) // Implement this. AI!
    

Then aider would update the file and implement the function:

    function factorial(n) {
      if (n === 0 || n === 1) {
        return 1;
      } else {
        return n * factorial(n - 1);
      }
    }
    

[](#comment-styles)Comment styles
---------------------------------

Aider only watches for these types of **one-liner** comments:

    # Python and bash style
    // Javascript style
    -- SQL style
    

Aider will look for those comment types in all files. You can use them into any code file you’re editing, even if they aren’t the correct comment syntax for that language.

[](#multiple-uses)Multiple uses
-------------------------------

This capability is quite flexible and powerful, and can be used in many ways.

### [](#in-context-instructions)In-context instructions

You can add an AI comment in the function you want changed, explaining the change request in-context right where you want the changes.

    app.get('/sqrt/:n', (req, res) => {
        const n = parseFloat(req.params.n);
    
        // Add error handling for NaN and less than zero. AI!
    
        const result = math.sqrt(n);
        res.json({ result: result });
    });
    

### [](#multiple-comments)Multiple comments

You can add multiple `AI` comments without the `!`, before triggering aider with a final `AI!`. Also keep in mind that you can spread the AI comments across multiple files, if you want to coordinate changes in multiple places. Just use `AI!` last, to trigger aider.

    @app.route('/factorial/<int:n>')
    def factorial(n):
        if n < 0:
            return jsonify(error="Factorial is not defined for negative numbers"), 400
    
        # AI: Refactor this code...
    
        result = 1
        for i in range(1, n + 1):
            result *= i
    
        # ... into to a compute_factorial() function. AI!
    
        return jsonify(result=result)
    

### [](#long-form-instructions)Long form instructions

You can add a block of comments, with longer instructions. Just be sure to start or end one of the lines with `AI` or `AI!` to draw aider’s attention to the block.

    # Make these changes: AI!
    # - Add a proper main() function
    # - Use Click to process cmd line args
    # - Accept --host and --port args
    # - Print a welcome message that includes the listening url
    
    if __name__ == "__main__":
        app.run(debug=True)
    

### [](#add-a-file-to-the-aider-chat)Add a file to the aider chat

Rather than using `/add` to add a file inside the aider chat, you can simply put an `#AI` comment in it and save the file. You can undo/remove the comment immediately if you like, the file will still be added to the aider chat.

[](#also-use-aider-chat-in-the-terminal)Also use aider chat in the terminal
---------------------------------------------------------------------------

It can be really helpful to get a change started with AI comments. But sometimes you want to build on or refine those changes. You can of course continue to do that with AI comments, but it can sometimes be effective to switch over to the aider terminal chat. The chat has the history of the AI comments you just made, so you can continue on naturally from there.

You can also use the normal aider chat in your terminal to work with many of aider’s more advanced features:

*   Use `/undo` to revert changes you don’t like. Although you may also be able to use your IDE’s undo function to step back in the file history.
*   Use [chat modes](https://aider.chat/docs/usage/modes.html) to ask questions or get help.
*   Manage the chat context with `/tokens`, `/clear`, `/drop`, `/reset`. Adding an AI comment will add the file to the chat. Periodically, you may want remove extra context that is no longer needed.
*   [Fix lint and test errors](https://aider.chat/docs/usage/lint-test.html).
*   Run shell commands.
*   Etc.

[](#you-can-be-lazy)You can be lazy
-----------------------------------

The examples above all show AI comments with full sentences, proper capitalization, punctuation, etc. This was done to help explain how AI comments work, but is not needed in practice.

Most LLMs are perfectly capable of dealing with ambiguity and inferring implied intent. This often allows you to be quite lazy with your AI comments. In particular, you can start and end comments with lowercase `ai` and `ai!`, but you can also be much more terse with the request itself. Below are simpler versions of some of the examples given above.

When the context clearly implies the needed action, `ai!` might be all you need. For example, to implement a factorial function in a program full of other math functions either of these approaches would probably work:

    function factorial(n) // ai!
    

Or…

    // add factorial() ai!
    

Rather than a long, explicit comment like “Add error handling for NaN and less than zero,” you can let aider infer more about the request. This simpler comment may be sufficient:

    app.get('/sqrt/:n', (req, res) => {
        const n = parseFloat(req.params.n);
    
        // add error handling ai!
    
        const result = math.sqrt(n);
        res.json({ result: result });
    });
    

Similarly, this refactor probably could have been requested with fewer words, like this:

    @app.route('/factorial/<int:n>')
    def factorial(n):
        if n < 0:
            return jsonify(error="Factorial is not defined for negative numbers"), 400
    
        # ai refactor...
    
        result = 1
        for i in range(1, n + 1):
            result *= i
    
        # ... to compute_factorial() ai!
    
        return jsonify(result=result)
    

As you use aider with your chosen LLM, you can develop a sense for how explicit you need to make your AI comments.

[](#behind-the-scenes)Behind the scenes
---------------------------------------

Aider sends your AI comments to the LLM with the [repo map](https://aider.chat/docs/repomap.html) and all the other code context you’ve added to the chat.

It also pulls out and highlights the AI comments with specific context, showing the LLM exactly how they fit into the code base.

    The "AI" comments below marked with █ can be found in the code files I've shared with you.
    They contain your instructions.
    Make the requested changes.
    Be sure to remove all these "AI" comments from the code!
    
    todo_app.py:
    ⋮...
    │class TodoList:
    ⋮...
    │    def __init__(self):
    │        """Initialize an empty todo list"""
    ⋮...
    │
    │    def list_tasks(self):
    │        """Display all tasks"""
    █        # Implement this. AI!
    │
    │def main():
    │    todo = TodoList()
    │
    ⋮...
    

* * *

#### [](#credits)Credits

_This feature was inspired by the way [Override](https://github.com/oi-overide) watches for file changes to find prompts embedded within `//> a specific set of delimiters <//`._

---



## [https://aider.chat/docs/usage/browser.html](https://aider.chat/docs/usage/browser.html)

[](#aider-in-your-browser)Aider in your browser
===============================================

 [Aider browser UI demo video](/assets/aider-browser-social.mp4)

Use aider’s new experimental browser UI to collaborate with LLMs to edit code in your local git repo. Aider will directly edit the code in your local source files, and [git commit the changes](https://aider.chat/docs/git.html) with sensible commit messages. You can start a new project or work with an existing git repo. Aider works well with GPT 3.5, GPT-4, GPT-4 Turbo with Vision, and Claude 3 Opus. It also supports [connecting to almost any LLM](https://aider.chat/docs/llms.html).

Use the `--browser` switch to launch the browser version of aider:

    python -m pip install -U aider-chat
    
    export OPENAI_API_KEY=<key> # Mac/Linux
    setx   OPENAI_API_KEY <key> # Windows, restart shell after setx
    
    aider --browser

---



## [https://aider.chat/docs/usage/conventions.html](https://aider.chat/docs/usage/conventions.html)

[](#specifying-coding-conventions)Specifying coding conventions
===============================================================

Sometimes you want GPT to be aware of certain coding guidelines, like whether to provide type hints, which libraries or packages to prefer, etc.

The easiest way to do that with aider is to simply create a small markdown file and include it in the chat.

For example, say we want our python code to:

    - Prefer httpx over requests for making http requests.
    - Use types everywhere possible.
    

We would simply create a file like `CONVENTIONS.md` with those lines and then we can add it to the aider chat, along with the file(s) that we want to edit.

It’s best to load the conventions file with `/read CONVENTIONS.md` or `aider --read CONVENTIONS.md`. This way it is marked as read-only, and cached if prompt caching is enabled.

[](#community-contributed-conventions)Community contributed conventions
-----------------------------------------------------------------------

You can check the [aider conventions repository](https://github.com/Aider-AI/conventions) to find or contribute conventions files.

[](#always-load-conventions)Always load conventions
---------------------------------------------------

You can also configure aider to always load your conventions file in the [`.aider.conf.yml` config file](https://aider.chat/docs/config/aider_conf.html):

    # alone
    read: CONVENTIONS.md
    
    # multiple files
    read: [CONVENTIONS.md, anotherfile.txt]
    

[](#example)Example
-------------------

See below for an example of how the conventions can affect the code that aider writes.

> $ aider –read CONVENTIONS.md useragent.py
> 
> Aider v0.24.2-dev  
> Added CONVENTIONS.md to the chat.  
> Added useragent.py to the chat.

#### [](#write-a-function-that-uses-httpbin-to-check-the-user-agent-on-the-request-return-the-ua)write a function that uses httpbin to check the user agent on the request. return the ua.

To fulfill your request, I will:

1.  Add an import for `httpx`.
2.  Write a function named `check_user_agent` that makes a GET request to `httpbin.org/user-agent` and returns the user agent string.

Here is the diff for the `useragent.py` file:

    --- useragent.py
    +++ useragent.py
    @@ ... @@
    +import httpx
    +
    +def check_user_agent() -> str:
    +    response = httpx.get('https://httpbin.org/user-agent')
    +    return response.json()['user-agent']
    

This function uses `httpx` to make a GET request to `httpbin.org/user-agent`, which returns a JSON response containing the user agent of the HTTP client. The function then extracts the user agent string from the JSON response and returns it.

> Applied edit to useragent.py

GPT correctly used `httpx` and provided type hints. See below for the transcript of this same coding task conducted _without_ using `CONVENTIONS.md`. In this case, GPT used `requests` and skipped types, which is perhaps more typical in small python scripts.

> $ aider useragent.py
> 
> Aider v0.24.2-dev  
> Added useragent.py to the chat.

#### [](#write-a-function-that-uses-httpbin-to-check-the-user-agent-on-the-request-return-the-ua-1)write a function that uses httpbin to check the user agent on the request. return the ua.

    --- /dev/null
    +++ useragent.py
    @@ ... @@
    +import requests
    +
    +def check_user_agent():
    +    response = requests.get('https://httpbin.org/user-agent')
    +    user_agent = response.json().get('user-agent')
    +    return user_agent
    

> Applied edit to useragent.py

---



## [https://aider.chat/docs/usage/copypaste.html](https://aider.chat/docs/usage/copypaste.html)

[](#copypaste-with-web-chat)Copy/paste with web chat
====================================================

 [Aider browser UI demo video](/assets/copypaste.mp4)

[](#working-with-an-llm-web-chat)Working with an LLM web chat
-------------------------------------------------------------

[Aider can connect to most LLMs via API](https://aider.chat/docs/llms.html) and works best that way. But there are times when you may want to work with an LLM via its web chat interface:

*   Workplace policies may limit your LLM usage to a proprietary web chat system.
*   The web chat LLM may have access to unique context or may have been specially fine tuned for your task.
*   It may be cost prohibitive to use some models via API.
*   There may not be an API available.

Aider has features for working with an LLM via its web chat interface. This allows you to use the web chat LLM as the “big brain code architect” while running aider with a smaller, cheaper LLM to actually make changes to your local files.

For this “file editor” part of the process you can run aider with many open source, free or very inexpensive LLMs. For example, the demo video above shows aider using DeepSeek to apply the changes that o1-preview is suggesting in the web chat.

### [](#copy-aiders-code-context-to-your-clipboard-paste-into-the-web-ui)Copy aider’s code context to your clipboard, paste into the web UI

The `/copy-context <instructions>` command can be used in chat to copy aider’s code context to your clipboard. It will include:

*   All the files which have been added to the chat via `/add`.
*   Any read only files which have been added via `/read`.
*   Aider’s [repository map](https://aider.chat/docs/repomap.html) that brings in code context related to the above files from elsewhere in your git repo.
*   Some instructions to the LLM that ask it to output change instructions concisely.
*   If you include `<instructions>`, they will be copied too.

You can paste the context into your browser, and start interacting with the LLM web chat to ask for code changes.

### [](#paste-the-llms-reply-back-into-aider-to-edit-your-files)Paste the LLM’s reply back into aider to edit your files

Once the LLM has replied, you can use the “copy response” button in the web UI to copy the LLM’s response. Back in aider, you can run `/paste` and aider will edit your files to implement the changes suggested by the LLM.

You can use a cheap, efficient model like GPT-4o Mini, DeepSeek or Qwen to do these edits. This works best if you run aider with `--edit-format editor-diff` or `--edit-format editor-whole`.

### [](#copypaste-mode)Copy/paste mode

Aider has a `--copy-paste` mode that streamlines this entire process:

*   Whenever you `/add` or `/read` files, aider will automatically copy the entire, updated code context to your clipboard. You’ll see “Copied code context to clipboard” whenever this happens.
*   When you copy the LLM reply to your clipboard outside aider, aider will automatically notice and load it into the aider chat. Just press ENTER to send the message and aider will apply the LLMs changes to your local files.
*   Aider will automatically select the best edit format for this copy/paste functionality. Depending on the LLM you have aider use, it will be either `editor-whole` or `editor-diff`.

[](#terms-of-service)Terms of service
-------------------------------------

Be sure to review the Terms Of Service of any LLM web chat service you use with these features. These features are not intended to be used in violation of any service’s Terms Of Service (TOS).

Aider’s web chat features have been designed to be compliant with the terms of service of most LLM web chats.

There are 4 copy/paste steps involved when coding with an LLM web chat:

1.  Copy code and context from aider.
2.  Paste the code and context into the LLM web chat.
3.  Copy the reply from the LLM web chat.
4.  Paste the LLM reply into aider.

Most LLM web chat TOS prohibit automating steps (2) and (3) where code is copied from and pasted into the web chat. Aider’s `--copy-paste` mode leaves those as 100% manual steps for the user to complete. It simply streamlines steps (1) and (4) that are interactions with aider, and which should not be under the scope of an LLM web chat TOS.

If you are concerned that the automatic interactions with aider in steps (1) and (4) may be problematic with respect to your LLM web chat provider’s TOS, you can forego `--copy-paste` mode. Instead, manually use the `/copy-context` and `/paste` commands if that will keep you in compliance.

Again, do not use these features in violation of any service’s Terms Of Service.

---



## [https://aider.chat/docs/usage/lint-test.html](https://aider.chat/docs/usage/lint-test.html)

[](#linting-and-testing)Linting and testing
===========================================

Aider can automatically lint and test your code every time it makes changes. This helps identify and repair any problems introduced by the AI edits.

[](#linting)Linting
-------------------

Aider comes with built in linters for [most popular languages](/docs/languages.html) and will automatically lint code in these languages.

Or you can specify your favorite linter with the `--lint-cmd <cmd>` switch. The lint command should accept the filenames of the files to lint. If there are linting errors, aider expects the command to print them on stdout/stderr and return a non-zero exit code. This is how most linters normally operate.

By default, aider will lint any files which it edits. You can disable this with the `--no-auto-lint` switch.

[](#testing)Testing
-------------------

You can run tests with `/test <test-command>`. Aider will run the test command without any arguments. If there are test errors, aider expects the command to print them on stdout/stderr and return a non-zero exit code.

Aider will try and fix any errors if the command returns a non-zero exit code.

You can configure aider to run your test suite after each time the AI edits your code using the `--test-cmd <test-command>` and `--auto-test` switch.

[](#compiled-languages)Compiled languages
-----------------------------------------

If you want to have aider compile code after each edit, you can use the lint and test commands to achieve this.

*   You might want to recompile each file which was modified to check for compile errors. To do this, provide a `--lint-cmd` which both lints and compiles the file. You could create a small shell script for this.
*   You might want to rebuild the entire project after files are edited to check for build errors. To do this, provide a `--test-cmd` which both builds and tests the project. You could create a small shell script for this. Or you may be able to do something as simple as `--test-cmd "dotnet build && dotnet test"`.

[](#manually-running-code)Manually running code
-----------------------------------------------

You can use the `/run` command in the chat to run your code and optionally share the output with aider. This can be useful to share error messages or to show aider the code’s output before asking for changes or corrections.

> Aider v0.43.5-dev

#### [](#run-python-myscriptpy)/run python myscript.py

    Traceback (most recent call last):  
     File "myscript.py", line 22, in \<module\ 
       raise ValueError("something bad happened")  
    ValueError: something bad happened  
    

> Add the output to the chat? y

---



## [https://aider.chat/docs/usage/not-code.html](https://aider.chat/docs/usage/not-code.html)

[](#editing-config--text-files)Editing config & text files
==========================================================

Aider isn’t just for code, it can be very helpful when editing almost any text file. You can use aider to make changes to your shell & ssh settings, Dockerfiles or pretty much any configuration or documentation file.

Here are some practical examples of modifying common config/text files:

[](#shell-configuration)Shell Configuration
-------------------------------------------

$ aider .bashrc

Added .bashrc to the chat.

#### [](#add-an-alias-ll-that-lists-all-files-with-all-details-in-human-readable-format-and-update-path-to-include-uv-installed-tools)Add an alias ‘ll’ that lists all files, with all details in human readable format. And update PATH to include uv installed tools.

    + alias ll='ls -alh'
    + export PATH="$PATH:$HOME/.local/bin:$PATH"
    

[](#ssh-configurations)SSH Configurations
-----------------------------------------

$ aider ~/.ssh/config

Added config to the chat.

#### [](#create-a-host-entry-my-server-using-bastionexamplecom-as-jumphost)Create a Host entry ‘my-server’ using bastion.example.com as JumpHost

    + Host my-server
    +     HostName 192.168.1.100
    +     User deploy
    +     Port 2222
    +     IdentityFile ~/.ssh/deploy_key
    +     ProxyJump bastion.example.com
    

[](#docker-setup)Docker Setup
-----------------------------

$ aider Dockerfile docker-compose.yml

Added Dockerfile and docker-compose.yml to the chat.

#### [](#set-non-root-user-and-enable-healthchecks)Set non-root user and enable healthchecks

    + USER appuser
    + HEALTHCHECK --interval=30s --timeout=3s \
    +   CMD curl -f http://localhost:8000/health || exit 1
    

#### [](#expose-port-5432-and-add-volume-for-postgres-data)Expose port 5432 and add volume for postgres data

      services:
        postgres:
          image: postgres:15
    +     ports:
    +       - "5432:5432"
    +     volumes:
    +       - pgdata:/var/lib/postgresql/data
    

[](#git-configuration)Git Configuration
---------------------------------------

$ aider .gitconfig

Added .gitconfig to the chat.

#### [](#set-default-push-behavior-to-current-branch-and-enable-color-ui)Set default push behavior to current branch and enable color UI

    + [push]
    +     default = current
    + [color]
    +     ui = auto
    

[](#system-configuration)System Configuration
---------------------------------------------

$ aider /etc/hosts # May need sudo

Added hosts to the chat.

#### [](#block-tracking-domains-by-pointing-them-to-127001)Block tracking domains by pointing them to 127.0.0.1

    + 127.0.0.1   ads.example.com
    + 127.0.0.1   track.analytics.co
    

[](#editor-configs)Editor Configs
---------------------------------

$ aider .vimrc

Added .vimrc to the chat.

#### [](#enable-line-numbers-and-set-4-space-tabs-for-python)Enable line numbers and set 4-space tabs for Python

    + set number
    + autocmd FileType python set tabstop=4 shiftwidth=4 expandtab
    

[](#vscode-configuration)VSCode Configuration
---------------------------------------------

$ aider settings.json

Added settings.json to the chat.

#### [](#enable-auto-format-on-save-and-set-default-formatter)Enable auto-format on save and set default formatter

    + "editor.formatOnSave": true,
    + "editor.defaultFormatter": "esbenp.prettier-vscode"
    

[](#markdown-documentation)Markdown Documentation
-------------------------------------------------

$ aider README.md

Added README.md to the chat.

#### [](#add-installation-section-with-brew-and-pip-options)Add installation section with brew and pip options

    + ## Installation
    + ```
    + # Homebrew
    + brew install cool-app-10k
    + 
    + # PyPI
    + pipx install cool-app-10k
    + ```
    

[](#xml-configuration)XML Configuration
---------------------------------------

$ aider pom.xml

Added pom.xml to the chat.

#### [](#add-junit-5-dependency-with-test-scope)Add JUnit 5 dependency with test scope

    + <dependency>
    +     <groupId>org.junit.jupiter</groupId>
    +     <artifactId>junit-jupiter-api</artifactId>
    +     <version>5.9.2</version>
    +     <scope>test</scope>
    + </dependency>

---



## [https://aider.chat/docs/llms.html](https://aider.chat/docs/llms.html)

[](#aider-can-connect-to-most-llms)Aider can connect to most LLMs
=================================================================

[](https://aider.chat/assets/llms.jpg)

[](#best-models)Best models
---------------------------

Aider works best with these models, which are skilled at editing code:

*   [GPT-4o](/docs/llms/openai.html)
*   [Claude 3.5 Sonnet](/docs/llms/anthropic.html)
*   [Claude 3 Opus](/docs/llms/anthropic.html)
*   [DeepSeek Coder V2](/docs/llms/deepseek.html)

[](#free-models)Free models
---------------------------

Aider works with a number of **free** API providers:

*   Google’s [Gemini 1.5 Pro](/docs/llms/gemini.html) works with aider, with code editing capabilities similar to GPT-3.5.
*   You can use [Llama 3 70B on Groq](/docs/llms/groq.html) which is comparable to GPT-3.5 in code editing performance.
*   Cohere also offers free API access to their [Command-R+ model](/docs/llms/cohere.html), which works with aider as a _very basic_ coding assistant.

[](#local-models)Local models
-----------------------------

Aider can work also with local models, for example using [Ollama](/docs/llms/ollama.html). It can also access local models that provide an [Open AI compatible API](/docs/llms/openai-compat.html).

[](#use-a-capable-model)Use a capable model
-------------------------------------------

Check [Aider’s LLM leaderboards](https://aider.chat/docs/leaderboards/) to see which models work best with aider.

Be aware that aider may not work well with less capable models. If you see the model returning code, but aider isn’t able to edit your files and commit the changes… this is usually because the model isn’t capable of properly returning “code edits”. Models weaker than GPT 3.5 may have problems working well with aider.

* * *

Table of contents
-----------------

*   [OpenAI](/docs/llms/openai.html)
*   [Anthropic](/docs/llms/anthropic.html)
*   [Gemini](/docs/llms/gemini.html)
*   [GROQ](/docs/llms/groq.html)
*   [LM Studio](/docs/llms/lm-studio.html)
*   [xAI](/docs/llms/xai.html)
*   [Azure](/docs/llms/azure.html)
*   [Cohere](/docs/llms/cohere.html)
*   [DeepSeek](/docs/llms/deepseek.html)
*   [Ollama](/docs/llms/ollama.html)
*   [OpenAI compatible APIs](/docs/llms/openai-compat.html)
*   [OpenRouter](/docs/llms/openrouter.html)
*   [Vertex AI](/docs/llms/vertex.html)
*   [Amazon Bedrock](/docs/llms/bedrock.html)
*   [Other LLMs](/docs/llms/other.html)
*   [Model warnings](/docs/llms/warnings.html)

---



## [https://aider.chat/docs/llms/openai.html](https://aider.chat/docs/llms/openai.html)

[](#openai)OpenAI
=================

To work with OpenAI’s models, you need to provide your [OpenAI API key](https://help.openai.com/en/articles/4936850-where-do-i-find-my-secret-api-key) either in the `OPENAI_API_KEY` environment variable or via the `--openai-api-key` command line switch.

Aider has some built in shortcuts for the most popular OpenAI models and has been tested and benchmarked to work well with them:

    python -m pip install -U aider-chat
    
    export OPENAI_API_KEY=<key> # Mac/Linux
    setx   OPENAI_API_KEY <key> # Windows, restart shell after setx
    
    # Aider uses gpt-4o by default (or use --4o)
    aider
    
    # GPT-4o
    aider --4o
    
    # GPT-3.5 Turbo
    aider --35-turbo
    
    # o1-mini
    aider --model o1-mini
    
    # o1-preview
    aider --model o1-preview
    
    # List models available from OpenAI
    aider --list-models openai/
    

You can use `aider --model <model-name>` to use any other OpenAI model. For example, if you want to use a specific version of GPT-4 Turbo you could do `aider --model gpt-4-0125-preview`.

---



## [https://aider.chat/docs/llms/anthropic.html](https://aider.chat/docs/llms/anthropic.html)

[](#anthropic)Anthropic
=======================

To work with Anthropic’s models, you need to provide your [Anthropic API key](https://docs.anthropic.com/claude/reference/getting-started-with-the-api) either in the `ANTHROPIC_API_KEY` environment variable or via the `--anthropic-api-key` command line switch.

Aider has some built in shortcuts for the most popular Anthropic models and has been tested and benchmarked to work well with them:

    python -m pip install -U aider-chat
    
    export ANTHROPIC_API_KEY=<key> # Mac/Linux
    setx   ANTHROPIC_API_KEY <key> # Windows, restart shell after setx
    
    # Aider uses Claude 3.5 Sonnet by default (or use --sonnet)
    aider
    
    # Claude 3 Opus
    aider --opus
    
    # List models available from Anthropic
    aider --list-models anthropic/
    

Anthropic has very low rate limits. You can access all the Anthropic models via [OpenRouter](/docs/llms/openrouter.html) or [Google Vertex AI](/docs/llms/vertex.html) with more generous rate limits.

You can use `aider --model <model-name>` to use any other Anthropic model. For example, if you want to use a specific version of Opus you could do `aider --model claude-3-opus-20240229`.

---



## [https://aider.chat/docs/llms/gemini.html](https://aider.chat/docs/llms/gemini.html)

[](#gemini)Gemini
=================

You’ll need a [Gemini API key](https://aistudio.google.com/app/u/2/apikey).

    python -m pip install -U aider-chat
    
    # You may need to install google-generativeai
    pip install -U google-generativeai
    
    # Or with pipx...
    pipx inject aider-chat google-generativeai
    
    export GEMINI_API_KEY=<key> # Mac/Linux
    setx   GEMINI_API_KEY <key> # Windows, restart shell after setx
    
    aider --model gemini/gemini-1.5-pro-latest
    
    # List models available from Gemini
    aider --list-models gemini/

---



## [https://aider.chat/docs/llms/groq.html](https://aider.chat/docs/llms/groq.html)

[](#groq)GROQ
=============

Groq currently offers _free_ API access to the models they host. The Llama 3 70B model works well with aider and is comparable to GPT-3.5 in code editing performance. You’ll need a [Groq API key](https://console.groq.com/keys).

To use **Llama3 70B**:

    python -m pip install -U aider-chat
    
    export GROQ_API_KEY=<key> # Mac/Linux
    setx   GROQ_API_KEY <key> # Windows, restart shell after setx
    
    aider --model groq/llama3-70b-8192
    
    # List models available from Groq
    aider --list-models groq/

---



## [https://aider.chat/docs/llms/lm-studio.html](https://aider.chat/docs/llms/lm-studio.html)

[](#lm-studio)LM Studio
=======================

To use LM Studio:

    python -m pip install -U aider-chat
    
    export LM_STUDIO_API_KEY=<key> # Mac/Linux
    setx   LM_STUDIO_API_KEY <key> # Windows, restart shell after setx
    
    export LM_STUDIO_API_BASE=<url> # Mac/Linux
    setx   LM_STUDIO_API_BASE <url> # Windows, restart shell after setx
    
    aider --model lm_studio/<your-model-name>
    

See the [model warnings](warnings.html) section for information on warnings which will occur when working with models that aider is not familiar with.

---



## [https://aider.chat/docs/llms/xai.html](https://aider.chat/docs/llms/xai.html)

[](#xai)xAI
===========

You’ll need a [xAI API key](https://console.x.ai.).

To use xAI:

    python -m pip install -U aider-chat
    
    export XAI_API_KEY=<key> # Mac/Linux
    setx   XAI_API_KEY <key> # Windows, restart shell after setx
    
    aider --model xai/grok-beta
    
    # List models available from xAI
    aider --list-models xai/

---



## [https://aider.chat/docs/llms/azure.html](https://aider.chat/docs/llms/azure.html)

[](#azure)Azure
===============

Aider can connect to the OpenAI models on Azure.

    python -m pip install -U aider-chat
    
    # Mac/Linux:                                           
    export AZURE_API_KEY=<key>
    export AZURE_API_VERSION=2023-05-15
    export AZURE_API_BASE=https://myendpt.openai.azure.com
    
    # Windows
    setx AZURE_API_KEY <key>
    setx AZURE_API_VERSION 2023-05-15
    setx AZURE_API_BASE https://myendpt.openai.azure.com
    # ... restart your shell after setx commands
    
    aider --model azure/<your_deployment_name>
    
    # List models available from Azure
    aider --list-models azure/
    

Note that aider will also use environment variables like `AZURE_OPENAI_API_xxx`.

---



## [https://aider.chat/docs/llms/cohere.html](https://aider.chat/docs/llms/cohere.html)

[](#cohere)Cohere
=================

Cohere offers _free_ API access to their models. Their Command-R+ model works well with aider as a _very basic_ coding assistant. You’ll need a [Cohere API key](https://dashboard.cohere.com/welcome/login).

To use **Command-R+**:

    python -m pip install -U aider-chat
    
    export COHERE_API_KEY=<key> # Mac/Linux
    setx   COHERE_API_KEY <key> # Windows, restart shell after setx
    
    aider --model command-r-plus-08-2024
    
    # List models available from Cohere
    aider --list-models cohere_chat/

---



## [https://aider.chat/docs/llms/deepseek.html](https://aider.chat/docs/llms/deepseek.html)

[](#deepseek)DeepSeek
=====================

Aider can connect to the DeepSeek.com API. The DeepSeek Coder V2 model has a top score on aider’s code editing benchmark.

    python -m pip install -U aider-chat
    
    export DEEPSEEK_API_KEY=<key> # Mac/Linux
    setx   DEEPSEEK_API_KEY <key> # Windows, restart shell after setx
    
    # Use DeepSeek Coder V2
    aider --deepseek

---



## [https://aider.chat/docs/llms/ollama.html](https://aider.chat/docs/llms/ollama.html)

[](#ollama)Ollama
=================

Aider can connect to local Ollama models.

    # Pull the model
    ollama pull <model>
    
    # Start your ollama server
    ollama serve
    
    # In another terminal window...
    python -m pip install -U aider-chat
    
    export OLLAMA_API_BASE=http://127.0.0.1:11434 # Mac/Linux
    setx   OLLAMA_API_BASE http://127.0.0.1:11434 # Windows, restart shell after setx
    
    aider --model ollama_chat/<model>
    

Using `ollama_chat/` is recommended over `ollama/`.

See the [model warnings](warnings.html) section for information on warnings which will occur when working with models that aider is not familiar with.

[](#api-key)API Key
-------------------

If you are using an ollama that requires an API key you can set `OLLAMA_API_KEY`:

    export OLLAMA_API_KEY=<api-key> # Mac/Linux
    setx   OLLAMA_API_KEY <api-key> # Windows, restart shell after setx
    

[](#setting-the-context-window-size)Setting the context window size
-------------------------------------------------------------------

[Ollama uses a 2k context window by default](https://github.com/ollama/ollama/blob/main/docs/faq.md#how-can-i-specify-the-context-window-size), which is very small for working with aider.

Aider sets Ollama’s context window to 8k by default. If you would like a larger context window you can use a [`.aider.model.settings.yml` file](https://aider.chat/docs/config/adv-model-settings.html#model-settings) like this:

    - name: ollama/qwen2.5-coder:32b-instruct-fp16
      extra_params:
        num_ctx: 8192
    

Unlike most other LLM servers, Ollama does not throw an error if you submit a request that exceeds the context window. Instead, it just silently truncates the request by discarding the “oldest” messages in the chat to make it fit within the context window. So if your context window is too small, you won’t get an error. Aider will probably just fail to work well and experience a lot of [file editing problems](https://aider.chat/docs/troubleshooting/edit-errors.html).

---



## [https://aider.chat/docs/llms/openai-compat.html](https://aider.chat/docs/llms/openai-compat.html)

[](#openai-compatible-apis)OpenAI compatible APIs
=================================================

Aider can connect to any LLM which is accessible via an OpenAI compatible API endpoint.

    python -m pip install -U aider-chat
    
    # Mac/Linux:
    export OPENAI_API_BASE=<endpoint>
    export OPENAI_API_KEY=<key>
    
    # Windows:
    setx OPENAI_API_BASE <endpoint>
    setx OPENAI_API_KEY <key>
    # ... restart shell after setx commands
    
    # Prefix the model name with openai/
    aider --model openai/<model-name>
    

See the [model warnings](warnings.html) section for information on warnings which will occur when working with models that aider is not familiar with.

---



## [https://aider.chat/docs/llms/openrouter.html](https://aider.chat/docs/llms/openrouter.html)

[](#openrouter)OpenRouter
=========================

Aider can connect to [models provided by OpenRouter](https://openrouter.ai/models?o=top-weekly): You’ll need an [OpenRouter API key](https://openrouter.ai/keys).

    python -m pip install -U aider-chat
    
    export OPENROUTER_API_KEY=<key> # Mac/Linux
    setx   OPENROUTER_API_KEY <key> # Windows, restart shell after setx
    
    # Or any other open router model
    aider --model openrouter/<provider>/<model>
    
    # List models available from OpenRouter
    aider --list-models openrouter/
    

In particular, many aider users access Sonnet via OpenRouter:

    python -m pip install -U aider-chat
    
    export OPENROUTER_API_KEY=<key> # Mac/Linux
    setx   OPENROUTER_API_KEY <key> # Windows, restart shell after setx
    
    aider --model openrouter/anthropic/claude-3.5-sonnet
    

If you get errors, check your [OpenRouter privacy settings](https://openrouter.ai/settings/privacy). Be sure to “enable providers that may train on inputs” to allow use of all models.

---



## [https://aider.chat/docs/llms/vertex.html](https://aider.chat/docs/llms/vertex.html)

[](#vertex-ai)Vertex AI
=======================

Aider can connect to models provided by Google Vertex AI. You will need to install the [gcloud CLI](https://cloud.google.com/sdk/docs/install) and [login](https://cloud.google.com/sdk/docs/initializing) with a GCP account or service account with permission to use the Vertex AI API.

With your chosen login method, the gcloud CLI should automatically set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable which points to the credentials file.

To configure Aider to use the Vertex AI API, you need to set `VERTEXAI_PROJECT` (the GCP project ID) and `VERTEXAI_LOCATION` (the GCP region) [environment variables for Aider](/docs/config/dotenv.html).

Note that Claude on Vertex AI is only available in certain GCP regions, check [the model card](https://console.cloud.google.com/vertex-ai/publishers/anthropic/model-garden/claude-3-5-sonnet) for your model to see which regions are supported.

Example `.env` file:

    VERTEXAI_PROJECT=my-project
    VERTEXAI_LOCATION=us-east5
    

Then you can run aider with the `--model` command line switch, like this:

    aider --model vertex_ai/claude-3-5-sonnet@20240620
    

Or you can use the [yaml config](/docs/config/aider_conf.html) to set the model to any of the models supported by Vertex AI.

Example `.aider.conf.yml` file:

    model: vertex_ai/claude-3-5-sonnet@20240620

---



## [https://aider.chat/docs/llms/bedrock.html](https://aider.chat/docs/llms/bedrock.html)

[](#amazon-bedrock)Amazon Bedrock
=================================

Aider can connect to models provided by Amazon Bedrock. You will need to have an AWS account with access to the Bedrock service.

To configure Aider to use the Amazon Bedrock API, you need to set up your AWS credentials. This can be done using the AWS CLI or by setting environment variables.

[](#aws-cli-configuration)AWS CLI Configuration
-----------------------------------------------

If you haven’t already, install the [AWS CLI](https://aws.amazon.com/cli/) and configure it with your credentials:

    aws configure
    

This will prompt you to enter your AWS Access Key ID, Secret Access Key, and default region.

[](#environment-variables)Environment Variables
-----------------------------------------------

Alternatively, you can set the following environment variables:

    export AWS_REGION=your_preferred_region
    
    # For user authentication
    export AWS_ACCESS_KEY_ID=your_access_key
    export AWS_SECRET_ACCESS_KEY=your_secret_key
    
    # For profile authentication
    export AWS_PROFILE=your-profile
    

You can add these to your [.env file](/docs/config/dotenv.html).

[](#install-boto3)Install boto3
-------------------------------

The AWS Bedrock provider requires the `boto3` package in order to function correctly:

    pip install boto3
    

To use aider installed via `pipx` with AWS Bedrock, you must add the `boto3` dependency to aider’s virtual environment by running

    pipx inject aider-chat boto3
    

You must install `boto3` dependency to aider’s virtual environment installed via one-liner or uv by running

    uv tool run --from aider-chat pip install boto3
    

[](#running-aider-with-bedrock)Running Aider with Bedrock
---------------------------------------------------------

Once your AWS credentials are set up, you can run Aider with the `--model` command line switch, specifying the Bedrock model you want to use:

    aider --model bedrock/anthropic.claude-3-5-sonnet-20240620-v1:0
    

Sometimes it seems to help if you prefix the model name with “us.”:

    aider --model bedrock/us.anthropic.claude-3-5-sonnet-20240620-v1:0
    

[](#available-models)Available Models
-------------------------------------

To see some models available via Bedrock, run:

    aider --list-models bedrock/
    

Make sure you have access to these models in your AWS account before attempting to use them with Aider.

[](#more-info)More info
=======================

For more information on Amazon Bedrock and its models, refer to the [official AWS documentation](https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html).

Also, see the [litellm docs on Bedrock](https://litellm.vercel.app/docs/providers/bedrock).

---



## [https://aider.chat/docs/llms/other.html](https://aider.chat/docs/llms/other.html)

[](#other-llms)Other LLMs
=========================

Aider uses the [litellm](https://docs.litellm.ai/docs/providers) package to connect to hundreds of other models. You can use `aider --model <model-name>` to use any supported model.

To explore the list of supported models you can run `aider --list-models <model-name>` with a partial model name. If the supplied name is not an exact match for a known model, aider will return a list of possible matching models. For example:

    $ aider --list-models turbo
    
    Aider v0.29.3-dev
    Models which match "turbo":
    - gpt-4-turbo-preview (openai/gpt-4-turbo-preview)
    - gpt-4-turbo (openai/gpt-4-turbo)
    - gpt-4-turbo-2024-04-09 (openai/gpt-4-turbo-2024-04-09)
    - gpt-3.5-turbo (openai/gpt-3.5-turbo)
    - ...
    

See the [model warnings](warnings.html) section for information on warnings which will occur when working with models that aider is not familiar with.

[](#litellm)LiteLLM
-------------------

Aider uses the LiteLLM package to connect to LLM providers. The [LiteLLM provider docs](https://docs.litellm.ai/docs/providers) contain more detail on all the supported providers, their models and any required environment variables.

[](#other-api-key-variables)Other API key variables
---------------------------------------------------

Here are the API key environment variables that are supported by litellm. See their docs for more info.

*   ALEPHALPHA\_API\_KEY
*   ALEPH\_ALPHA\_API\_KEY
*   ANTHROPIC\_API\_KEY
*   ANYSCALE\_API\_KEY
*   AZURE\_AI\_API\_KEY
*   AZURE\_API\_KEY
*   AZURE\_OPENAI\_API\_KEY
*   BASETEN\_API\_KEY
*   CEREBRAS\_API\_KEY
*   CLARIFAI\_API\_KEY
*   CLOUDFLARE\_API\_KEY
*   CODESTRAL\_API\_KEY
*   COHERE\_API\_KEY
*   CO\_API\_KEY
*   DATABRICKS\_API\_KEY
*   DEEPINFRA\_API\_KEY
*   DEEPSEEK\_API\_KEY
*   FIREWORKSAI\_API\_KEY
*   FIREWORKS\_AI\_API\_KEY
*   FIREWORKS\_API\_KEY
*   GEMINI\_API\_KEY
*   GROQ\_API\_KEY
*   HUGGINGFACE\_API\_KEY
*   MARITALK\_API\_KEY
*   MISTRAL\_API\_KEY
*   NLP\_CLOUD\_API\_KEY
*   NVIDIA\_NIM\_API\_KEY
*   OLLAMA\_API\_KEY
*   OPENAI\_API\_KEY
*   OPENAI\_LIKE\_API\_KEY
*   OPENROUTER\_API\_KEY
*   OR\_API\_KEY
*   PALM\_API\_KEY
*   PERPLEXITYAI\_API\_KEY
*   PREDIBASE\_API\_KEY
*   PROVIDER\_API\_KEY
*   REPLICATE\_API\_KEY
*   TOGETHERAI\_API\_KEY
*   VOLCENGINE\_API\_KEY
*   VOYAGE\_API\_KEY
*   WATSONX\_API\_KEY
*   WX\_API\_KEY
*   XAI\_API\_KEY
*   XINFERENCE\_API\_KEY

---



## [https://aider.chat/docs/llms/warnings.html](https://aider.chat/docs/llms/warnings.html)

[](#model-warnings)Model warnings
=================================

[](#unknown-context-window-size-and-token-costs)Unknown context window size and token costs
-------------------------------------------------------------------------------------------

    Model foobar: Unknown context window size and costs, using sane defaults.
    

If you specify a model that aider has never heard of, you will get this warning. This means aider doesn’t know the context window size and token costs for that model. Aider will use an unlimited context window and assume the model is free, so this is not usually a significant problem.

See the docs on [configuring advanced model settings](/docs/config/adv-model-settings.html) for details on how to remove this warning.

You can probably ignore the unknown context window size and token costs warning.

[](#did-you-mean)Did you mean?
------------------------------

If aider isn’t familiar with the model you’ve specified, it will suggest similarly named models. This helps in the case where you made a typo or mistake when specifying the model name.

    Model gpt-5o: Unknown context window size and costs, using sane defaults.
    Did you mean one of these?
    - gpt-4o
    

[](#missing-environment-variables)Missing environment variables
---------------------------------------------------------------

You need to set the listed environment variables. Otherwise you will get error messages when you start chatting with the model.

    Model azure/gpt-4-turbo: Missing these environment variables:
    - AZURE_API_BASE
    - AZURE_API_VERSION
    - AZURE_API_KEY
    

On Windows, if you just set these environment variables using `setx` you may need to restart your terminal or command prompt for the changes to take effect.

[](#unknown-which-environment-variables-are-required)Unknown which environment variables are required
-----------------------------------------------------------------------------------------------------

    Model gpt-5: Unknown which environment variables are required.
    

Aider is unable verify the environment because it doesn’t know which variables are required for the model. If required variables are missing, you may get errors when you attempt to chat with the model. You can look in the [aider’s LLM documentation](/docs/llms.html) or the [litellm documentation](https://docs.litellm.ai/docs/providers) to see if the required variables are listed there.

---



## [https://aider.chat/docs/config.html](https://aider.chat/docs/config.html)

[](#configuration)Configuration
===============================

Aider has many options which can be set with command line switches. Most options can also be set in an `.aider.conf.yml` file which can be placed in your home directory or at the root of your git repo. Or by setting environment variables like `AIDER_xxx` either in your shell or a `.env` file.

Here are 4 equivalent ways of setting an option.

With a command line switch:

    $ aider --dark-mode
    

Using a `.aider.conf.yml` file:

    dark-mode: true
    

By setting an environment variable:

    export AIDER_DARK_MODE=true
    

Using an `.env` file:

    AIDER_DARK_MODE=true
    

See the [API key configuration docs](/docs/config/api-keys.html) for information on how to configure and store your API keys.

* * *

Table of contents
-----------------

*   [API Keys](/docs/config/api-keys.html)
*   [Options reference](/docs/config/options.html)
*   [YAML config file](/docs/config/aider_conf.html)
*   [Config with .env](/docs/config/dotenv.html)
*   [Editor configuration](/docs/config/editor.html)
*   [Advanced model settings](/docs/config/adv-model-settings.html)
*   [Model Aliases](/docs/config/model-aliases.html)

---



## [https://aider.chat/docs/config/api-keys.html](https://aider.chat/docs/config/api-keys.html)

[](#api-keys)API Keys
=====================

Aider lets you specify API keys in a few ways:

*   On the command line
*   As environment variables
*   In a `.env` file
*   In your `.aider.conf.yml` config file

* * *

[](#openai-and-anthropic)OpenAI and Anthropic
---------------------------------------------

Aider has special support for providing OpenAI and Anthropic API keys via dedicated switches and configuration options. Settings keys for other providers works a bit differently, see below.

#### [](#command-line)Command line

You can set OpenAI and Anthropic API keys via [command line switches](/docs/config/options.html#api-keys-and-settings) `--openai-api-key` and `--anthropic-api-key`.

#### [](#environment-variables-or-env-file)Environment variables or .env file

You can also store them in environment variables or a [.env file](/docs/config/dotenv.html), which also works for every API provider:

    OPENAI_API_KEY=<key>
    ANTHROPIC_API_KEY=<key>
    

#### [](#yaml-config-file)Yaml config file

You can also set those API keys via special entries in the [yaml config file](/docs/config/aider_conf.html), like this:

    openai-api-key: <key>
    anthropic-api-key: <key>
    

* * *

[](#other-api-providers)Other API providers
-------------------------------------------

All other LLM providers can use one of these other methods to set their API keys.

#### [](#command-line-1)Command line

Use `--api-key provider=<key>` which has the effect of setting the environment variable `PROVIDER_API_KEY=<key>`. So `--api-key gemini=xxx` would set `GEMINI_API_KEY=xxx`.

#### [](#environment-variables-or-env-file-1)Environment variables or .env file

You can set API keys in environment variables. The [.env file](/docs/config/dotenv.html) is a great place to store your API keys and other provider API environment variables:

    GEMINI_API_KEY=foo
    OPENROUTER_API_KEY=bar
    DEEPSEEK_API_KEY=baz
    

#### [](#yaml-config-file-1)Yaml config file

You can also set API keys in the [`.aider.conf.yml` file](/docs/config/aider_conf.html) via the `api-key` entry:

    api-key:
    - gemini=foo      # Sets env var GEMINI_API_KEY=foo
    - openrouter=bar  # Sets env var OPENROUTER_API_KEY=bar
    - deepseek=baz    # Sets env var DEEPSEEK_API_KEY=baz

---



## [https://aider.chat/docs/config/options.html](https://aider.chat/docs/config/options.html)

[](#options-reference)Options reference
=======================================

You can use `aider --help` to see all the available options, or review them below.

*   [Usage summary](#usage-summary)
*   [options:](#options)
    *   [`--help`](#--help)
*   [Main model:](#main-model)
    *   [`--model MODEL`](#--model-model)
    *   [`--opus`](#--opus)
    *   [`--sonnet`](#--sonnet)
    *   [`--haiku`](#--haiku)
    *   [`--4`](#--4)
    *   [`--4o`](#--4o)
    *   [`--mini`](#--mini)
    *   [`--4-turbo`](#--4-turbo)
    *   [`--35turbo`](#--35turbo)
    *   [`--deepseek`](#--deepseek)
    *   [`--o1-mini`](#--o1-mini)
    *   [`--o1-preview`](#--o1-preview)
*   [API Keys and settings:](#api-keys-and-settings)
    *   [`--openai-api-key VALUE`](#--openai-api-key-value)
    *   [`--anthropic-api-key VALUE`](#--anthropic-api-key-value)
    *   [`--openai-api-base VALUE`](#--openai-api-base-value)
    *   [`--openai-api-type VALUE`](#--openai-api-type-value)
    *   [`--openai-api-version VALUE`](#--openai-api-version-value)
    *   [`--openai-api-deployment-id VALUE`](#--openai-api-deployment-id-value)
    *   [`--openai-organization-id VALUE`](#--openai-organization-id-value)
    *   [`--set-env ENV_VAR_NAME=value`](#--set-env-env_var_namevalue)
    *   [`--api-key PROVIDER=KEY`](#--api-key-providerkey)
*   [Model settings:](#model-settings)
    *   [`--list-models MODEL`](#--list-models-model)
    *   [`--model-settings-file MODEL_SETTINGS_FILE`](#--model-settings-file-model_settings_file)
    *   [`--model-metadata-file MODEL_METADATA_FILE`](#--model-metadata-file-model_metadata_file)
    *   [`--alias ALIAS:MODEL`](#--alias-aliasmodel)
    *   [`--verify-ssl`](#--verify-ssl)
    *   [`--timeout VALUE`](#--timeout-value)
    *   [`--edit-format EDIT_FORMAT`](#--edit-format-edit_format)
    *   [`--architect`](#--architect)
    *   [`--weak-model WEAK_MODEL`](#--weak-model-weak_model)
    *   [`--editor-model EDITOR_MODEL`](#--editor-model-editor_model)
    *   [`--editor-edit-format EDITOR_EDIT_FORMAT`](#--editor-edit-format-editor_edit_format)
    *   [`--show-model-warnings`](#--show-model-warnings)
    *   [`--max-chat-history-tokens VALUE`](#--max-chat-history-tokens-value)
*   [Cache settings:](#cache-settings)
    *   [`--cache-prompts`](#--cache-prompts)
    *   [`--cache-keepalive-pings VALUE`](#--cache-keepalive-pings-value)
*   [Repomap settings:](#repomap-settings)
    *   [`--map-tokens VALUE`](#--map-tokens-value)
    *   [`--map-refresh VALUE`](#--map-refresh-value)
    *   [`--map-multiplier-no-files VALUE`](#--map-multiplier-no-files-value)
*   [History Files:](#history-files)
    *   [`--input-history-file INPUT_HISTORY_FILE`](#--input-history-file-input_history_file)
    *   [`--chat-history-file CHAT_HISTORY_FILE`](#--chat-history-file-chat_history_file)
    *   [`--restore-chat-history`](#--restore-chat-history)
    *   [`--llm-history-file LLM_HISTORY_FILE`](#--llm-history-file-llm_history_file)
*   [Output settings:](#output-settings)
    *   [`--dark-mode`](#--dark-mode)
    *   [`--light-mode`](#--light-mode)
    *   [`--pretty`](#--pretty)
    *   [`--stream`](#--stream)
    *   [`--user-input-color VALUE`](#--user-input-color-value)
    *   [`--tool-output-color VALUE`](#--tool-output-color-value)
    *   [`--tool-error-color VALUE`](#--tool-error-color-value)
    *   [`--tool-warning-color VALUE`](#--tool-warning-color-value)
    *   [`--assistant-output-color VALUE`](#--assistant-output-color-value)
    *   [`--completion-menu-color COLOR`](#--completion-menu-color-color)
    *   [`--completion-menu-bg-color COLOR`](#--completion-menu-bg-color-color)
    *   [`--completion-menu-current-color COLOR`](#--completion-menu-current-color-color)
    *   [`--completion-menu-current-bg-color COLOR`](#--completion-menu-current-bg-color-color)
    *   [`--code-theme VALUE`](#--code-theme-value)
    *   [`--show-diffs`](#--show-diffs)
*   [Git settings:](#git-settings)
    *   [`--git`](#--git)
    *   [`--gitignore`](#--gitignore)
    *   [`--aiderignore AIDERIGNORE`](#--aiderignore-aiderignore)
    *   [`--subtree-only`](#--subtree-only)
    *   [`--auto-commits`](#--auto-commits)
    *   [`--dirty-commits`](#--dirty-commits)
    *   [`--attribute-author`](#--attribute-author)
    *   [`--attribute-committer`](#--attribute-committer)
    *   [`--attribute-commit-message-author`](#--attribute-commit-message-author)
    *   [`--attribute-commit-message-committer`](#--attribute-commit-message-committer)
    *   [`--commit`](#--commit)
    *   [`--commit-prompt PROMPT`](#--commit-prompt-prompt)
    *   [`--dry-run`](#--dry-run)
    *   [`--skip-sanity-check-repo`](#--skip-sanity-check-repo)
    *   [`--watch-files`](#--watch-files)
*   [Fixing and committing:](#fixing-and-committing)
    *   [`--lint`](#--lint)
    *   [`--lint-cmd`](#--lint-cmd)
    *   [`--auto-lint`](#--auto-lint)
    *   [`--test-cmd VALUE`](#--test-cmd-value)
    *   [`--auto-test`](#--auto-test)
    *   [`--test`](#--test)
*   [Analytics:](#analytics)
    *   [`--analytics`](#--analytics)
    *   [`--analytics-log ANALYTICS_LOG_FILE`](#--analytics-log-analytics_log_file)
    *   [`--analytics-disable`](#--analytics-disable)
*   [Upgrading:](#upgrading)
    *   [`--just-check-update`](#--just-check-update)
    *   [`--check-update`](#--check-update)
    *   [`--show-release-notes`](#--show-release-notes)
    *   [`--install-main-branch`](#--install-main-branch)
    *   [`--upgrade`](#--upgrade)
    *   [`--version`](#--version)
*   [Modes:](#modes)
    *   [`--message COMMAND`](#--message-command)
    *   [`--message-file MESSAGE_FILE`](#--message-file-message_file)
    *   [`--gui`](#--gui)
    *   [`--copy-paste`](#--copy-paste)
    *   [`--apply FILE`](#--apply-file)
    *   [`--apply-clipboard-edits`](#--apply-clipboard-edits)
    *   [`--exit`](#--exit)
    *   [`--show-repo-map`](#--show-repo-map)
    *   [`--show-prompts`](#--show-prompts)
*   [Voice settings:](#voice-settings)
    *   [`--voice-format VOICE_FORMAT`](#--voice-format-voice_format)
    *   [`--voice-language VOICE_LANGUAGE`](#--voice-language-voice_language)
    *   [`--voice-input-device VOICE_INPUT_DEVICE`](#--voice-input-device-voice_input_device)
*   [Other settings:](#other-settings)
    *   [`--file FILE`](#--file-file)
    *   [`--read FILE`](#--read-file)
    *   [`--vim`](#--vim)
    *   [`--chat-language CHAT_LANGUAGE`](#--chat-language-chat_language)
    *   [`--yes-always`](#--yes-always)
    *   [`--verbose`](#--verbose)
    *   [`--load LOAD_FILE`](#--load-load_file)
    *   [`--encoding VALUE`](#--encoding-value)
    *   [`--line-endings VALUE`](#--line-endings-value)
    *   [`--config CONFIG_FILE`](#--config-config_file)
    *   [`--env-file ENV_FILE`](#--env-file-env_file)
    *   [`--suggest-shell-commands`](#--suggest-shell-commands)
    *   [`--fancy-input`](#--fancy-input)
    *   [`--multiline`](#--multiline)
    *   [`--detect-urls`](#--detect-urls)
    *   [`--editor VALUE`](#--editor-value)

See the [API key configuration docs](/docs/config/api-keys.html) for information on how to configure and store your API keys.

[](#usage-summary)Usage summary
-------------------------------

    usage: aider [-h] [--model] [--opus] [--sonnet] [--haiku] [--4]
                 [--4o] [--mini] [--4-turbo] [--35turbo] [--deepseek]
                 [--o1-mini] [--o1-preview] [--openai-api-key]
                 [--anthropic-api-key] [--openai-api-base]
                 [--openai-api-type] [--openai-api-version]
                 [--openai-api-deployment-id] [--openai-organization-id]
                 [--set-env] [--api-key] [--list-models]
                 [--model-settings-file] [--model-metadata-file]
                 [--alias] [--verify-ssl | --no-verify-ssl] [--timeout]
                 [--edit-format] [--architect] [--weak-model]
                 [--editor-model] [--editor-edit-format]
                 [--show-model-warnings | --no-show-model-warnings]
                 [--max-chat-history-tokens]
                 [--cache-prompts | --no-cache-prompts]
                 [--cache-keepalive-pings] [--map-tokens]
                 [--map-refresh] [--map-multiplier-no-files]
                 [--input-history-file] [--chat-history-file]
                 [--restore-chat-history | --no-restore-chat-history]
                 [--llm-history-file] [--dark-mode] [--light-mode]
                 [--pretty | --no-pretty] [--stream | --no-stream]
                 [--user-input-color] [--tool-output-color]
                 [--tool-error-color] [--tool-warning-color]
                 [--assistant-output-color] [--completion-menu-color]
                 [--completion-menu-bg-color]
                 [--completion-menu-current-color]
                 [--completion-menu-current-bg-color] [--code-theme]
                 [--show-diffs] [--git | --no-git]
                 [--gitignore | --no-gitignore] [--aiderignore]
                 [--subtree-only] [--auto-commits | --no-auto-commits]
                 [--dirty-commits | --no-dirty-commits]
                 [--attribute-author | --no-attribute-author]
                 [--attribute-committer | --no-attribute-committer]
                 [--attribute-commit-message-author | --no-attribute-commit-message-author]
                 [--attribute-commit-message-committer | --no-attribute-commit-message-committer]
                 [--commit] [--commit-prompt] [--dry-run | --no-dry-run]
                 [--skip-sanity-check-repo]
                 [--watch-files | --no-watch-files] [--lint]
                 [--lint-cmd] [--auto-lint | --no-auto-lint]
                 [--test-cmd] [--auto-test | --no-auto-test] [--test]
                 [--analytics | --no-analytics] [--analytics-log]
                 [--analytics-disable] [--just-check-update]
                 [--check-update | --no-check-update]
                 [--show-release-notes | --no-show-release-notes]
                 [--install-main-branch] [--upgrade] [--version]
                 [--message] [--message-file]
                 [--gui | --no-gui | --browser | --no-browser]
                 [--copy-paste | --no-copy-paste] [--apply]
                 [--apply-clipboard-edits] [--exit] [--show-repo-map]
                 [--show-prompts] [--voice-format] [--voice-language]
                 [--voice-input-device] [--file] [--read] [--vim]
                 [--chat-language] [--yes-always] [-v] [--load]
                 [--encoding] [--line-endings] [-c] [--env-file]
                 [--suggest-shell-commands | --no-suggest-shell-commands]
                 [--fancy-input | --no-fancy-input]
                 [--multiline | --no-multiline]
                 [--detect-urls | --no-detect-urls] [--editor]
    
    

[](#options)options:
--------------------

### [](#--help)`--help`

show this help message and exit  
Aliases:

*   `-h`
*   `--help`

[](#main-model)Main model:
--------------------------

### [](#--model-model)`--model MODEL`

Specify the model to use for the main chat  
Environment variable: `AIDER_MODEL`

### [](#--opus)`--opus`

Use claude-3-opus-20240229 model for the main chat  
Environment variable: `AIDER_OPUS`

### [](#--sonnet)`--sonnet`

Use claude-3-5-sonnet-20241022 model for the main chat  
Environment variable: `AIDER_SONNET`

### [](#--haiku)`--haiku`

Use claude-3-5-haiku-20241022 model for the main chat  
Environment variable: `AIDER_HAIKU`

### [](#--4)`--4`

Use gpt-4-0613 model for the main chat  
Environment variable: `AIDER_4`  
Aliases:

*   `--4`
*   `-4`

### [](#--4o)`--4o`

Use gpt-4o model for the main chat  
Environment variable: `AIDER_4O`

### [](#--mini)`--mini`

Use gpt-4o-mini model for the main chat  
Environment variable: `AIDER_MINI`

### [](#--4-turbo)`--4-turbo`

Use gpt-4-1106-preview model for the main chat  
Environment variable: `AIDER_4_TURBO`

### [](#--35turbo)`--35turbo`

Use gpt-3.5-turbo model for the main chat  
Environment variable: `AIDER_35TURBO`  
Aliases:

*   `--35turbo`
*   `--35-turbo`
*   `--3`
*   `-3`

### [](#--deepseek)`--deepseek`

Use deepseek/deepseek-chat model for the main chat  
Environment variable: `AIDER_DEEPSEEK`

### [](#--o1-mini)`--o1-mini`

Use o1-mini model for the main chat  
Environment variable: `AIDER_O1_MINI`

### [](#--o1-preview)`--o1-preview`

Use o1-preview model for the main chat  
Environment variable: `AIDER_O1_PREVIEW`

[](#api-keys-and-settings)API Keys and settings:
------------------------------------------------

### [](#--openai-api-key-value)`--openai-api-key VALUE`

Specify the OpenAI API key  
Environment variable: `AIDER_OPENAI_API_KEY`

### [](#--anthropic-api-key-value)`--anthropic-api-key VALUE`

Specify the Anthropic API key  
Environment variable: `AIDER_ANTHROPIC_API_KEY`

### [](#--openai-api-base-value)`--openai-api-base VALUE`

Specify the api base url  
Environment variable: `AIDER_OPENAI_API_BASE`

### [](#--openai-api-type-value)`--openai-api-type VALUE`

(deprecated, use –set-env OPENAI\_API\_TYPE=) Environment variable: \`AIDER\_OPENAI\_API\_TYPE\`

### [](#--openai-api-version-value)`--openai-api-version VALUE`

(deprecated, use –set-env OPENAI\_API\_VERSION=) Environment variable: \`AIDER\_OPENAI\_API\_VERSION\`

### [](#--openai-api-deployment-id-value)`--openai-api-deployment-id VALUE`

(deprecated, use –set-env OPENAI\_API\_DEPLOYMENT\_ID=) Environment variable: \`AIDER\_OPENAI\_API\_DEPLOYMENT\_ID\`

### [](#--openai-organization-id-value)`--openai-organization-id VALUE`

(deprecated, use –set-env OPENAI\_ORGANIZATION=) Environment variable: \`AIDER\_OPENAI\_ORGANIZATION\_ID\`

### [](#--set-env-env_var_namevalue)`--set-env ENV_VAR_NAME=value`

Set an environment variable (to control API settings, can be used multiple times)  
Default: \[\]  
Environment variable: `AIDER_SET_ENV`

### [](#--api-key-providerkey)`--api-key PROVIDER=KEY`

Set an API key for a provider (eg: –api-key provider= sets PROVIDER\_API\_KEY=) Default: \[\] Environment variable: \`AIDER\_API\_KEY\`

[](#model-settings)Model settings:
----------------------------------

### [](#--list-models-model)`--list-models MODEL`

List known models which match the (partial) MODEL name  
Environment variable: `AIDER_LIST_MODELS`  
Aliases:

*   `--list-models MODEL`
*   `--models MODEL`

### [](#--model-settings-file-model_settings_file)`--model-settings-file MODEL_SETTINGS_FILE`

Specify a file with aider model settings for unknown models  
Default: .aider.model.settings.yml  
Environment variable: `AIDER_MODEL_SETTINGS_FILE`

### [](#--model-metadata-file-model_metadata_file)`--model-metadata-file MODEL_METADATA_FILE`

Specify a file with context window and costs for unknown models  
Default: .aider.model.metadata.json  
Environment variable: `AIDER_MODEL_METADATA_FILE`

### [](#--alias-aliasmodel)`--alias ALIAS:MODEL`

Add a model alias (can be used multiple times)  
Environment variable: `AIDER_ALIAS`

### [](#--verify-ssl)`--verify-ssl`

Verify the SSL cert when connecting to models (default: True)  
Default: True  
Environment variable: `AIDER_VERIFY_SSL`  
Aliases:

*   `--verify-ssl`
*   `--no-verify-ssl`

### [](#--timeout-value)`--timeout VALUE`

Timeout in seconds for API calls (default: None)  
Environment variable: `AIDER_TIMEOUT`

### [](#--edit-format-edit_format)`--edit-format EDIT_FORMAT`

Specify what edit format the LLM should use (default depends on model)  
Environment variable: `AIDER_EDIT_FORMAT`  
Aliases:

*   `--edit-format EDIT_FORMAT`
*   `--chat-mode EDIT_FORMAT`

### [](#--architect)`--architect`

Use architect edit format for the main chat  
Environment variable: `AIDER_ARCHITECT`

### [](#--weak-model-weak_model)`--weak-model WEAK_MODEL`

Specify the model to use for commit messages and chat history summarization (default depends on –model)  
Environment variable: `AIDER_WEAK_MODEL`

### [](#--editor-model-editor_model)`--editor-model EDITOR_MODEL`

Specify the model to use for editor tasks (default depends on –model)  
Environment variable: `AIDER_EDITOR_MODEL`

### [](#--editor-edit-format-editor_edit_format)`--editor-edit-format EDITOR_EDIT_FORMAT`

Specify the edit format for the editor model (default: depends on editor model)  
Environment variable: `AIDER_EDITOR_EDIT_FORMAT`

### [](#--show-model-warnings)`--show-model-warnings`

Only work with models that have meta-data available (default: True)  
Default: True  
Environment variable: `AIDER_SHOW_MODEL_WARNINGS`  
Aliases:

*   `--show-model-warnings`
*   `--no-show-model-warnings`

### [](#--max-chat-history-tokens-value)`--max-chat-history-tokens VALUE`

Soft limit on tokens for chat history, after which summarization begins. If unspecified, defaults to the model’s max\_chat\_history\_tokens.  
Environment variable: `AIDER_MAX_CHAT_HISTORY_TOKENS`

[](#cache-settings)Cache settings:
----------------------------------

### [](#--cache-prompts)`--cache-prompts`

Enable caching of prompts (default: False)  
Default: False  
Environment variable: `AIDER_CACHE_PROMPTS`  
Aliases:

*   `--cache-prompts`
*   `--no-cache-prompts`

### [](#--cache-keepalive-pings-value)`--cache-keepalive-pings VALUE`

Number of times to ping at 5min intervals to keep prompt cache warm (default: 0)  
Default: 0  
Environment variable: `AIDER_CACHE_KEEPALIVE_PINGS`

[](#repomap-settings)Repomap settings:
--------------------------------------

### [](#--map-tokens-value)`--map-tokens VALUE`

Suggested number of tokens to use for repo map, use 0 to disable  
Environment variable: `AIDER_MAP_TOKENS`

### [](#--map-refresh-value)`--map-refresh VALUE`

Control how often the repo map is refreshed. Options: auto, always, files, manual (default: auto)  
Default: auto  
Environment variable: `AIDER_MAP_REFRESH`

### [](#--map-multiplier-no-files-value)`--map-multiplier-no-files VALUE`

Multiplier for map tokens when no files are specified (default: 2)  
Default: 2  
Environment variable: `AIDER_MAP_MULTIPLIER_NO_FILES`

[](#history-files)History Files:
--------------------------------

### [](#--input-history-file-input_history_file)`--input-history-file INPUT_HISTORY_FILE`

Specify the chat input history file (default: .aider.input.history)  
Default: .aider.input.history  
Environment variable: `AIDER_INPUT_HISTORY_FILE`

### [](#--chat-history-file-chat_history_file)`--chat-history-file CHAT_HISTORY_FILE`

Specify the chat history file (default: .aider.chat.history.md)  
Default: .aider.chat.history.md  
Environment variable: `AIDER_CHAT_HISTORY_FILE`

### [](#--restore-chat-history)`--restore-chat-history`

Restore the previous chat history messages (default: False)  
Default: False  
Environment variable: `AIDER_RESTORE_CHAT_HISTORY`  
Aliases:

*   `--restore-chat-history`
*   `--no-restore-chat-history`

### [](#--llm-history-file-llm_history_file)`--llm-history-file LLM_HISTORY_FILE`

Log the conversation with the LLM to this file (for example, .aider.llm.history)  
Environment variable: `AIDER_LLM_HISTORY_FILE`

[](#output-settings)Output settings:
------------------------------------

### [](#--dark-mode)`--dark-mode`

Use colors suitable for a dark terminal background (default: False)  
Default: False  
Environment variable: `AIDER_DARK_MODE`

### [](#--light-mode)`--light-mode`

Use colors suitable for a light terminal background (default: False)  
Default: False  
Environment variable: `AIDER_LIGHT_MODE`

### [](#--pretty)`--pretty`

Enable/disable pretty, colorized output (default: True)  
Default: True  
Environment variable: `AIDER_PRETTY`  
Aliases:

*   `--pretty`
*   `--no-pretty`

### [](#--stream)`--stream`

Enable/disable streaming responses (default: True)  
Default: True  
Environment variable: `AIDER_STREAM`  
Aliases:

*   `--stream`
*   `--no-stream`

### [](#--user-input-color-value)`--user-input-color VALUE`

Set the color for user input (default: #00cc00)  
Default: #00cc00  
Environment variable: `AIDER_USER_INPUT_COLOR`

### [](#--tool-output-color-value)`--tool-output-color VALUE`

Set the color for tool output (default: None)  
Environment variable: `AIDER_TOOL_OUTPUT_COLOR`

### [](#--tool-error-color-value)`--tool-error-color VALUE`

Set the color for tool error messages (default: #FF2222)  
Default: #FF2222  
Environment variable: `AIDER_TOOL_ERROR_COLOR`

### [](#--tool-warning-color-value)`--tool-warning-color VALUE`

Set the color for tool warning messages (default: #FFA500)  
Default: #FFA500  
Environment variable: `AIDER_TOOL_WARNING_COLOR`

### [](#--assistant-output-color-value)`--assistant-output-color VALUE`

Set the color for assistant output (default: #0088ff)  
Default: #0088ff  
Environment variable: `AIDER_ASSISTANT_OUTPUT_COLOR`

### [](#--completion-menu-color-color)`--completion-menu-color COLOR`

Set the color for the completion menu (default: terminal’s default text color)  
Environment variable: `AIDER_COMPLETION_MENU_COLOR`

### [](#--completion-menu-bg-color-color)`--completion-menu-bg-color COLOR`

Set the background color for the completion menu (default: terminal’s default background color)  
Environment variable: `AIDER_COMPLETION_MENU_BG_COLOR`

### [](#--completion-menu-current-color-color)`--completion-menu-current-color COLOR`

Set the color for the current item in the completion menu (default: terminal’s default background color)  
Environment variable: `AIDER_COMPLETION_MENU_CURRENT_COLOR`

### [](#--completion-menu-current-bg-color-color)`--completion-menu-current-bg-color COLOR`

Set the background color for the current item in the completion menu (default: terminal’s default text color)  
Environment variable: `AIDER_COMPLETION_MENU_CURRENT_BG_COLOR`

### [](#--code-theme-value)`--code-theme VALUE`

Set the markdown code theme (default: default, other options include monokai, solarized-dark, solarized-light, or a Pygments builtin style, see https://pygments.org/styles for available themes)  
Default: default  
Environment variable: `AIDER_CODE_THEME`

### [](#--show-diffs)`--show-diffs`

Show diffs when committing changes (default: False)  
Default: False  
Environment variable: `AIDER_SHOW_DIFFS`

[](#git-settings)Git settings:
------------------------------

### [](#--git)`--git`

Enable/disable looking for a git repo (default: True)  
Default: True  
Environment variable: `AIDER_GIT`  
Aliases:

*   `--git`
*   `--no-git`

### [](#--gitignore)`--gitignore`

Enable/disable adding .aider\* to .gitignore (default: True)  
Default: True  
Environment variable: `AIDER_GITIGNORE`  
Aliases:

*   `--gitignore`
*   `--no-gitignore`

### [](#--aiderignore-aiderignore)`--aiderignore AIDERIGNORE`

Specify the aider ignore file (default: .aiderignore in git root)  
Default: .aiderignore  
Environment variable: `AIDER_AIDERIGNORE`

### [](#--subtree-only)`--subtree-only`

Only consider files in the current subtree of the git repository  
Default: False  
Environment variable: `AIDER_SUBTREE_ONLY`

### [](#--auto-commits)`--auto-commits`

Enable/disable auto commit of LLM changes (default: True)  
Default: True  
Environment variable: `AIDER_AUTO_COMMITS`  
Aliases:

*   `--auto-commits`
*   `--no-auto-commits`

### [](#--dirty-commits)`--dirty-commits`

Enable/disable commits when repo is found dirty (default: True)  
Default: True  
Environment variable: `AIDER_DIRTY_COMMITS`  
Aliases:

*   `--dirty-commits`
*   `--no-dirty-commits`

### [](#--attribute-author)`--attribute-author`

Attribute aider code changes in the git author name (default: True)  
Default: True  
Environment variable: `AIDER_ATTRIBUTE_AUTHOR`  
Aliases:

*   `--attribute-author`
*   `--no-attribute-author`

### [](#--attribute-committer)`--attribute-committer`

Attribute aider commits in the git committer name (default: True)  
Default: True  
Environment variable: `AIDER_ATTRIBUTE_COMMITTER`  
Aliases:

*   `--attribute-committer`
*   `--no-attribute-committer`

### [](#--attribute-commit-message-author)`--attribute-commit-message-author`

Prefix commit messages with ‘aider: ‘ if aider authored the changes (default: False)  
Default: False  
Environment variable: `AIDER_ATTRIBUTE_COMMIT_MESSAGE_AUTHOR`  
Aliases:

*   `--attribute-commit-message-author`
*   `--no-attribute-commit-message-author`

### [](#--attribute-commit-message-committer)`--attribute-commit-message-committer`

Prefix all commit messages with ‘aider: ‘ (default: False)  
Default: False  
Environment variable: `AIDER_ATTRIBUTE_COMMIT_MESSAGE_COMMITTER`  
Aliases:

*   `--attribute-commit-message-committer`
*   `--no-attribute-commit-message-committer`

### [](#--commit)`--commit`

Commit all pending changes with a suitable commit message, then exit  
Default: False  
Environment variable: `AIDER_COMMIT`

### [](#--commit-prompt-prompt)`--commit-prompt PROMPT`

Specify a custom prompt for generating commit messages  
Environment variable: `AIDER_COMMIT_PROMPT`

### [](#--dry-run)`--dry-run`

Perform a dry run without modifying files (default: False)  
Default: False  
Environment variable: `AIDER_DRY_RUN`  
Aliases:

*   `--dry-run`
*   `--no-dry-run`

### [](#--skip-sanity-check-repo)`--skip-sanity-check-repo`

Skip the sanity check for the git repository (default: False)  
Default: False  
Environment variable: `AIDER_SKIP_SANITY_CHECK_REPO`

### [](#--watch-files)`--watch-files`

Enable/disable watching files for ai coding comments (default: False)  
Default: False  
Environment variable: `AIDER_WATCH_FILES`  
Aliases:

*   `--watch-files`
*   `--no-watch-files`

[](#fixing-and-committing)Fixing and committing:
------------------------------------------------

### [](#--lint)`--lint`

Lint and fix provided files, or dirty files if none provided  
Default: False  
Environment variable: `AIDER_LINT`

### [](#--lint-cmd)`--lint-cmd`

Specify lint commands to run for different languages, eg: “python: flake8 –select=…” (can be used multiple times)  
Default: \[\]  
Environment variable: `AIDER_LINT_CMD`

### [](#--auto-lint)`--auto-lint`

Enable/disable automatic linting after changes (default: True)  
Default: True  
Environment variable: `AIDER_AUTO_LINT`  
Aliases:

*   `--auto-lint`
*   `--no-auto-lint`

### [](#--test-cmd-value)`--test-cmd VALUE`

Specify command to run tests  
Default: \[\]  
Environment variable: `AIDER_TEST_CMD`

### [](#--auto-test)`--auto-test`

Enable/disable automatic testing after changes (default: False)  
Default: False  
Environment variable: `AIDER_AUTO_TEST`  
Aliases:

*   `--auto-test`
*   `--no-auto-test`

### [](#--test)`--test`

Run tests, fix problems found and then exit  
Default: False  
Environment variable: `AIDER_TEST`

[](#analytics)Analytics:
------------------------

### [](#--analytics)`--analytics`

Enable/disable analytics for current session (default: random)  
Environment variable: `AIDER_ANALYTICS`  
Aliases:

*   `--analytics`
*   `--no-analytics`

### [](#--analytics-log-analytics_log_file)`--analytics-log ANALYTICS_LOG_FILE`

Specify a file to log analytics events  
Environment variable: `AIDER_ANALYTICS_LOG`

### [](#--analytics-disable)`--analytics-disable`

Permanently disable analytics  
Default: False  
Environment variable: `AIDER_ANALYTICS_DISABLE`

[](#upgrading)Upgrading:
------------------------

### [](#--just-check-update)`--just-check-update`

Check for updates and return status in the exit code  
Default: False  
Environment variable: `AIDER_JUST_CHECK_UPDATE`

### [](#--check-update)`--check-update`

Check for new aider versions on launch  
Default: True  
Environment variable: `AIDER_CHECK_UPDATE`  
Aliases:

*   `--check-update`
*   `--no-check-update`

### [](#--show-release-notes)`--show-release-notes`

Show release notes on first run of new version (default: None, ask user)  
Environment variable: `AIDER_SHOW_RELEASE_NOTES`  
Aliases:

*   `--show-release-notes`
*   `--no-show-release-notes`

### [](#--install-main-branch)`--install-main-branch`

Install the latest version from the main branch  
Default: False  
Environment variable: `AIDER_INSTALL_MAIN_BRANCH`

### [](#--upgrade)`--upgrade`

Upgrade aider to the latest version from PyPI  
Default: False  
Environment variable: `AIDER_UPGRADE`  
Aliases:

*   `--upgrade`
*   `--update`

### [](#--version)`--version`

Show the version number and exit

[](#modes)Modes:
----------------

### [](#--message-command)`--message COMMAND`

Specify a single message to send the LLM, process reply then exit (disables chat mode)  
Environment variable: `AIDER_MESSAGE`  
Aliases:

*   `--message COMMAND`
*   `--msg COMMAND`
*   `-m COMMAND`

### [](#--message-file-message_file)`--message-file MESSAGE_FILE`

Specify a file containing the message to send the LLM, process reply, then exit (disables chat mode)  
Environment variable: `AIDER_MESSAGE_FILE`  
Aliases:

*   `--message-file MESSAGE_FILE`
*   `-f MESSAGE_FILE`

### [](#--gui)`--gui`

Run aider in your browser (default: False)  
Default: False  
Environment variable: `AIDER_GUI`  
Aliases:

*   `--gui`
*   `--no-gui`
*   `--browser`
*   `--no-browser`

### [](#--copy-paste)`--copy-paste`

Enable automatic copy/paste of chat between aider and web UI (default: False)  
Default: False  
Environment variable: `AIDER_COPY_PASTE`  
Aliases:

*   `--copy-paste`
*   `--no-copy-paste`

### [](#--apply-file)`--apply FILE`

Apply the changes from the given file instead of running the chat (debug)  
Environment variable: `AIDER_APPLY`

### [](#--apply-clipboard-edits)`--apply-clipboard-edits`

Apply clipboard contents as edits using the main model’s editor format  
Default: False  
Environment variable: `AIDER_APPLY_CLIPBOARD_EDITS`

### [](#--exit)`--exit`

Do all startup activities then exit before accepting user input (debug)  
Default: False  
Environment variable: `AIDER_EXIT`

### [](#--show-repo-map)`--show-repo-map`

Print the repo map and exit (debug)  
Default: False  
Environment variable: `AIDER_SHOW_REPO_MAP`

### [](#--show-prompts)`--show-prompts`

Print the system prompts and exit (debug)  
Default: False  
Environment variable: `AIDER_SHOW_PROMPTS`

[](#voice-settings)Voice settings:
----------------------------------

### [](#--voice-format-voice_format)`--voice-format VOICE_FORMAT`

Audio format for voice recording (default: wav). webm and mp3 require ffmpeg  
Default: wav  
Environment variable: `AIDER_VOICE_FORMAT`

### [](#--voice-language-voice_language)`--voice-language VOICE_LANGUAGE`

Specify the language for voice using ISO 639-1 code (default: auto)  
Default: en  
Environment variable: `AIDER_VOICE_LANGUAGE`

### [](#--voice-input-device-voice_input_device)`--voice-input-device VOICE_INPUT_DEVICE`

Specify the input device name for voice recording  
Environment variable: `AIDER_VOICE_INPUT_DEVICE`

[](#other-settings)Other settings:
----------------------------------

### [](#--file-file)`--file FILE`

specify a file to edit (can be used multiple times)  
Environment variable: `AIDER_FILE`

### [](#--read-file)`--read FILE`

specify a read-only file (can be used multiple times)  
Environment variable: `AIDER_READ`

### [](#--vim)`--vim`

Use VI editing mode in the terminal (default: False)  
Default: False  
Environment variable: `AIDER_VIM`

### [](#--chat-language-chat_language)`--chat-language CHAT_LANGUAGE`

Specify the language to use in the chat (default: None, uses system settings)  
Environment variable: `AIDER_CHAT_LANGUAGE`

### [](#--yes-always)`--yes-always`

Always say yes to every confirmation  
Environment variable: `AIDER_YES_ALWAYS`

### [](#--verbose)`--verbose`

Enable verbose output  
Default: False  
Environment variable: `AIDER_VERBOSE`  
Aliases:

*   `-v`
*   `--verbose`

### [](#--load-load_file)`--load LOAD_FILE`

Load and execute /commands from a file on launch  
Environment variable: `AIDER_LOAD`

### [](#--encoding-value)`--encoding VALUE`

Specify the encoding for input and output (default: utf-8)  
Default: utf-8  
Environment variable: `AIDER_ENCODING`

### [](#--line-endings-value)`--line-endings VALUE`

Line endings to use when writing files (default: platform)  
Default: platform  
Environment variable: `AIDER_LINE_ENDINGS`

### [](#--config-config_file)`--config CONFIG_FILE`

Specify the config file (default: search for .aider.conf.yml in git root, cwd or home directory)  
Aliases:

*   `-c CONFIG_FILE`
*   `--config CONFIG_FILE`

### [](#--env-file-env_file)`--env-file ENV_FILE`

Specify the .env file to load (default: .env in git root)  
Default: .env  
Environment variable: `AIDER_ENV_FILE`

### [](#--suggest-shell-commands)`--suggest-shell-commands`

Enable/disable suggesting shell commands (default: True)  
Default: True  
Environment variable: `AIDER_SUGGEST_SHELL_COMMANDS`  
Aliases:

*   `--suggest-shell-commands`
*   `--no-suggest-shell-commands`

### [](#--fancy-input)`--fancy-input`

Enable/disable fancy input with history and completion (default: True)  
Default: True  
Environment variable: `AIDER_FANCY_INPUT`  
Aliases:

*   `--fancy-input`
*   `--no-fancy-input`

### [](#--multiline)`--multiline`

Enable/disable multi-line input mode with Meta-Enter to submit (default: False)  
Default: False  
Environment variable: `AIDER_MULTILINE`  
Aliases:

*   `--multiline`
*   `--no-multiline`

### [](#--detect-urls)`--detect-urls`

Enable/disable detection and offering to add URLs to chat (default: True)  
Default: True  
Environment variable: `AIDER_DETECT_URLS`  
Aliases:

*   `--detect-urls`
*   `--no-detect-urls`

### [](#--editor-value)`--editor VALUE`

Specify which editor to use for the /editor command  
Environment variable: `AIDER_EDITOR`

---



## [https://aider.chat/docs/config/aider_conf.html](https://aider.chat/docs/config/aider_conf.html)

[](#yaml-config-file)YAML config file
=====================================

Most of aider’s options can be set in an `.aider.conf.yml` file. Aider will look for a this file in these locations:

*   Your home directory.
*   The root of your git repo.
*   The current directory.

If the files above exist, they will be loaded in that order. Files loaded last will take priority.

You can also specify the `--config <filename>` parameter, which will only load the one config file.

See the [API key configuration docs](/docs/config/api-keys.html) for information on how to configure and store your API keys.

[](#a-note-on-lists)A note on lists
-----------------------------------

Lists of values can be specified either as a bulleted list:

    read:
      - CONVENTIONS.md
      - anotherfile.txt
      - thirdfile.py
    

Or lists can be specified using commas and square brackets:

    read: [CONVENTIONS.md, anotherfile.txt, thirdfile.py]
    

[](#sample-yaml-config-file)Sample YAML config file
---------------------------------------------------

Below is a sample of the YAML config file, which you can also [download from GitHub](https://github.com/Aider-AI/aider/blob/main/aider/website/assets/sample.aider.conf.yml).

    ##########################################################
    # Sample .aider.conf.yml
    # This file lists *all* the valid configuration entries.
    # Place in your home dir, or at the root of your git repo.
    ##########################################################
    
    # Note: You can only put OpenAI and Anthropic API keys in the yaml
    # config file. Keys for all APIs can be stored in a .env file
    # https://aider.chat/docs/config/dotenv.html
    
    ##########
    # options:
    
    ## show this help message and exit
    #help: xxx
    
    #############
    # Main model:
    
    ## Specify the model to use for the main chat
    #model: xxx
    
    ## Use claude-3-opus-20240229 model for the main chat
    #opus: false
    
    ## Use claude-3-5-sonnet-20241022 model for the main chat
    #sonnet: false
    
    ## Use claude-3-5-haiku-20241022 model for the main chat
    #haiku: false
    
    ## Use gpt-4-0613 model for the main chat
    #4: false
    
    ## Use gpt-4o model for the main chat
    #4o: false
    
    ## Use gpt-4o-mini model for the main chat
    #mini: false
    
    ## Use gpt-4-1106-preview model for the main chat
    #4-turbo: false
    
    ## Use gpt-3.5-turbo model for the main chat
    #35turbo: false
    
    ## Use deepseek/deepseek-chat model for the main chat
    #deepseek: false
    
    ## Use o1-mini model for the main chat
    #o1-mini: false
    
    ## Use o1-preview model for the main chat
    #o1-preview: false
    
    ########################
    # API Keys and settings:
    
    ## Specify the OpenAI API key
    #openai-api-key: xxx
    
    ## Specify the Anthropic API key
    #anthropic-api-key: xxx
    
    ## Specify the api base url
    #openai-api-base: xxx
    
    ## (deprecated, use --set-env OPENAI_API_TYPE=<value>)
    #openai-api-type: xxx
    
    ## (deprecated, use --set-env OPENAI_API_VERSION=<value>)
    #openai-api-version: xxx
    
    ## (deprecated, use --set-env OPENAI_API_DEPLOYMENT_ID=<value>)
    #openai-api-deployment-id: xxx
    
    ## (deprecated, use --set-env OPENAI_ORGANIZATION=<value>)
    #openai-organization-id: xxx
    
    ## Set an environment variable (to control API settings, can be used multiple times)
    #set-env: xxx
    ## Specify multiple values like this:
    #set-env:
    #  - xxx
    #  - yyy
    #  - zzz
    
    ## Set an API key for a provider (eg: --api-key provider=<key> sets PROVIDER_API_KEY=<key>)
    #api-key: xxx
    ## Specify multiple values like this:
    #api-key:
    #  - xxx
    #  - yyy
    #  - zzz
    
    #################
    # Model settings:
    
    ## List known models which match the (partial) MODEL name
    #list-models: xxx
    
    ## Specify a file with aider model settings for unknown models
    #model-settings-file: .aider.model.settings.yml
    
    ## Specify a file with context window and costs for unknown models
    #model-metadata-file: .aider.model.metadata.json
    
    ## Add a model alias (can be used multiple times)
    #alias: xxx
    ## Specify multiple values like this:
    #alias:
    #  - xxx
    #  - yyy
    #  - zzz
    
    ## Verify the SSL cert when connecting to models (default: True)
    #verify-ssl: true
    
    ## Timeout in seconds for API calls (default: None)
    #timeout: xxx
    
    ## Specify what edit format the LLM should use (default depends on model)
    #edit-format: xxx
    
    ## Use architect edit format for the main chat
    #architect: false
    
    ## Specify the model to use for commit messages and chat history summarization (default depends on --model)
    #weak-model: xxx
    
    ## Specify the model to use for editor tasks (default depends on --model)
    #editor-model: xxx
    
    ## Specify the edit format for the editor model (default: depends on editor model)
    #editor-edit-format: xxx
    
    ## Only work with models that have meta-data available (default: True)
    #show-model-warnings: true
    
    ## Soft limit on tokens for chat history, after which summarization begins. If unspecified, defaults to the model's max_chat_history_tokens.
    #max-chat-history-tokens: xxx
    
    #################
    # Cache settings:
    
    ## Enable caching of prompts (default: False)
    #cache-prompts: false
    
    ## Number of times to ping at 5min intervals to keep prompt cache warm (default: 0)
    #cache-keepalive-pings: false
    
    ###################
    # Repomap settings:
    
    ## Suggested number of tokens to use for repo map, use 0 to disable
    #map-tokens: xxx
    
    ## Control how often the repo map is refreshed. Options: auto, always, files, manual (default: auto)
    #map-refresh: auto
    
    ## Multiplier for map tokens when no files are specified (default: 2)
    #map-multiplier-no-files: true
    
    ################
    # History Files:
    
    ## Specify the chat input history file (default: .aider.input.history)
    #input-history-file: .aider.input.history
    
    ## Specify the chat history file (default: .aider.chat.history.md)
    #chat-history-file: .aider.chat.history.md
    
    ## Restore the previous chat history messages (default: False)
    #restore-chat-history: false
    
    ## Log the conversation with the LLM to this file (for example, .aider.llm.history)
    #llm-history-file: xxx
    
    ##################
    # Output settings:
    
    ## Use colors suitable for a dark terminal background (default: False)
    #dark-mode: false
    
    ## Use colors suitable for a light terminal background (default: False)
    #light-mode: false
    
    ## Enable/disable pretty, colorized output (default: True)
    #pretty: true
    
    ## Enable/disable streaming responses (default: True)
    #stream: true
    
    ## Set the color for user input (default: #00cc00)
    #user-input-color: #00cc00
    
    ## Set the color for tool output (default: None)
    #tool-output-color: xxx
    
    ## Set the color for tool error messages (default: #FF2222)
    #tool-error-color: #FF2222
    
    ## Set the color for tool warning messages (default: #FFA500)
    #tool-warning-color: #FFA500
    
    ## Set the color for assistant output (default: #0088ff)
    #assistant-output-color: #0088ff
    
    ## Set the color for the completion menu (default: terminal's default text color)
    #completion-menu-color: xxx
    
    ## Set the background color for the completion menu (default: terminal's default background color)
    #completion-menu-bg-color: xxx
    
    ## Set the color for the current item in the completion menu (default: terminal's default background color)
    #completion-menu-current-color: xxx
    
    ## Set the background color for the current item in the completion menu (default: terminal's default text color)
    #completion-menu-current-bg-color: xxx
    
    ## Set the markdown code theme (default: default, other options include monokai, solarized-dark, solarized-light, or a Pygments builtin style, see https://pygments.org/styles for available themes)
    #code-theme: default
    
    ## Show diffs when committing changes (default: False)
    #show-diffs: false
    
    ###############
    # Git settings:
    
    ## Enable/disable looking for a git repo (default: True)
    #git: true
    
    ## Enable/disable adding .aider* to .gitignore (default: True)
    #gitignore: true
    
    ## Specify the aider ignore file (default: .aiderignore in git root)
    #aiderignore: .aiderignore
    
    ## Only consider files in the current subtree of the git repository
    #subtree-only: false
    
    ## Enable/disable auto commit of LLM changes (default: True)
    #auto-commits: true
    
    ## Enable/disable commits when repo is found dirty (default: True)
    #dirty-commits: true
    
    ## Attribute aider code changes in the git author name (default: True)
    #attribute-author: true
    
    ## Attribute aider commits in the git committer name (default: True)
    #attribute-committer: true
    
    ## Prefix commit messages with 'aider: ' if aider authored the changes (default: False)
    #attribute-commit-message-author: false
    
    ## Prefix all commit messages with 'aider: ' (default: False)
    #attribute-commit-message-committer: false
    
    ## Commit all pending changes with a suitable commit message, then exit
    #commit: false
    
    ## Specify a custom prompt for generating commit messages
    #commit-prompt: xxx
    
    ## Perform a dry run without modifying files (default: False)
    #dry-run: false
    
    ## Skip the sanity check for the git repository (default: False)
    #skip-sanity-check-repo: false
    
    ## Enable/disable watching files for ai coding comments (default: False)
    #watch-files: false
    
    ########################
    # Fixing and committing:
    
    ## Lint and fix provided files, or dirty files if none provided
    #lint: false
    
    ## Specify lint commands to run for different languages, eg: "python: flake8 --select=..." (can be used multiple times)
    #lint-cmd: xxx
    ## Specify multiple values like this:
    #lint-cmd:
    #  - xxx
    #  - yyy
    #  - zzz
    
    ## Enable/disable automatic linting after changes (default: True)
    #auto-lint: true
    
    ## Specify command to run tests
    #test-cmd: xxx
    
    ## Enable/disable automatic testing after changes (default: False)
    #auto-test: false
    
    ## Run tests, fix problems found and then exit
    #test: false
    
    ############
    # Analytics:
    
    ## Enable/disable analytics for current session (default: random)
    #analytics: xxx
    
    ## Specify a file to log analytics events
    #analytics-log: xxx
    
    ## Permanently disable analytics
    #analytics-disable: false
    
    ############
    # Upgrading:
    
    ## Check for updates and return status in the exit code
    #just-check-update: false
    
    ## Check for new aider versions on launch
    #check-update: true
    
    ## Show release notes on first run of new version (default: None, ask user)
    #show-release-notes: xxx
    
    ## Install the latest version from the main branch
    #install-main-branch: false
    
    ## Upgrade aider to the latest version from PyPI
    #upgrade: false
    
    ## Show the version number and exit
    #version: xxx
    
    ########
    # Modes:
    
    ## Specify a single message to send the LLM, process reply then exit (disables chat mode)
    #message: xxx
    
    ## Specify a file containing the message to send the LLM, process reply, then exit (disables chat mode)
    #message-file: xxx
    
    ## Run aider in your browser (default: False)
    #gui: false
    
    ## Enable automatic copy/paste of chat between aider and web UI (default: False)
    #copy-paste: false
    
    ## Apply the changes from the given file instead of running the chat (debug)
    #apply: xxx
    
    ## Apply clipboard contents as edits using the main model's editor format
    #apply-clipboard-edits: false
    
    ## Do all startup activities then exit before accepting user input (debug)
    #exit: false
    
    ## Print the repo map and exit (debug)
    #show-repo-map: false
    
    ## Print the system prompts and exit (debug)
    #show-prompts: false
    
    #################
    # Voice settings:
    
    ## Audio format for voice recording (default: wav). webm and mp3 require ffmpeg
    #voice-format: wav
    
    ## Specify the language for voice using ISO 639-1 code (default: auto)
    #voice-language: en
    
    ## Specify the input device name for voice recording
    #voice-input-device: xxx
    
    #################
    # Other settings:
    
    ## specify a file to edit (can be used multiple times)
    #file: xxx
    ## Specify multiple values like this:
    #file:
    #  - xxx
    #  - yyy
    #  - zzz
    
    ## specify a read-only file (can be used multiple times)
    #read: xxx
    ## Specify multiple values like this:
    #read:
    #  - xxx
    #  - yyy
    #  - zzz
    
    ## Use VI editing mode in the terminal (default: False)
    #vim: false
    
    ## Specify the language to use in the chat (default: None, uses system settings)
    #chat-language: xxx
    
    ## Always say yes to every confirmation
    #yes-always: false
    
    ## Enable verbose output
    #verbose: false
    
    ## Load and execute /commands from a file on launch
    #load: xxx
    
    ## Specify the encoding for input and output (default: utf-8)
    #encoding: utf-8
    
    ## Line endings to use when writing files (default: platform)
    #line-endings: platform
    
    ## Specify the config file (default: search for .aider.conf.yml in git root, cwd or home directory)
    #config: xxx
    
    ## Specify the .env file to load (default: .env in git root)
    #env-file: .env
    
    ## Enable/disable suggesting shell commands (default: True)
    #suggest-shell-commands: true
    
    ## Enable/disable fancy input with history and completion (default: True)
    #fancy-input: true
    
    ## Enable/disable multi-line input mode with Meta-Enter to submit (default: False)
    #multiline: false
    
    ## Enable/disable detection and offering to add URLs to chat (default: True)
    #detect-urls: true
    
    ## Specify which editor to use for the /editor command
    #editor: xxx

---



## [https://aider.chat/docs/config/dotenv.html](https://aider.chat/docs/config/dotenv.html)

[](#config-with-env)Config with .env
====================================

You can use a `.env` file to store API keys and other settings for the models you use with aider. You can also set many general aider options in the `.env` file.

Aider will look for a `.env` file in these locations:

*   Your home directory.
*   The root of your git repo.
*   The current directory.
*   As specified with the `--env-file <filename>` parameter.

If the files above exist, they will be loaded in that order. Files loaded last will take priority.

See the [API key configuration docs](/docs/config/api-keys.html) for information on how to configure and store your API keys.

[](#sample-env-file)Sample .env file
------------------------------------

Below is a sample `.env` file, which you can also [download from GitHub](https://github.com/Aider-AI/aider/blob/main/aider/website/assets/sample.env).

    ##########################################################
    # Sample aider .env file.
    # Place at the root of your git repo.
    # Or use `aider --env <fname>` to specify.
    ##########################################################
    
    #################
    # LLM parameters:
    #
    # Include xxx_API_KEY parameters and other params needed for your LLMs.
    # See https://aider.chat/docs/llms.html for details.
    
    ## OpenAI
    #OPENAI_API_KEY=
    
    ## Anthropic
    #ANTHROPIC_API_KEY=
    
    ##...
    
    #############
    # Main model:
    
    ## Specify the model to use for the main chat
    #AIDER_MODEL=
    
    ## Use claude-3-opus-20240229 model for the main chat
    #AIDER_OPUS=
    
    ## Use claude-3-5-sonnet-20241022 model for the main chat
    #AIDER_SONNET=
    
    ## Use claude-3-5-haiku-20241022 model for the main chat
    #AIDER_HAIKU=
    
    ## Use gpt-4-0613 model for the main chat
    #AIDER_4=
    
    ## Use gpt-4o model for the main chat
    #AIDER_4O=
    
    ## Use gpt-4o-mini model for the main chat
    #AIDER_MINI=
    
    ## Use gpt-4-1106-preview model for the main chat
    #AIDER_4_TURBO=
    
    ## Use gpt-3.5-turbo model for the main chat
    #AIDER_35TURBO=
    
    ## Use deepseek/deepseek-chat model for the main chat
    #AIDER_DEEPSEEK=
    
    ## Use o1-mini model for the main chat
    #AIDER_O1_MINI=
    
    ## Use o1-preview model for the main chat
    #AIDER_O1_PREVIEW=
    
    ########################
    # API Keys and settings:
    
    ## Specify the OpenAI API key
    #AIDER_OPENAI_API_KEY=
    
    ## Specify the Anthropic API key
    #AIDER_ANTHROPIC_API_KEY=
    
    ## Specify the api base url
    #AIDER_OPENAI_API_BASE=
    
    ## (deprecated, use --set-env OPENAI_API_TYPE=<value>)
    #AIDER_OPENAI_API_TYPE=
    
    ## (deprecated, use --set-env OPENAI_API_VERSION=<value>)
    #AIDER_OPENAI_API_VERSION=
    
    ## (deprecated, use --set-env OPENAI_API_DEPLOYMENT_ID=<value>)
    #AIDER_OPENAI_API_DEPLOYMENT_ID=
    
    ## (deprecated, use --set-env OPENAI_ORGANIZATION=<value>)
    #AIDER_OPENAI_ORGANIZATION_ID=
    
    ## Set an environment variable (to control API settings, can be used multiple times)
    #AIDER_SET_ENV=
    
    ## Set an API key for a provider (eg: --api-key provider=<key> sets PROVIDER_API_KEY=<key>)
    #AIDER_API_KEY=
    
    #################
    # Model settings:
    
    ## List known models which match the (partial) MODEL name
    #AIDER_LIST_MODELS=
    
    ## Specify a file with aider model settings for unknown models
    #AIDER_MODEL_SETTINGS_FILE=.aider.model.settings.yml
    
    ## Specify a file with context window and costs for unknown models
    #AIDER_MODEL_METADATA_FILE=.aider.model.metadata.json
    
    ## Add a model alias (can be used multiple times)
    #AIDER_ALIAS=
    
    ## Verify the SSL cert when connecting to models (default: True)
    #AIDER_VERIFY_SSL=true
    
    ## Timeout in seconds for API calls (default: None)
    #AIDER_TIMEOUT=
    
    ## Specify what edit format the LLM should use (default depends on model)
    #AIDER_EDIT_FORMAT=
    
    ## Use architect edit format for the main chat
    #AIDER_ARCHITECT=
    
    ## Specify the model to use for commit messages and chat history summarization (default depends on --model)
    #AIDER_WEAK_MODEL=
    
    ## Specify the model to use for editor tasks (default depends on --model)
    #AIDER_EDITOR_MODEL=
    
    ## Specify the edit format for the editor model (default: depends on editor model)
    #AIDER_EDITOR_EDIT_FORMAT=
    
    ## Only work with models that have meta-data available (default: True)
    #AIDER_SHOW_MODEL_WARNINGS=true
    
    ## Soft limit on tokens for chat history, after which summarization begins. If unspecified, defaults to the model's max_chat_history_tokens.
    #AIDER_MAX_CHAT_HISTORY_TOKENS=
    
    #################
    # Cache settings:
    
    ## Enable caching of prompts (default: False)
    #AIDER_CACHE_PROMPTS=false
    
    ## Number of times to ping at 5min intervals to keep prompt cache warm (default: 0)
    #AIDER_CACHE_KEEPALIVE_PINGS=false
    
    ###################
    # Repomap settings:
    
    ## Suggested number of tokens to use for repo map, use 0 to disable
    #AIDER_MAP_TOKENS=
    
    ## Control how often the repo map is refreshed. Options: auto, always, files, manual (default: auto)
    #AIDER_MAP_REFRESH=auto
    
    ## Multiplier for map tokens when no files are specified (default: 2)
    #AIDER_MAP_MULTIPLIER_NO_FILES=true
    
    ################
    # History Files:
    
    ## Specify the chat input history file (default: .aider.input.history)
    #AIDER_INPUT_HISTORY_FILE=.aider.input.history
    
    ## Specify the chat history file (default: .aider.chat.history.md)
    #AIDER_CHAT_HISTORY_FILE=.aider.chat.history.md
    
    ## Restore the previous chat history messages (default: False)
    #AIDER_RESTORE_CHAT_HISTORY=false
    
    ## Log the conversation with the LLM to this file (for example, .aider.llm.history)
    #AIDER_LLM_HISTORY_FILE=
    
    ##################
    # Output settings:
    
    ## Use colors suitable for a dark terminal background (default: False)
    #AIDER_DARK_MODE=false
    
    ## Use colors suitable for a light terminal background (default: False)
    #AIDER_LIGHT_MODE=false
    
    ## Enable/disable pretty, colorized output (default: True)
    #AIDER_PRETTY=true
    
    ## Enable/disable streaming responses (default: True)
    #AIDER_STREAM=true
    
    ## Set the color for user input (default: #00cc00)
    #AIDER_USER_INPUT_COLOR=#00cc00
    
    ## Set the color for tool output (default: None)
    #AIDER_TOOL_OUTPUT_COLOR=
    
    ## Set the color for tool error messages (default: #FF2222)
    #AIDER_TOOL_ERROR_COLOR=#FF2222
    
    ## Set the color for tool warning messages (default: #FFA500)
    #AIDER_TOOL_WARNING_COLOR=#FFA500
    
    ## Set the color for assistant output (default: #0088ff)
    #AIDER_ASSISTANT_OUTPUT_COLOR=#0088ff
    
    ## Set the color for the completion menu (default: terminal's default text color)
    #AIDER_COMPLETION_MENU_COLOR=
    
    ## Set the background color for the completion menu (default: terminal's default background color)
    #AIDER_COMPLETION_MENU_BG_COLOR=
    
    ## Set the color for the current item in the completion menu (default: terminal's default background color)
    #AIDER_COMPLETION_MENU_CURRENT_COLOR=
    
    ## Set the background color for the current item in the completion menu (default: terminal's default text color)
    #AIDER_COMPLETION_MENU_CURRENT_BG_COLOR=
    
    ## Set the markdown code theme (default: default, other options include monokai, solarized-dark, solarized-light, or a Pygments builtin style, see https://pygments.org/styles for available themes)
    #AIDER_CODE_THEME=default
    
    ## Show diffs when committing changes (default: False)
    #AIDER_SHOW_DIFFS=false
    
    ###############
    # Git settings:
    
    ## Enable/disable looking for a git repo (default: True)
    #AIDER_GIT=true
    
    ## Enable/disable adding .aider* to .gitignore (default: True)
    #AIDER_GITIGNORE=true
    
    ## Specify the aider ignore file (default: .aiderignore in git root)
    #AIDER_AIDERIGNORE=.aiderignore
    
    ## Only consider files in the current subtree of the git repository
    #AIDER_SUBTREE_ONLY=false
    
    ## Enable/disable auto commit of LLM changes (default: True)
    #AIDER_AUTO_COMMITS=true
    
    ## Enable/disable commits when repo is found dirty (default: True)
    #AIDER_DIRTY_COMMITS=true
    
    ## Attribute aider code changes in the git author name (default: True)
    #AIDER_ATTRIBUTE_AUTHOR=true
    
    ## Attribute aider commits in the git committer name (default: True)
    #AIDER_ATTRIBUTE_COMMITTER=true
    
    ## Prefix commit messages with 'aider: ' if aider authored the changes (default: False)
    #AIDER_ATTRIBUTE_COMMIT_MESSAGE_AUTHOR=false
    
    ## Prefix all commit messages with 'aider: ' (default: False)
    #AIDER_ATTRIBUTE_COMMIT_MESSAGE_COMMITTER=false
    
    ## Commit all pending changes with a suitable commit message, then exit
    #AIDER_COMMIT=false
    
    ## Specify a custom prompt for generating commit messages
    #AIDER_COMMIT_PROMPT=
    
    ## Perform a dry run without modifying files (default: False)
    #AIDER_DRY_RUN=false
    
    ## Skip the sanity check for the git repository (default: False)
    #AIDER_SKIP_SANITY_CHECK_REPO=false
    
    ## Enable/disable watching files for ai coding comments (default: False)
    #AIDER_WATCH_FILES=false
    
    ########################
    # Fixing and committing:
    
    ## Lint and fix provided files, or dirty files if none provided
    #AIDER_LINT=false
    
    ## Specify lint commands to run for different languages, eg: "python: flake8 --select=..." (can be used multiple times)
    #AIDER_LINT_CMD=
    
    ## Enable/disable automatic linting after changes (default: True)
    #AIDER_AUTO_LINT=true
    
    ## Specify command to run tests
    #AIDER_TEST_CMD=
    
    ## Enable/disable automatic testing after changes (default: False)
    #AIDER_AUTO_TEST=false
    
    ## Run tests, fix problems found and then exit
    #AIDER_TEST=false
    
    ############
    # Analytics:
    
    ## Enable/disable analytics for current session (default: random)
    #AIDER_ANALYTICS=
    
    ## Specify a file to log analytics events
    #AIDER_ANALYTICS_LOG=
    
    ## Permanently disable analytics
    #AIDER_ANALYTICS_DISABLE=false
    
    ############
    # Upgrading:
    
    ## Check for updates and return status in the exit code
    #AIDER_JUST_CHECK_UPDATE=false
    
    ## Check for new aider versions on launch
    #AIDER_CHECK_UPDATE=true
    
    ## Show release notes on first run of new version (default: None, ask user)
    #AIDER_SHOW_RELEASE_NOTES=
    
    ## Install the latest version from the main branch
    #AIDER_INSTALL_MAIN_BRANCH=false
    
    ## Upgrade aider to the latest version from PyPI
    #AIDER_UPGRADE=false
    
    ########
    # Modes:
    
    ## Specify a single message to send the LLM, process reply then exit (disables chat mode)
    #AIDER_MESSAGE=
    
    ## Specify a file containing the message to send the LLM, process reply, then exit (disables chat mode)
    #AIDER_MESSAGE_FILE=
    
    ## Run aider in your browser (default: False)
    #AIDER_GUI=false
    
    ## Enable automatic copy/paste of chat between aider and web UI (default: False)
    #AIDER_COPY_PASTE=false
    
    ## Apply the changes from the given file instead of running the chat (debug)
    #AIDER_APPLY=
    
    ## Apply clipboard contents as edits using the main model's editor format
    #AIDER_APPLY_CLIPBOARD_EDITS=false
    
    ## Do all startup activities then exit before accepting user input (debug)
    #AIDER_EXIT=false
    
    ## Print the repo map and exit (debug)
    #AIDER_SHOW_REPO_MAP=false
    
    ## Print the system prompts and exit (debug)
    #AIDER_SHOW_PROMPTS=false
    
    #################
    # Voice settings:
    
    ## Audio format for voice recording (default: wav). webm and mp3 require ffmpeg
    #AIDER_VOICE_FORMAT=wav
    
    ## Specify the language for voice using ISO 639-1 code (default: auto)
    #AIDER_VOICE_LANGUAGE=en
    
    ## Specify the input device name for voice recording
    #AIDER_VOICE_INPUT_DEVICE=
    
    #################
    # Other settings:
    
    ## specify a file to edit (can be used multiple times)
    #AIDER_FILE=
    
    ## specify a read-only file (can be used multiple times)
    #AIDER_READ=
    
    ## Use VI editing mode in the terminal (default: False)
    #AIDER_VIM=false
    
    ## Specify the language to use in the chat (default: None, uses system settings)
    #AIDER_CHAT_LANGUAGE=
    
    ## Always say yes to every confirmation
    #AIDER_YES_ALWAYS=
    
    ## Enable verbose output
    #AIDER_VERBOSE=false
    
    ## Load and execute /commands from a file on launch
    #AIDER_LOAD=
    
    ## Specify the encoding for input and output (default: utf-8)
    #AIDER_ENCODING=utf-8
    
    ## Line endings to use when writing files (default: platform)
    #AIDER_LINE_ENDINGS=platform
    
    ## Specify the .env file to load (default: .env in git root)
    #AIDER_ENV_FILE=.env
    
    ## Enable/disable suggesting shell commands (default: True)
    #AIDER_SUGGEST_SHELL_COMMANDS=true
    
    ## Enable/disable fancy input with history and completion (default: True)
    #AIDER_FANCY_INPUT=true
    
    ## Enable/disable multi-line input mode with Meta-Enter to submit (default: False)
    #AIDER_MULTILINE=false
    
    ## Enable/disable detection and offering to add URLs to chat (default: True)
    #AIDER_DETECT_URLS=true
    
    ## Specify which editor to use for the /editor command
    #AIDER_EDITOR=

---



## [https://aider.chat/docs/config/editor.html](https://aider.chat/docs/config/editor.html)

[](#editor-configuration)Editor configuration
=============================================

Aider allows you to configure your preferred text editor for use with the `/editor` command. The editor must be capable of running in “blocking mode”, meaning the command line will wait until you close the editor before proceeding.

[](#using---editor)Using `--editor`
-----------------------------------

You can specify the text editor with the `--editor` switch or using `editor:` in aider’s [yaml config file](https://aider.chat/docs/config/aider_conf.html).

[](#environment-variables)Environment variables
-----------------------------------------------

Aider checks the following environment variables in order to determine which editor to use:

1.  `AIDER_EDITOR`
2.  `VISUAL`
3.  `EDITOR`

[](#default-behavior)Default behavior
-------------------------------------

If no editor is configured, aider will use these platform-specific defaults:

*   Windows: `notepad`
*   macOS: `vim`
*   Linux/Unix: `vi`

[](#using-a-custom-editor)Using a custom editor
-----------------------------------------------

You can set your preferred editor in your shell’s configuration file (e.g., `.bashrc`, `.zshrc`):

    export AIDER_EDITOR=vim
    

[](#popular-editors-by-platform)Popular Editors by Platform
-----------------------------------------------------------

### [](#macos)macOS

1.  **vim**
    
        export AIDER_EDITOR=vim
        
    
2.  **Emacs**
    
        export AIDER_EDITOR=emacs
        
    
3.  **VSCode**
    
        export AIDER_EDITOR="code --wait"
        
    
4.  **Sublime Text**
    
        export AIDER_EDITOR="subl --wait"
        
    
5.  **BBEdit**
    
        export AIDER_EDITOR="bbedit --wait"
        
    

### [](#linux)Linux

1.  **vim**
    
        export AIDER_EDITOR=vim
        
    
2.  **Emacs**
    
        export AIDER_EDITOR=emacs
        
    
3.  **nano**
    
        export AIDER_EDITOR=nano
        
    
4.  **VSCode**
    
        export AIDER_EDITOR="code --wait"
        
    
5.  **Sublime Text**
    
        export AIDER_EDITOR="subl --wait"
        
    

### [](#windows)Windows

1.  **Notepad**
    
        set AIDER_EDITOR=notepad
        
    
2.  **VSCode**
    
        set AIDER_EDITOR="code --wait"
        
    
3.  **Notepad++**
    
        set AIDER_EDITOR="notepad++ -multiInst -notabbar -nosession -noPlugin -waitForClose"
        
    

[](#editor-command-arguments)Editor command arguments
-----------------------------------------------------

Some editors require specific command-line arguments to operate in blocking mode. The `--wait` flag (or equivalent) is commonly used to make the editor block until the file is closed.

[](#troubleshooting)Troubleshooting
-----------------------------------

If you encounter issues with your editor not blocking (returning to the prompt immediately), verify that:

1.  Your editor supports blocking mode
2.  You’ve included the necessary command-line arguments for blocking mode
3.  The editor command is properly quoted if it contains spaces or special characters, e.g.:
    
        export AIDER_EDITOR="code --wait"

---



## [https://aider.chat/docs/config/adv-model-settings.html](https://aider.chat/docs/config/adv-model-settings.html)

[](#advanced-model-settings)Advanced model settings
===================================================

[](#context-window-size-and-token-costs)Context window size and token costs
---------------------------------------------------------------------------

In most cases, you can safely ignore aider’s warning about unknown context window size and model costs.

Aider never _enforces_ token limits, it only _reports_ token limit errors from the API provider. You probably don’t need to configure aider with the proper token limits for unusual models.

But, you can register context window limits and costs for models that aren’t known to aider. Create a `.aider.model.metadata.json` file in one of these locations:

*   Your home directory.
*   The root if your git repo.
*   The current directory where you launch aider.
*   Or specify a specific file with the `--model-metadata-file <filename>` switch.

If the files above exist, they will be loaded in that order. Files loaded last will take priority.

The json file should be a dictionary with an entry for each model, as follows:

    {
        "deepseek/deepseek-chat": {
            "max_tokens": 4096,
            "max_input_tokens": 32000,
            "max_output_tokens": 4096,
            "input_cost_per_token": 0.00000014,
            "output_cost_per_token": 0.00000028,
            "litellm_provider": "deepseek",
            "mode": "chat"
        }
    }
    

Use a fully qualified model name with a `provider/` at the front in the `.aider.model.metadata.json` file. For example, use `deepseek/deepseek-chat`, not just `deepseek-chat`. That prefix should match the `litellm_provider` field.

### [](#contribute-model-metadata)Contribute model metadata

Aider relies on [litellm’s model\_prices\_and\_context\_window.json file](https://github.com/BerriAI/litellm/blob/main/model_prices_and_context_window.json) for model metadata.

Consider submitting a PR to that file to add missing models.

[](#model-settings)Model settings
---------------------------------

Aider has a number of settings that control how it works with different models. These model settings are pre-configured for most popular models. But it can sometimes be helpful to override them or add settings for a model that aider doesn’t know about.

### [](#configuration-file-locations)Configuration file locations

You can override or add settings for any model by creating a `.aider.model.settings.yml` file in one of these locations:

*   Your home directory.
*   The root if your git repo.
*   The current directory where you launch aider.
*   Or specify a specific file with the `--model-settings-file <filename>` switch.

If the files above exist, they will be loaded in that order. Files loaded last will take priority.

The yaml file should be a list of dictionary objects for each model.

### [](#global-extra-params)Global extra params

You can use the special model name `aider/extra_params` to define `extra_params` that will be passed to `litellm.completion()` for all models. Only the `extra_params` dict is used from this special model name.

For example:

    - name: aider/extra_params
      extra_params:
        extra_headers:
          Custom-Header: value
        max_tokens: 8192
    

These settings will be merged with any model-specific settings, with the `aider/extra_params` settings taking precedence for any direct conflicts.

### [](#example-model-settings)Example model settings

Below are all the pre-configured model settings to give a sense for the settings which are supported.

You can also look at the `ModelSettings` class in [models.py](https://github.com/Aider-AI/aider/blob/main/aider/models.py) file for more details about all of the model setting that aider supports.

    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-3.5-turbo
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-3.5-turbo-0125
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-3.5-turbo-1106
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-3.5-turbo-0613
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-3.5-turbo-16k-0613
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: udiff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: true
      name: gpt-4-turbo-2024-04-09
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: udiff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: true
      name: gpt-4-turbo
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: openai/gpt-4o
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: openai/gpt-4o-2024-08-06
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: gpt-4o-2024-08-06
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: gpt-4o-2024-11-20
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: openai/gpt-4o-2024-11-20
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: gpt-4o
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: true
      name: gpt-4o-mini
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: true
      name: openai/gpt-4o-mini
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: udiff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: gpt-4-0125-preview
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: udiff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: true
      name: gpt-4-1106-preview
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-4-vision-preview
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: false
      name: gpt-4-0314
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-4-0613
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gpt-4-32k-0613
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: claude-3-opus-20240229
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-5-haiku-20241022
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openrouter/anthropic/claude-3-opus
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/anthropic/claude-3-5-haiku
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: claude-3-sonnet-20240229
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: claude-3-5-sonnet-20240620
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: claude-3-5-sonnet-20240620
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: anthropic/claude-3-5-sonnet-20240620
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: anthropic/claude-3-5-sonnet-20240620
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: anthropic/claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: anthropic/claude-3-5-sonnet-20241022
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: anthropic/claude-3-5-sonnet-20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: anthropic/claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: bedrock/anthropic.claude-3-5-sonnet-20241022-v2:0
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: bedrock/anthropic.claude-3-5-sonnet-20241022-v2:0
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: bedrock/anthropic.claude-3-5-haiku-20241022-v1:0
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: anthropic/claude-3-5-sonnet-20241022
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: anthropic/claude-3-5-sonnet-latest
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: anthropic/claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: claude-3-5-sonnet-20241022
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
        max_tokens: 8192
      lazy: false
      name: claude-3-5-sonnet-20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
      lazy: false
      name: anthropic/claude-3-haiku-20240307
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: anthropic/claude-3-haiku-20240307
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
      lazy: false
      name: anthropic/claude-3-5-haiku-20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: anthropic/claude-3-5-haiku-20241022
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
      lazy: false
      name: bedrock/anthropic.claude-3-5-haiku-20241022-v1:0
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: bedrock/anthropic.claude-3-5-haiku-20241022-v1:0
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
      lazy: false
      name: claude-3-5-haiku-20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-5-haiku-20241022
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params:
        max_tokens: 4096
      lazy: false
      name: vertex_ai/claude-3-5-haiku@20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: vertex_ai/claude-3-5-haiku@20241022
    - cache_control: true
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        extra_headers:
          anthropic-beta: prompt-caching-2024-07-31,pdfs-2024-09-25
      lazy: false
      name: claude-3-haiku-20240307
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: claude-3-haiku-20240307
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/anthropic/claude-3.5-sonnet
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: openrouter/anthropic/claude-3.5-sonnet
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/anthropic/claude-3-5-haiku
    - cache_control: true
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/anthropic/claude-3.5-sonnet:beta
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: openrouter/anthropic/claude-3.5-sonnet:beta
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/anthropic/claude-3-5-haiku:beta
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: vertex_ai/claude-3-5-sonnet@20240620
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: vertex_ai/claude-3-5-sonnet@20240620
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: vertex_ai/claude-3-5-haiku@20241022
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: vertex_ai/claude-3-5-sonnet-v2@20241022
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: vertex_ai/claude-3-5-sonnet-v2@20241022
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: vertex_ai/claude-3-5-haiku@20241022
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: vertex_ai/claude-3-opus@20240229
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: vertex_ai/claude-3-5-haiku@20241022
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: vertex_ai/claude-3-sonnet@20240229
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: vertex_ai/claude-3-5-haiku@20241022
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: command-r-plus
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: command-r-plus
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: command-r-08-2024
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: command-r-08-2024
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: command-r-plus-08-2024
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: command-r-plus-08-2024
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: false
      name: groq/llama3-70b-8192
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: groq/llama3-8b-8192
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: false
      name: openrouter/meta-llama/llama-3-70b-instruct
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/meta-llama/llama-3-70b-instruct
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-pro-002
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-flash-002
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff-fenced
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-pro
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff-fenced
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-pro-latest
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff-fenced
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-pro-exp-0827
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-exp-1206
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-exp-1114
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-exp-1121
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff-fenced
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: vertex_ai/gemini-pro-experimental
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-1.5-flash-exp-0827
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: false
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: gemini/gemini-2.0-flash-exp
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: true
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/deepseek/deepseek-chat
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: openrouter/deepseek/deepseek-r1
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: false
      weak_model_name: openrouter/deepseek/deepseek-chat
    - cache_control: false
      caches_by_default: true
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: deepseek/deepseek-chat
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: deepseek/deepseek-reasoner
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: false
      weak_model_name: deepseek/deepseek-chat
    - cache_control: false
      caches_by_default: true
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: deepseek/deepseek-chat
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: true
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: deepseek/deepseek-coder
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: deepseek-chat
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: true
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params:
        max_tokens: 8192
      lazy: false
      name: deepseek-coder
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: false
      name: openrouter/deepseek/deepseek-coder
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: null
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: false
      name: openrouter/deepseek/deepseek-chat
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: null
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: null
      examples_as_sys_msg: true
      extra_params: null
      lazy: true
      name: openrouter/openai/gpt-4o
      reminder: sys
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: editor-diff
      editor_model_name: openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openai/o1-mini
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: editor-diff
      editor_model_name: azure/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: azure/o1-mini
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: azure/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: editor-diff
      editor_model_name: gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: o1-mini
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openai/o1-preview
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: azure/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: azure/o1-preview
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: azure/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: architect
      editor_edit_format: editor-diff
      editor_model_name: gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: o1-preview
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: whole
      editor_edit_format: editor-diff
      editor_model_name: openrouter/openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openrouter/openai/o1-mini
      reminder: user
      send_undo_reply: false
      streaming: false
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: openrouter/openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openrouter/openai/o1-preview
      reminder: user
      send_undo_reply: false
      streaming: false
      use_repo_map: true
      use_system_prompt: false
      use_temperature: false
      weak_model_name: openrouter/openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openrouter/openai/o1
      reminder: user
      send_undo_reply: false
      streaming: false
      use_repo_map: true
      use_system_prompt: true
      use_temperature: false
      weak_model_name: openrouter/openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openai/gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openai/o1
      reminder: user
      send_undo_reply: false
      streaming: false
      use_repo_map: true
      use_system_prompt: true
      use_temperature: false
      weak_model_name: openai/gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: gpt-4o
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: o1
      reminder: user
      send_undo_reply: false
      streaming: false
      use_repo_map: true
      use_system_prompt: true
      use_temperature: false
      weak_model_name: gpt-4o-mini
    - cache_control: false
      caches_by_default: false
      edit_format: diff
      editor_edit_format: editor-diff
      editor_model_name: openrouter/qwen/qwen-2.5-coder-32b-instruct
      examples_as_sys_msg: false
      extra_params: null
      lazy: false
      name: openrouter/qwen/qwen-2.5-coder-32b-instruct
      reminder: user
      send_undo_reply: false
      streaming: true
      use_repo_map: true
      use_system_prompt: true
      use_temperature: true
      weak_model_name: openrouter/qwen/qwen-2.5-coder-32b-instruct

---



## [https://aider.chat/docs/config/model-aliases.html](https://aider.chat/docs/config/model-aliases.html)

[](#model-aliases)Model Aliases
===============================

Model aliases allow you to create shorthand names for models you frequently use. This is particularly useful for models with long names or when you want to standardize model usage across your team.

[](#command-line-usage)Command Line Usage
-----------------------------------------

You can define aliases when launching aider using the `--alias` option:

    aider --alias "fast:gpt-3.5-turbo" --alias "smart:gpt-4"
    

Multiple aliases can be defined by using the `--alias` option multiple times. Each alias definition should be in the format `alias:model-name`.

[](#configuration-file)Configuration File
-----------------------------------------

You can also define aliases in your [`.aider.conf.yml` file](https://aider.chat/docs/config/aider_conf.html):

    alias:
      - "fast:gpt-3.5-turbo"
      - "smart:gpt-4"
      - "hacker:claude-3-sonnet-20240229"
    

[](#using-aliases)Using Aliases
-------------------------------

Once defined, you can use the alias instead of the full model name:

    aider --model fast  # Uses gpt-3.5-turbo
    aider --model smart  # Uses gpt-4
    

[](#built-in-aliases)Built-in Aliases
-------------------------------------

Aider includes some built-in aliases for convenience:

*   `3`: gpt-3.5-turbo
*   `35-turbo`: gpt-3.5-turbo
*   `35turbo`: gpt-3.5-turbo
*   `4`: gpt-4-0613
*   `4-turbo`: gpt-4-1106-preview
*   `4o`: gpt-4o
*   `deepseek`: deepseek/deepseek-chat
*   `flash`: gemini/gemini-2.0-flash-exp
*   `haiku`: claude-3-5-haiku-20241022
*   `opus`: claude-3-opus-20240229
*   `r1`: deepseek/deepseek-reasoner
*   `sonnet`: claude-3-5-sonnet-20241022

[](#priority)Priority
---------------------

If the same alias is defined in multiple places, the priority is:

1.  Command line aliases (highest priority)
2.  Configuration file aliases
3.  Built-in aliases (lowest priority)

This allows you to override built-in aliases with your own preferences.

---



## [https://aider.chat/docs/troubleshooting.html](https://aider.chat/docs/troubleshooting.html)

[](#troubleshooting)Troubleshooting
===================================

Below are some approaches for troubleshooting problems with aider.

If you need more help, please check our [GitHub issues](https://github.com/Aider-AI/aider/issues) and file a new issue if your problem isn’t discussed. Or drop into our [Discord](https://discord.gg/Tv2uQnR88V) to chat with us.

When reporting problems, it is very helpful if you can provide:

*   Aider version
*   LLM model you are using

Including the “announcement” lines that aider prints at startup is an easy way to share this helpful info.

    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 243 files
    Repo-map: using 1024 tokens
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

* * *

Table of contents
-----------------

*   [File editing problems](/docs/troubleshooting/edit-errors.html)
*   [Model warnings](/docs/troubleshooting/warnings.html)
*   [Token limits](/docs/troubleshooting/token-limits.html)
*   [Aider not found](/docs/troubleshooting/aider-not-found.html)
*   [Dependency versions](/docs/troubleshooting/imports.html)
*   [Using /help](/docs/troubleshooting/support.html)

---



## [https://aider.chat/docs/troubleshooting/edit-errors.html](https://aider.chat/docs/troubleshooting/edit-errors.html)

[](#file-editing-problems)File editing problems
===============================================

Sometimes the LLM will reply with some code changes that don’t get applied to your local files. In these cases, aider might say something like “Failed to apply edit to _filename_” or other error messages.

This usually happens because the LLM is disobeying the system prompts and trying to make edits in a format that aider doesn’t expect. Aider makes every effort to get the LLM to conform, and works hard to deal with LLM edits that are “almost” correctly formatted.

But sometimes the LLM just won’t cooperate. In these cases, here are some things you might try.

[](#dont-add-too-many-files)Don’t add too many files
----------------------------------------------------

Many LLMs now have very large context windows, but filling them with irrelevant code or conversation can confuse the model.

*   Don’t add too many files to the chat, _just_ add the files you think need to be edited. Aider also sends the LLM a [map of your entire git repo](https://aider.chat/docs/repomap.html), so other relevant code will be included automatically.
*   Use `/drop` to remove files from the chat session which aren’t needed for the task at hand. This will reduce distractions and may help the LLM produce properly formatted edits.
*   Use `/clear` to remove the conversation history, again to help the LLM focus.
*   Use `/tokens` to see how many tokens you are using for each message.

[](#use-a-more-capable-model)Use a more capable model
-----------------------------------------------------

If possible try using GPT-4o, Claude 3.5 Sonnet or Claude 3 Opus, as they are the strongest and most capable models.

Weaker models are more prone to disobeying the system prompt instructions. Most local models are just barely capable of working with aider, so editing errors are probably unavoidable.

[](#local-models-context-window-and-quantization)Local models: context window and quantization
----------------------------------------------------------------------------------------------

Be especially careful about the [Ollama context window](https://aider.chat/docs/llms/ollama.html#setting-the-context-window-size) when working with local models. It defaults to be very small and silently discards data if you exceed it.

Local models which have been quantized are more likely to have editing problems because they are not capable enough to follow aider’s system prompts.

[](#try-the-whole-edit-format)Try the whole edit format
-------------------------------------------------------

Run aider with `--edit-format whole` if were using a different edit format. You can see which edit format it is using in the announce lines:

    Aider v0.50.2-dev
    Models: claude-3-5-sonnet-20240620 with ♾️ diff edit format
    

[](#try-architect-mode)Try architect mode
-----------------------------------------

Run aider with `--architect` or `/chat-mode architect` to enable [architect mode](/docs/usage/modes.html#architect-mode-and-the-editor-model). This mode first proposes changes, then uses a separate model to handle the file edits. This two-step process often produces more reliable edits, especially with models that have trouble following edit format instructions.

[](#more-help)More help
-----------------------

If you need more help, please check our [GitHub issues](https://github.com/Aider-AI/aider/issues) and file a new issue if your problem isn’t discussed. Or drop into our [Discord](https://discord.gg/Tv2uQnR88V) to chat with us.

When reporting problems, it is very helpful if you can provide:

*   Aider version
*   LLM model you are using

Including the “announcement” lines that aider prints at startup is an easy way to share this helpful info.

    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 243 files
    Repo-map: using 1024 tokens
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

---



## [https://aider.chat/docs/troubleshooting/warnings.html](https://aider.chat/docs/troubleshooting/warnings.html)

[](#model-warnings)Model warnings
=================================

[](#unknown-context-window-size-and-token-costs)Unknown context window size and token costs
-------------------------------------------------------------------------------------------

    Model foobar: Unknown context window size and costs, using sane defaults.
    

If you specify a model that aider has never heard of, you will get this warning. This means aider doesn’t know the context window size and token costs for that model. Aider will use an unlimited context window and assume the model is free, so this is not usually a significant problem.

See the docs on [configuring advanced model settings](/docs/config/adv-model-settings.html) for details on how to remove this warning.

You can probably ignore the unknown context window size and token costs warning.

[](#did-you-mean)Did you mean?
------------------------------

If aider isn’t familiar with the model you’ve specified, it will suggest similarly named models. This helps in the case where you made a typo or mistake when specifying the model name.

    Model gpt-5o: Unknown context window size and costs, using sane defaults.
    Did you mean one of these?
    - gpt-4o
    

[](#missing-environment-variables)Missing environment variables
---------------------------------------------------------------

You need to set the listed environment variables. Otherwise you will get error messages when you start chatting with the model.

    Model azure/gpt-4-turbo: Missing these environment variables:
    - AZURE_API_BASE
    - AZURE_API_VERSION
    - AZURE_API_KEY
    

On Windows, if you just set these environment variables using `setx` you may need to restart your terminal or command prompt for the changes to take effect.

[](#unknown-which-environment-variables-are-required)Unknown which environment variables are required
-----------------------------------------------------------------------------------------------------

    Model gpt-5: Unknown which environment variables are required.
    

Aider is unable verify the environment because it doesn’t know which variables are required for the model. If required variables are missing, you may get errors when you attempt to chat with the model. You can look in the [aider’s LLM documentation](/docs/llms.html) or the [litellm documentation](https://docs.litellm.ai/docs/providers) to see if the required variables are listed there.

[](#more-help)More help
-----------------------

If you need more help, please check our [GitHub issues](https://github.com/Aider-AI/aider/issues) and file a new issue if your problem isn’t discussed. Or drop into our [Discord](https://discord.gg/Tv2uQnR88V) to chat with us.

When reporting problems, it is very helpful if you can provide:

*   Aider version
*   LLM model you are using

Including the “announcement” lines that aider prints at startup is an easy way to share this helpful info.

    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 243 files
    Repo-map: using 1024 tokens
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

---



## [https://aider.chat/docs/troubleshooting/token-limits.html](https://aider.chat/docs/troubleshooting/token-limits.html)

[](#token-limits)Token limits
=============================

Every LLM has limits on how many tokens it can process for each request:

*   The model’s **context window** limits how many total tokens of _input and output_ it can process.
*   Each model has limit on how many **output tokens** it can produce.

Aider will report an error **if a model responds** indicating that it has exceeded a token limit. The error will include suggested actions to try and avoid hitting token limits.

Here’s an example error:

    Model gpt-3.5-turbo has hit a token limit!
    
    Input tokens: 768 of 16385
    Output tokens: 4096 of 4096 -- exceeded output limit!
    Total tokens: 4864 of 16385
    
    To reduce output tokens:
    - Ask for smaller changes in each request.
    - Break your code into smaller source files.
    - Try using a stronger model like gpt-4o or opus that can return diffs.
    
    For more info: https://aider.chat/docs/token-limits.html
    

Aider never _enforces_ token limits, it only _reports_ token limit errors from the API provider. The token counts that aider reports are _estimates_.

[](#input-tokens--context-window-size)Input tokens & context window size
------------------------------------------------------------------------

The most common problem is trying to send too much data to a model, overflowing its context window. Technically you can exhaust the context window if the input is too large or if the input plus output are too large.

Strong models like GPT-4o and Opus have quite large context windows, so this sort of error is typically only an issue when working with weaker models.

The easiest solution is to try and reduce the input tokens by removing files from the chat. It’s best to only add the files that aider will need to _edit_ to complete your request.

*   Use `/tokens` to see token usage.
*   Use `/drop` to remove unneeded files from the chat session.
*   Use `/clear` to clear the chat history.
*   Break your code into smaller source files.

[](#output-token-limits)Output token limits
-------------------------------------------

Most models have quite small output limits, often as low as 4k tokens. If you ask aider to make a large change that affects a lot of code, the LLM may hit output token limits as it tries to send back all the changes.

To avoid hitting output token limits:

*   Ask for smaller changes in each request.
*   Break your code into smaller source files.
*   Use a strong model like gpt-4o, sonnet or opus that can return diffs.
*   Use a model that supports [infinite output](/docs/more/infinite-output.html).

[](#other-causes)Other causes
-----------------------------

Sometimes token limit errors are caused by non-compliant API proxy servers or bugs in the API server you are using to host a local model. Aider has been well tested when directly connecting to major [LLM provider cloud APIs](https://aider.chat/docs/llms.html). For serving local models, [Ollama](https://aider.chat/docs/llms/ollama.html) is known to work well with aider.

Try using aider without an API proxy server or directly with one of the recommended cloud APIs and see if your token limit problems resolve.

[](#more-help)More help
-----------------------

If you need more help, please check our [GitHub issues](https://github.com/Aider-AI/aider/issues) and file a new issue if your problem isn’t discussed. Or drop into our [Discord](https://discord.gg/Tv2uQnR88V) to chat with us.

When reporting problems, it is very helpful if you can provide:

*   Aider version
*   LLM model you are using

Including the “announcement” lines that aider prints at startup is an easy way to share this helpful info.

    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 243 files
    Repo-map: using 1024 tokens
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

---



## [https://aider.chat/docs/troubleshooting/aider-not-found.html](https://aider.chat/docs/troubleshooting/aider-not-found.html)

[](#aider-not-found)Aider not found
===================================

In some environments the `aider` command may not be available on your shell path. This can occur because of permissions/security settings in your OS, and often happens to Windows users.

You may see an error message like this:

> aider: The term ‘aider’ is not recognized as a name of a cmdlet, function, script file, or executable program. Check the spelling of the name, or if a path was included, verify that the path is correct and try again.

Below is the most fail safe way to run aider in these situations:

    python -m aider
    

You should also consider [installing aider using aider-install, uv or pipx](/docs/install.html).

---



## [https://aider.chat/docs/troubleshooting/imports.html](https://aider.chat/docs/troubleshooting/imports.html)

[](#dependency-versions)Dependency versions
===========================================

Aider expects to be installed with the correct versions of all of its required dependencies.

If you’ve been linked to this doc from a GitHub issue, or if aider is reporting `ImportErrors` it is likely that your aider install is using incorrect dependencies.

[](#avoid-package-conflicts)Avoid package conflicts
---------------------------------------------------

If you are using aider to work on a python project, sometimes your project will require specific versions of python packages which conflict with the versions that aider requires. If this happens, you may see errors like these when running pip installs:

    aider-chat 0.23.0 requires somepackage==X.Y.Z, but you have somepackage U.W.V which is incompatible.
    

[](#install-with-aider-install-uv-or-pipx)Install with aider-install, uv or pipx
--------------------------------------------------------------------------------

If you are having dependency problems you should consider [installing aider using aider-install, uv or pipx](/docs/install.html). This will ensure that aider is installed in its own python environment, with the correct set of dependencies.

[](#package-managers-like-homebrew-aur-ports)Package managers like Homebrew, AUR, ports
---------------------------------------------------------------------------------------

Package managers often install aider with the wrong dependencies, leading to import errors and other problems.

It is recommended to [install aider using aider-install, uv or pipx](/docs/install.html).

[](#dependency-versions-matter)Dependency versions matter
---------------------------------------------------------

Aider pins its dependencies and is tested to work with those specific versions. If you are installing aider directly with pip you should be careful about upgrading or downgrading the python packages that aider uses.

In particular, be careful with the packages with pinned versions noted at the end of [aider’s requirements.in file](https://github.com/Aider-AI/aider/blob/main/requirements/requirements.in). These versions are pinned because aider is known not to work with the latest versions of these libraries.

Also be wary of upgrading `litellm`, as it changes versions frequently and sometimes introduces bugs or backwards incompatible changes.

[](#replit)Replit
-----------------

To use aider with pipx on replit, you can run these commands in the replit shell:

    pip install pipx
    pipx run aider-chat ...normal aider args...
    

If you install aider with pipx on replit and try and run it as just `aider` it will crash with a missing `libstdc++.so.6` library.

---



## [https://aider.chat/docs/troubleshooting/support.html](https://aider.chat/docs/troubleshooting/support.html)

[](#using-help)Using /help
==========================

Type `/help <question>` and aider will respond with helpful information. You can ask questions about using aider, customizing settings, troubleshooting, using LLMs, etc.

Behind the scenes, aider has indexed all of its [documentation](https://aider.chat/). It uses the question to find relevant docs and share them with the LLM to do retrieval augmented generation (RAG) The LLM also has the full context of your ongoing aider chat, so it can help with the exact issue you might be facing.

> Aider v0.42.1-dev  
> Models: claude-3-5-sonnet with diff edit format  
> Repo-map: using 1024 tokens  
> Use /help <question> to ask for help, run with –help to see cmd line args

#### [](#help-is-the-env-file-global-or-for-a-git-repo)/help is the .env file global or for a git repo?

Based on the provided documentation, here’s the answer to your question about the .env file in aider:

The .env file in aider can be both global and specific to a git repository. Aider looks for .env files in multiple locations, with the following priority order:

1.  Your home directory (global)
2.  The root of your git repo (repo-specific)
3.  The current directory
4.  A file specified with the `--env-file <filename>` parameter

If multiple .env files exist in these locations, they are loaded in the order listed above, with files loaded last taking priority. This means you can have a global .env file in your home directory with general settings, and then override or add to those settings with a repo-specific .env file in your git repository root.

Here are some relevant documentation links that you might find helpful:

*   https://aider.chat/docs/config.html
*   https://aider.chat/docs/config/dotenv.html

The ability to use both global and repo-specific .env files allows for flexible configuration, where you can set default values globally and override them on a per-project basis as needed.

#### [](#help-can-i-use-local-llms)/help can i use local LLMs?

Yes, you can use local LLMs with Aider. Here’s a summary of the options:

1.  Ollama: Aider supports using local models through Ollama.
    
2.  OpenAI-compatible API: Aider can access local models that provide an OpenAI-compatible API.
    
3.  Other local models: Aider uses the LiteLLM package to connect to various LLM providers, which may include options for running models locally.
    

However, it’s important to note that Aider works best with more capable models. Less capable models may have difficulty properly returning “code edits,” which could result in Aider not being able to edit your files and commit changes effectively.

For more detailed information on using local LLMs and connecting to various models, you might want to check out these relevant documentation pages:

*   https://aider.chat/docs/llms.html
*   https://aider.chat/docs/llms/ollama.html
*   https://aider.chat/docs/llms/openai-compat.html

Keep in mind that the performance and capabilities of local LLMs may vary depending on the specific model and your hardware resources.

[](#getting-more-help)Getting more help
---------------------------------------

If you need more help, please check our [GitHub issues](https://github.com/Aider-AI/aider/issues) and file a new issue if your problem isn’t discussed. Or drop into our [Discord](https://discord.gg/Tv2uQnR88V) to chat with us.

When reporting problems, it is very helpful if you can provide:

*   Aider version
*   LLM model you are using

Including the “announcement” lines that aider prints at startup is an easy way to share this helpful info.

    Aider v0.37.1-dev
    Models: gpt-4o with diff edit format, weak model gpt-3.5-turbo
    Git repo: .git with 243 files
    Repo-map: using 1024 tokens
    

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

---



## [https://aider.chat/examples/README.html](https://aider.chat/examples/README.html)

[](#example-chat-transcripts)Example chat transcripts
=====================================================

Below are some chat transcripts showing what it’s like to code with aider. In the chats, you’ll see a variety of coding tasks like generating new code, editing existing code, debugging, exploring unfamiliar code, etc.

*   [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have aider create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
    
*   [**Javascript Game Modification**](https://aider.chat/examples/2048-game.html): Dive into an existing open-source repo, and get aider’s help to understand it and make modifications.
    
*   [**Complex Multi-file Change with Debugging**](https://aider.chat/examples/complex-change.html): Aider makes a complex code change that is coordinated across multiple source files, and resolves bugs by reviewing error output and doc snippets.
    
*   [**Create a Black Box Test Case**](https://aider.chat/examples/add-test.html): Aider creates a “black box” test case without access to the source of the method being tested, using only a [high level map of the repository based on ctags](https://aider.chat/docs/ctags.html).
    
*   [**Honor the NO\_COLOR env var**](https://aider.chat/examples/no-color.html): The user pastes the NO\_COLOR spec from no-color.org into the chat, and aider modifies the application to conform.
    
*   [**Download, analyze and plot US Census data**](https://aider.chat/examples/census.html): Aider downloads census data, suggests some hypotheses to test, tests one and then summarizes and plots a graph of the results.
    
*   [**Semantic Search & Replace**](/examples/semantic-search-replace.html): Updating a collection of function calls, which requires dealing with various formatting and semantic differences in the various function call sites.
    
*   [**Pong Game with Pygame**](/examples/pong.html): Creating a simple Pong game using the Pygame library, with customizations for paddle size and color, and ball speed adjustments.
    
*   [**CSS Exercise: Animation Dropdown Menu**](/examples/css-exercises.html): A small CSS exercise involving adding animation to a dropdown menu.
    
*   [**Automatically Update Docs**](/examples/update-docs.html): Automatically updating documentation based on the latest version of the main() function.
    
*   [**Editing an Asciinema Cast File**](/examples/asciinema.html): Editing escape sequences in an `asciinema` screencast file.
    

[](#whats-happening-in-these-chats)What’s happening in these chats?
-------------------------------------------------------------------

To better understand the chat transcripts, it’s worth knowing that:

*   Each time the LLM suggests a code change, `aider` automatically applies it to the source files.
*   After applying the edits, `aider` commits them to git with a descriptive commit message.
*   The LLM can only see and edit files which have been “added to the chat session”. The user adds files either via the command line or the in-chat `/add` command. If the LLM asks to see specific files, `aider` asks the user for permission to add them to the chat. The transcripts contain notifications from `aider` whenever a file is added or dropped from the session.

[](#transcript-formatting)Transcript formatting
-----------------------------------------------

> This is output from the aider tool.

#### [](#these-are-chat-messages-written-by-the-user)These are chat messages written by the user.

Chat responses from the LLM are in a blue font like this, and often include colorized “edit blocks” that specify edits to the code. Here’s a sample edit block that switches from printing “hello” to “goodbye”:

    hello.py
    <<<<<<< ORIGINAL
    print("hello")
    =======
    print("goodbye")
    >>>>>>> UPDATED

---



## [https://aider.chat/examples/hello-world-flask.html](https://aider.chat/examples/hello-world-flask.html)

[](#create-a-simple-flask-app-with-aider)Create a simple flask app with aider
=============================================================================

In this chat transcript, the user asks to make a simple flask app with various endpoints.

> $ aider app.py  
> Creating empty file app.py  
> Added app.py to the chat

#### [](#make-a-flask-app-with-a-hello-endpoint-that-returns-hello-world)make a flask app with a /hello endpoint that returns hello world

To create a Flask app with a `/hello` endpoint that returns “Hello, World!”, we need to install Flask, import it, create an app instance, and define a route for the `/hello` endpoint. Here’s how to update the `app.py` file:

    app.py
    <<<<<<< ORIGINAL
    
    =======
    from flask import Flask
    
    app = Flask(__name__)
    
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    
    if __name__ == '__main__':
        app.run()
    >>>>>>> UPDATED
    

Make sure to install Flask in your project environment using `pip install flask` before running the app.

> Applied edit to app.py  
> Commit 414c394 aider: Added a `/hello` endpoint that returns “Hello, World!” to the Flask app.

#### [](#add-an-endpoint-like-add35-which-returns-the-sum-of-the-2-numbers)add an endpoint like /add/3/5 which returns the sum of the 2 numbers

To add an endpoint like `/add/3/5` that returns the sum of the two numbers, you can create a new route with two URL parameters. Update the `app.py` file as follows:

    app.py
    <<<<<<< ORIGINAL
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    =======
    @app.route('/add/<int:num1>/<int:num2>')
    def add(num1, num2):
        return str(num1 + num2)
    
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    >>>>>>> UPDATED
    

Now, when you visit `/add/3/5`, it will return the sum of the two numbers, which is `8`.

> Applied edit to app.py  
> Commit 0872c51 aider: Added an endpoint `/add/<int:num1>/<int:num2>` that returns the sum of the two numbers.

#### [](#add-fibonaccix)add /fibonacci/X

To add a `/fibonacci/X` endpoint that returns the Xth number in the Fibonacci sequence, you can create a new route with a URL parameter for X and a function to calculate the Fibonacci number. Update the `app.py` file as follows:

    app.py
    <<<<<<< ORIGINAL
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    =======
    def fibonacci(n):
        if n <= 0:
            return "Invalid input. Please enter a positive integer."
        elif n == 1:
            return 0
        elif n == 2:
            return 1
        else:
            a, b = 0, 1
            for _ in range(n - 2):
                a, b = b, a + b
            return b
    
    @app.route('/fibonacci/<int:x>')
    def fibonacci_x(x):
        return str(fibonacci(x))
    
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    >>>>>>> UPDATED
    

Now, when you visit `/fibonacci/X`, it will return the Xth number in the Fibonacci sequence. For example, `/fibonacci/5` will return `3`.

> Applied edit to app.py  
> Commit 163fba8 aider: Added a `/fibonacci/X` endpoint that returns the Xth number in the Fibonacci sequence.

#### [](#remove-the-hello-endpoint)remove the hello endpoint

To remove the `/hello` endpoint, you can simply delete the corresponding route and function in the `app.py` file. Here’s the update:

    app.py
    <<<<<<< ORIGINAL
    @app.route('/hello')
    def hello():
        return "Hello, World!"
    =======
    >>>>>>> UPDATED
    

Now, the `/hello` endpoint has been removed from the Flask app.

> Applied edit to app.py  
> Commit eab6620 aider: Removed the `/hello` endpoint from the Flask app.

---



## [https://aider.chat/examples/2048-game.html](https://aider.chat/examples/2048-game.html)

[](#modify-an-open-source-2048-game-with-aider)Modify an open source 2048 game with aider
=========================================================================================

In this chat transcript, the user explores and modifies an open source [javascript 2048 game repo](https://github.com/gabrielecirulli/2048).

Notice that the LLM asks to see a particular source file, and aider automatically includes it in the chat session after getting permission from the user.

> $ git clone https://github.com/gabrielecirulli/2048  
> $ cd 2048  
> $ aider

#### [](#what-is-this-repo)what is this repo?

Based on the file names you provided, it seems like this repository is for a web-based game, possibly a 2048 game clone. The files include JavaScript files for game logic, HTML and CSS files for the user interface, and various meta files for icons and touch startup images.

If you need help with any specific part of the code or want to add new features, please let me know, and I’ll be happy to assist you.

#### [](#how-does-the-scoring-work)how does the scoring work?

To help you with the scoring mechanism, I need to see the relevant code. Please provide the contents of the `js/game_manager.js` file, as it is likely to contain the scoring logic.

> js/game\_manager.js  
> Add these files to the chat? y

Apologies for the oversight. I see the contents of the `js/game_manager.js` file now.

The scoring in this 2048 game works as follows:

1.  When two tiles with the same value merge, they create a new tile with a value equal to the sum of the merged tiles’ values.
2.  The score is updated by adding the value of the new merged tile.

Here’s the relevant code snippet from the `js/game_manager.js` file:

    if (next && next.value === tile.value && !next.mergedFrom) {
      var merged = new Tile(positions.next, tile.value * 2);
      merged.mergedFrom = [tile, next];
    
      self.grid.insertTile(merged);
      self.grid.removeTile(tile);
    
      // Converge the two tiles' positions
      tile.updatePosition(positions.next);
    
      // Update the score
      self.score += merged.value;
    
      // The mighty 2048 tile
      if (merged.value === 2048) self.won = true;
    }
    

In this code snippet, when two tiles with the same value (`tile` and `next`) are found, they are merged into a new tile (`merged`). The value of the new tile is added to the current score (`self.score += merged.value`). If the merged tile’s value is 2048, the game is considered won (`self.won = true`).

#### [](#can-we-add-some-randomness-maybe-10-of-the-time-give-the-user-a-10x-bonus)can we add some randomness? maybe 10% of the time give the user a 10x bonus?

Sure, we can add a 10% chance of giving the user a 10x bonus when two tiles merge. To implement this, we’ll modify the scoring logic in the `js/game_manager.js` file. Here’s the step-by-step plan:

1.  Generate a random number between 0 and 1.
2.  Check if the random number is less than or equal to 0.1 (10% chance).
3.  If the condition is met, multiply the merged tile’s value by 10 before adding it to the score.

Here’s the code change for the `js/game_manager.js` file:

    js/game_manager.js
    <<<<<<< ORIGINAL
      // Update the score
      self.score += merged.value;
    =======
      // Update the score with a 10% chance of 10x bonus
      var bonus = Math.random() <= 0.1 ? 10 : 1;
      self.score += merged.value * bonus;
    >>>>>>> UPDATED
    

This change will give the user a 10x bonus 10% of the time when two tiles merge.

> Applied edit to js/game\_manager.js  
> Commit eb9d882 aider: Added a 10% chance of giving the user a 10x bonus when two tiles merge.

---



## [https://aider.chat/examples/complex-change.html](https://aider.chat/examples/complex-change.html)

[](#a-complex-multi-file-change-with-debugging)A complex multi-file change, with debugging
==========================================================================================

This is a chat transcript of a fairly complex code change. The user is trying to update tests to use an input mock provided by `prompt_toolkit`. This requires changes to multiple source files.

Some things to notice:

*   The initial changes don’t work, so the user provides error messages and snippets from the `prompt_toolkit` docs to collaboratively debug and solve the problem.
*   The user edits a file outside the chat using their editor. `aider` notices these out-of-band changes and offers to commit them.
*   At one point the user hits `^C` to interrupt the LLM response, since it’s not a useful response. The user gives clarifications and gets a better result on the next reply.

> $ aider tests/test\_main.py aider/getinput.py  
> Added tests/test\_main.py to the chat  
> Added aider/getinput.py to the chat

#### [](#instead-of-using-devnull-to-send-no-input-in-the-main-tests-can-we-use-the-prompttoolkit-input-mocking-functions)instead of using /dev/null to send no input in the main tests, can we use the prompt\_toolkit input mocking functions?

Yes, we can use the `prompt_toolkit.input` module to mock the input in the tests. Here’s how to modify the `tests/test_main.py` file:

    tests/test_main.py
    <<<<<<< ORIGINAL
    import os
    import sys
    import tempfile
    from unittest import TestCase
    from aider.main import main
    import subprocess
    =======
    import os
    import tempfile
    from unittest import TestCase
    from aider.main import main
    import subprocess
    from prompt_toolkit.input import create_pipe_input
    from prompt_toolkit.output import DummyOutput
    >>>>>>> UPDATED
    

Now, update the tests to use the `create_pipe_input` and `DummyOutput`:

    tests/test_main.py
    <<<<<<< ORIGINAL
                with open(os.devnull, "r") as dev_null:
                    save_stdin = sys.stdin
                    sys.stdin = dev_null
                    main([])
                    sys.stdin = save_stdin
    =======
                pipe_input = create_pipe_input()
                save_stdin = sys.stdin
                sys.stdin = pipe_input
                main([], input=pipe_input, output=DummyOutput())
                sys.stdin = save_stdin
                pipe_input.close()
    >>>>>>> UPDATED
    

    tests/test_main.py
    <<<<<<< ORIGINAL
                with open(os.devnull, "r") as dev_null:
                    save_stdin = sys.stdin
                    sys.stdin = dev_null
                    main(["foo.txt"])
                    sys.stdin = save_stdin
                    self.assertTrue(os.path.exists("foo.txt"))
    =======
                pipe_input = create_pipe_input()
                save_stdin = sys.stdin
                sys.stdin = pipe_input
                main(["foo.txt"], input=pipe_input, output=DummyOutput())
                sys.stdin = save_stdin
                pipe_input.close()
                self.assertTrue(os.path.exists("foo.txt"))
    >>>>>>> UPDATED
    

    tests/test_main.py
    <<<<<<< ORIGINAL
                with open(os.devnull, "r") as dev_null:
                    save_stdin = sys.stdin
                    sys.stdin = dev_null
                    main(["--yes", "foo.txt"])
                    sys.stdin = save_stdin
                    self.assertTrue(os.path.exists("foo.txt"))
    =======
                pipe_input = create_pipe_input()
                save_stdin = sys.stdin
                sys.stdin = pipe_input
                main(["--yes", "foo.txt"], input=pipe_input, output=DummyOutput())
                sys.stdin = save_stdin
                pipe_input.close()
                self.assertTrue(os.path.exists("foo.txt"))
    >>>>>>> UPDATED
    

These changes will replace the usage of `/dev/null` with `prompt_toolkit`’s input mocking functions.

> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Commit c177e29 aider: Replaced usage of /dev/null with prompt\_toolkit’s input mocking functions in tests.

> Git repo has uncommitted changes.  
> Suggested commit message:  
> Added import statement for sys module in test\_main.py.  
> Commit before the chat proceeds \[y/n/commit message\]? y  
> Commit 6724fcd Added import statement for sys module in test\_main.py.

#### [](#add-aidermainpy)/add aider/main.py

> Added aider/main.py to the chat

#### [](#i-am-getting-this-error-failed-teststestmainpytestmaintestmainwithemptygitdirnewfile---typeerror-main-got-an-unexpected-keyword-argument-input)I am getting this error: FAILED tests/test\_main.py::TestMain::test\_main\_with\_empty\_git\_dir\_new\_file - TypeError: main() got an unexpected keyword argument ‘input’

I apologize for the confusion. It seems I made a mistake in the `main()` function definition in `aider/main.py`. The `main()` function should accept `input` and `output` keyword arguments. Here’s the fix:

    aider/main.py
    <<<<<<< ORIGINAL
    def main(args=None):
        if args is None:
            args = sys.argv[1:]
    =======
    def main(args=None, input=None, output=None):
        if args is None:
            args = sys.argv[1:]
        if input is None:
            input = sys.stdin
        if output is None:
            output = sys.stdout
    >>>>>>> UPDATED
    

Now, the `main()` function will accept the `input` and `output` keyword arguments, and the tests should pass.

> Applied edit to aider/main.py  
> Commit 79dfba9 aider: Fixed main() function to accept input and output keyword arguments.

#### [](#we-need-to-pass-those-into-inputoutput-and-to-prompttoolkit-right)we need to pass those into InputOutput and to prompt\_toolkit right?

Yes, you’re right. We need to pass the `input` and `output` arguments to the `InputOutput` class and then to the `prompt_toolkit.prompt()` function. Here’s how to modify the `aider/getinput.py` and `aider/main.py` files:

In `aider/getinput.py`, update the `InputOutput` class to accept `input` and `output` arguments:

    aider/getinput.py
    <<<<<<< ORIGINAL
    class InputOutput:
        def __init__(self, pretty, yes, input_history_file, chat_history_file):
    =======
    class InputOutput:
        def __init__(self, pretty, yes, input_history_file, chat_history_file, input=None, output=None):
            self.input = input
            self.output = output
    >>>>>>> UPDATED
    

Now, update the `prompt()` function calls in the `get_input()` method to use the `input` and `output` arguments:

    aider/getinput.py
    <<<<<<< ORIGINAL
                line = prompt(
                    show,
                    completer=completer_instance,
                    history=FileHistory(self.input_history_file),
                    style=style,
                    reserve_space_for_menu=4,
                    complete_style=CompleteStyle.MULTI_COLUMN,
                )
    =======
                line = prompt(
                    show,
                    completer=completer_instance,
                    history=FileHistory(self.input_history_file),
                    style=style,
                    reserve_space_for_menu=4,
                    complete_style=CompleteStyle.MULTI_COLUMN,
                    input=self.input,
                    output=self.output,
                )
    >>>>>>> UPDATED
    

In `aider/main.py`, pass the `input` and `output` arguments to the `InputOutput` class:

    aider/main.py
    <<<<<<< ORIGINAL
        io = InputOutput(args.pretty, args.yes, args.input_history_file, args.chat_history_file)
    =======
        io = InputOutput(args.pretty, args.yes, args.input_history_file, args.chat_history_file, input=input, output=output)
    >>>>>>> UPDATED
    

These changes will ensure that the `input` and `output` arguments are passed to the `InputOutput` class and then to the `prompt_toolkit.prompt()` function.

> Applied edit to aider/getinput.py  
> Applied edit to aider/getinput.py  
> Applied edit to aider/main.py  
> Commit cea9d2a aider: Updated InputOutput class to accept input and output arguments and passed them to prompt\_toolkit.prompt() function.

#### [](#failed-teststestmainpytestmaintestmainwithemptygitdirnewfile---typeerror-prompt-got-an-unexpected-keyword-argument-input)FAILED tests/test\_main.py::TestMain::test\_main\_with\_empty\_git\_dir\_new\_file - TypeError: prompt() got an unexpected keyword argument ‘input’

I apologize for the confusion. It seems I made a mistake in the `prompt_toolkit.prompt()` function call. The `prompt()` function accepts `stdin` and `stdout` arguments instead of `input` and `output`. Here’s the fix:

Update the `prompt()` function call in the `get_input()` method in `aider/getinput.py`:

    aider/getinput.py
    <<<<<<< ORIGINAL
                input=self.input,
                output=self.output,
    =======
                stdin=self.input,
                stdout=self.output,
    >>>>>>> UPDATED
    

These changes will ensure that the `input` and `output` arguments are passed correctly to the `prompt_toolkit.prompt()` function.

> Applied edit to aider/getinput.py  
> Commit 55d3540 aider: Fixed `prompt()` function call in `get_input()` method to pass `stdin` and `stdout` arguments instead of `input` and `output`.

#### [](#prompttoolkitshortcutspromptmessage-anyformattedtext--none--none--history-history--none--none-editingmode-editingmode--none--none-refreshinterval-float--none--none-vimode-bool--none--none-lexer-lexer--none--none-completer-completer--none--none-completeinthread-bool--none--none-ispassword-bool--none--none-keybindings-keybindingsbase--none--none-bottomtoolbar-anyformattedtext--none--none-style-basestyle--none--none-colordepth-colordepth--none--none-cursor-anycursorshapeconfig--none-includedefaultpygmentsstyle-filterorbool--none--none-styletransformation-styletransformation--none--none-swaplightanddarkcolors-filterorbool--none--none-rprompt-anyformattedtext--none--none-multiline-filterorbool--none--none-promptcontinuation-promptcontinuationtext--none--none-wraplines-filterorbool--none--none-enablehistorysearch-filterorbool--none--none-searchignorecase-filterorbool--none--none-completewhiletyping-filterorbool--none--none-validatewhiletyping-filterorbool--none--none-completestyle-completestyle--none--none-autosuggest-autosuggest--none--none-validator-validator--none--none-clipboard-clipboard--none--none-mousesupport-filterorbool--none--none-inputprocessors-listprocessor--none--none-placeholder-anyformattedtext--none--none-reservespaceformenu-int--none--none-enablesystemprompt-filterorbool--none--none-enablesuspend-filterorbool--none--none-enableopenineditor-filterorbool--none--none-tempfilesuffix-str--callable-str--none--none-tempfile-str--callable-str--none--none-default-str---acceptdefault-bool--false-prerun-callable-none--none--none--str)prompt\_toolkit.shortcuts.prompt(message: AnyFormattedText | None = None, \*, history: History | None = None, editing\_mode: EditingMode | None = None, refresh\_interval: float | None = None, vi\_mode: bool | None = None, lexer: Lexer | None = None, completer: Completer | None = None, complete\_in\_thread: bool | None = None, is\_password: bool | None = None, key\_bindings: KeyBindingsBase | None = None, bottom\_toolbar: AnyFormattedText | None = None, style: BaseStyle | None = None, color\_depth: ColorDepth | None = None, cursor: AnyCursorShapeConfig = None, include\_default\_pygments\_style: FilterOrBool | None = None, style\_transformation: StyleTransformation | None = None, swap\_light\_and\_dark\_colors: FilterOrBool | None = None, rprompt: AnyFormattedText | None = None, multiline: FilterOrBool | None = None, prompt\_continuation: PromptContinuationText | None = None, wrap\_lines: FilterOrBool | None = None, enable\_history\_search: FilterOrBool | None = None, search\_ignore\_case: FilterOrBool | None = None, complete\_while\_typing: FilterOrBool | None = None, validate\_while\_typing: FilterOrBool | None = None, complete\_style: CompleteStyle | None = None, auto\_suggest: AutoSuggest | None = None, validator: Validator | None = None, clipboard: Clipboard | None = None, mouse\_support: FilterOrBool | None = None, input\_processors: list\[Processor\] | None = None, placeholder: AnyFormattedText | None = None, reserve\_space\_for\_menu: int | None = None, enable\_system\_prompt: FilterOrBool | None = None, enable\_suspend: FilterOrBool | None = None, enable\_open\_in\_editor: FilterOrBool | None = None, tempfile\_suffix: str | Callable\[\[\], str\] | None = None, tempfile: str | Callable\[\[\], str\] | None = None, default: str = ‘’, accept\_default: bool = False, pre\_run: Callable\[\[\], None\] | None = None) → str

I apologize for the confusion earlier. It seems that the `prompt_toolkit.prompt()` function does not accept `stdin` and `stdout` arguments directly. Instead, we need to use the `Application` class from `prompt_toolkit` to create a custom application with the desired input and output. Here’s how to modify the `aider/getinput.py` file:

First, import the necessary classes and functions from \`prompt\_tool

> ^C KeyboardInterrupt

#### [](#class-prompttoolkitshortcutspromptsessionmessage-anyformattedtext----multiline-filterorbool--false-wraplines-filterorbool--true-ispassword-filterorbool--false-vimode-bool--false-editingmode-editingmode--editingmodeemacs-emacs-completewhiletyping-filterorbool--true-validatewhiletyping-filterorbool--true-enablehistorysearch-filterorbool--false-searchignorecase-filterorbool--false-lexer-lexer--none--none-enablesystemprompt-filterorbool--false-enablesuspend-filterorbool--false-enableopenineditor-filterorbool--false-validator-validator--none--none-completer-completer--none--none-completeinthread-bool--false-reservespaceformenu-int--8-completestyle-completestyle--completestylecolumn-column-autosuggest-autosuggest--none--none-style-basestyle--none--none-styletransformation-styletransformation--none--none-swaplightanddarkcolors-filterorbool--false-colordepth-colordepth--none--none-cursor-anycursorshapeconfig--none-includedefaultpygmentsstyle-filterorbool--true-history-history--none--none-clipboard-clipboard--none--none-promptcontinuation-promptcontinuationtext--none--none-rprompt-anyformattedtext--none-bottomtoolbar-anyformattedtext--none-mousesupport-filterorbool--false-inputprocessors-listprocessor--none--none-placeholder-anyformattedtext--none--none-keybindings-keybindingsbase--none--none-erasewhendone-bool--false-tempfilesuffix-str--callable-str--none--txt-tempfile-str--callable-str--none--none-refreshinterval-float--0-input-input--none--none-output-output--none--none)class prompt\_toolkit.shortcuts.PromptSession(message: AnyFormattedText = ‘’, \*, multiline: FilterOrBool = False, wrap\_lines: FilterOrBool = True, is\_password: FilterOrBool = False, vi\_mode: bool = False, editing\_mode: EditingMode = <EditingMode.EMACS: ‘EMACS’>, complete\_while\_typing: FilterOrBool = True, validate\_while\_typing: FilterOrBool = True, enable\_history\_search: FilterOrBool = False, search\_ignore\_case: FilterOrBool = False, lexer: Lexer | None = None, enable\_system\_prompt: FilterOrBool = False, enable\_suspend: FilterOrBool = False, enable\_open\_in\_editor: FilterOrBool = False, validator: Validator | None = None, completer: Completer | None = None, complete\_in\_thread: bool = False, reserve\_space\_for\_menu: int = 8, complete\_style: CompleteStyle = <CompleteStyle.COLUMN: ‘COLUMN’>, auto\_suggest: AutoSuggest | None = None, style: BaseStyle | None = None, style\_transformation: StyleTransformation | None = None, swap\_light\_and\_dark\_colors: FilterOrBool = False, color\_depth: ColorDepth | None = None, cursor: AnyCursorShapeConfig = None, include\_default\_pygments\_style: FilterOrBool = True, history: History | None = None, clipboard: Clipboard | None = None, prompt\_continuation: PromptContinuationText | None = None, rprompt: AnyFormattedText = None, bottom\_toolbar: AnyFormattedText = None, mouse\_support: FilterOrBool = False, input\_processors: list\[Processor\] | None = None, placeholder: AnyFormattedText | None = None, key\_bindings: KeyBindingsBase | None = None, erase\_when\_done: bool = False, tempfile\_suffix: str | Callable\[\[\], str\] | None = ‘.txt’, tempfile: str | Callable\[\[\], str\] | None = None, refresh\_interval: float = 0, input: Input | None = None, output: Output | None = None)

Thank you for providing the `PromptSession` class information. We can use the `PromptSession` class to create a custom session with the desired input and output. Here’s how to modify the `aider/getinput.py` file:

First, import the `PromptSession` class from `prompt_toolkit.shortcuts`:

    aider/getinput.py
    <<<<<<< ORIGINAL
    from prompt_toolkit import prompt
    =======
    from prompt_toolkit.shortcuts import PromptSession
    >>>>>>> UPDATED
    

Now, update the `get_input()` method to use the `PromptSession` class:

    aider/getinput.py
    <<<<<<< ORIGINAL
                line = prompt(
                    show,
                    completer=completer_instance,
                    history=FileHistory(self.input_history_file),
                    style=style,
                    reserve_space_for_menu=4,
                    complete_style=CompleteStyle.MULTI_COLUMN,
                    input=self.input,
                    output=self.output,
                )
    =======
                session = PromptSession(
                    message=show,
                    completer=completer_instance,
                    history=FileHistory(self.input_history_file),
                    style=style,
                    reserve_space_for_menu=4,
                    complete_style=CompleteStyle.MULTI_COLUMN,
                    input=self.input,
                    output=self.output,
                )
                line = session.prompt()
    >>>>>>> UPDATED
    

These changes will ensure that the `input` and `output` arguments are passed correctly to the `prompt_toolkit`’s `PromptSession` class.

> Applied edit to aider/getinput.py  
> Applied edit to aider/getinput.py  
> Commit ac92cca aider: Replaced `prompt()` with `PromptSession()` to correctly pass input and output arguments.

#### [](#try-using-createinputstringio-in-the-tests)try using create\_input(StringIO(‘’)) in the tests

I understand that you want to use `create_input(StringIO(''))` in the tests. However, I need more information about which test cases you want to apply this change to and how you want to use it. Please provide more details or examples.

#### [](#the-ones-that-currently-use-createpipeinput)the ones that currently use create\_pipe\_input()

I see that you want to replace `create_pipe_input()` with `create_input(StringIO(''))` in the test cases. Here are the changes for the `tests/test_main.py` file:

    tests/test_main.py
    <<<<<<< ORIGINAL
    from prompt_toolkit.input import create_pipe_input
    =======
    from prompt_toolkit.input import create_input
    from io import StringIO
    >>>>>>> UPDATED
    

    tests/test_main.py
    <<<<<<< ORIGINAL
                pipe_input = create_pipe_input()
    =======
                pipe_input = create_input(StringIO(''))
    >>>>>>> UPDATED
    

    tests/test_main.py
    <<<<<<< ORIGINAL
                pipe_input = create_pipe_input()
    =======
                pipe_input = create_input(StringIO(''))
    >>>>>>> UPDATED
    

    tests/test_main.py
    <<<<<<< ORIGINAL
                pipe_input = create_pipe_input()
    =======
                pipe_input = create_input(StringIO(''))
    >>>>>>> UPDATED
    

These changes will replace the usage of `create_pipe_input()` with `create_input(StringIO(''))` in the test cases.

> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Applied edit to tests/test\_main.py  
> Commit 4bb043f aider: Replaced the usage of `create_pipe_input()` with `create_input(StringIO(''))` in the test cases.

#### [](#nice-that-worked)nice, that worked!

I’m glad the changes worked for you! If you have any more requests or need further assistance, feel free to ask.

---



## [https://aider.chat/examples/add-test.html](https://aider.chat/examples/add-test.html)

[](#create-a-black-box-test-case)Create a “black box” test case
===============================================================

This transcript shows aider creating a black box test case, **without being given access to the source code of the function being tested or any of the other code in the repo.**

Instead, aider is operating entirely off a [high level map of the repository based on ctags](https://aider.chat/docs/ctags.html), which provides details on all the symbols and function signatures in the repo. Using only the meta-data in the map, the LLM is able to figure out how to call the method to be tested, as well as how to instantiate multiple class objects that are required to prepare for the test.

In detail, aider is able to use the repo map to:

*   Find the function signature of the `cmd_add()` function which the user wants a test case for.
*   Determine that it is a method of the `Command` class, so the test case will need to instantiate an instance to conduct the test.
*   Identify that creating a `Command` instance requires passing in `InputOutput` and `Coder` instances.
*   Figure out the arguments required to instantiate the `InputOutput` instance.
*   Decide that the `Coder` class looks complex enough to use a `MagickMock`.

The `cmd_add()` method is defined without type annotations, so aider makes a reasonable but incorrect guess that it accepts a `list` of files. The user invokes the `/run` command to run the new unit test, which throws an error based on this misunderstanding.

The LLM reviews the error message and fixes the call to `cmd_add()` to correctly pass a `str` with a space-separated list of filenames instead. The test then passes on the next `/run`.

> $ aider tests/test\_commands.py  
> Creating empty file tests/test\_commands.py  
> Added tests/test\_commands.py to the chat  
> Files not tracked in .git:
> 
> *   tests/test\_commands.py
> 
> Add them? y  
> Added tests/test\_commands.py to the git repo  
> Commit b9cea2c Added new files to the git repo: tests/test\_commands.py  
> Using git repo: .git

#### [](#add-a-test-for-cmdadd-that-passes-in-footxt-and-bartxt-and-ensures-they-have-both-been-created-after-the-test-run-the-test-in-a-tmp-dir)add a test for cmd\_add that passes in ‘foo.txt’ and ‘bar.txt’ and ensures they have both been created after the test. run the test in a tmp dir.

I will add a new test method called `test_cmd_add` in the `tests/test_commands.py` file. This test will create a temporary directory, change the current working directory to the temporary directory, and then call the `cmd_add` method with ‘foo.txt’ and ‘bar.txt’ as arguments. After that, it will check if both files have been created in the temporary directory.

Here’s the code change:

    tests/test_commands.py
    <<<<<<< ORIGINAL
    =======
    import os
    import tempfile
    from unittest import TestCase
    from unittest.mock import MagicMock
    from aider.commands import Commands
    from aider.io import InputOutput
    
    class TestCommands(TestCase):
        def test_cmd_add(self):
            # Create a temporary directory and change the current working directory
            with tempfile.TemporaryDirectory() as tmpdir:
                os.chdir(tmpdir)
    
                # Initialize the Commands and InputOutput objects
                io = InputOutput(pretty=False, yes=True)
                coder = MagicMock()
                commands = Commands(io, coder)
    
                # Call the cmd_add method with 'foo.txt' and 'bar.txt'
                commands.cmd_add(["foo.txt", "bar.txt"])
    
                # Check if both files have been created in the temporary directory
                self.assertTrue(os.path.exists("foo.txt"))
                self.assertTrue(os.path.exists("bar.txt"))
    >>>>>>> UPDATED
    

This test will ensure that the `cmd_add` method creates the specified files in the current working directory.

> Applied edit to tests/test\_commands.py  
> Commit e2d5212 aider: Added a test method `test_cmd_add` that creates a temporary directory, calls the `cmd_add` method with ‘foo.txt’ and ‘bar.txt’, and checks if both files have been created in the temporary directory.

#### [](#run-pytest-teststestcommandspy)/run pytest tests/test\_commands.py

>     ============================= test session starts ==============================  
>     platform darwin -- Python 3.11.3, pytest-7.3.1, pluggy-1.0.0  
>     rootdir: /Users/gauthier/Projects/aider  
>     collected 1 item  
>       
>     tests/test_commands.py F                                                 [100%]  
>       
>     =================================== FAILURES ===================================  
>     __________________________ TestCommands.test_cmd_add ___________________________  
>       
>     self = <tests.test_commands.TestCommands testMethod=test_cmd_add>  
>       
>         def test_cmd_add(self):  
>             # Create a temporary directory and change the current working directory  
>             with tempfile.TemporaryDirectory() as tmpdir:  
>                 os.chdir(tmpdir)  
>       
>                 # Initialize the Commands and InputOutput objects  
>                 io = InputOutput(pretty=False, yes=True)  
>                 coder = MagicMock()  
>                 commands = Commands(io, coder)  
>       
>                 # Call the cmd_add method with 'foo.txt' and 'bar.txt'  
>     >           commands.cmd_add(["foo.txt", "bar.txt"])  
>       
>     /Users/gauthier/Projects/aider/tests/test_commands.py:20:  
>     _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _  
>       
>     self = <aider.commands.Commands object at 0x10b412b50>  
>     args = ['foo.txt', 'bar.txt']  
>       
>         def cmd_add(self, args):  
>             "Add matching files to the chat session"  
>       
>             added_fnames = []  
>             files = self.coder.get_all_relative_files()  
>     >       for word in args.split():  
>     E       AttributeError: 'list' object has no attribute 'split'  
>       
>     /Users/gauthier/Projects/aider/aider/commands.py:161: AttributeError  
>     =========================== short test summary info ============================  
>     FAILED tests/test_commands.py::TestCommands::test_cmd_add - AttributeError: '...  
>     ============================== 1 failed in 0.34s ===============================  
>     
> 
> Add the output to the chat? \[y/n\] (y): y

It seems that the `cmd_add` method in `aider/commands.py` is expecting a string as input, but in the test, we are passing a list. I will update the test to pass a string instead of a list.

Here’s the code change:

    tests/test_commands.py
    <<<<<<< ORIGINAL
                # Call the cmd_add method with 'foo.txt' and 'bar.txt'
                commands.cmd_add(["foo.txt", "bar.txt"])
    =======
                # Call the cmd_add method with 'foo.txt' and 'bar.txt' as a single string
                commands.cmd_add("foo.txt bar.txt")
    >>>>>>> UPDATED
    

Now, run the test again with the updated test method:

    pytest tests/test_commands.py
    

> Applied edit to tests/test\_commands.py  
> Commit d1551b4 aider: Updated test to pass a string instead of a list when calling `cmd_add` method.

#### [](#run-pytest-teststestcommandspy-1)/run pytest tests/test\_commands.py

>     ============================= test session starts ==============================  
>     platform darwin -- Python 3.11.3, pytest-7.3.1, pluggy-1.0.0  
>     rootdir: /Users/gauthier/Projects/aider  
>     collected 1 item  
>       
>     tests/test_commands.py .                                                 [100%]  
>       
>     ============================== 1 passed in 0.38s ===============================  
>

---



## [https://aider.chat/examples/update-docs.html](https://aider.chat/examples/update-docs.html)

[](#automatically-update-docs-with-aider)Automatically update docs with aider
=============================================================================

In this chat transcript, the user asks to automatically update the Usage docs based on the latest version of the main() function in the code.

> $ aider ./README.md aider/main.py  
> Added README.md to the chat  
> Added aider/main.py to the chat

#### [](#the-cmd-line-args-in-main-have-been-updated-update-the-readme-to-accurately-describe-them)the cmd line args in main() have been updated. update the readme to accurately describe them.

    README.md
    <<<<<<< ORIGINAL
    - `--history-file HISTORY_FILE`: Specify the chat input history file (default: .aider.history). Override the default with the environment variable `AIDER_HISTORY_FILE`.
    - `--model MODEL`: Specify the model to use for the main chat (default: gpt-4). Override the default with the environment variable `AIDER_MODEL`.
    - `-3`: Use gpt-3.5-turbo model for the main chat (basically won't work). No environment variable override.
    - `--no-pretty`: Disable pretty, colorized output. Override the default with the environment variable `AIDER_PRETTY` (default: 1 for enabled, 0 for disabled).
    - `--show-diffs`: Show diffs when committing changes (default: False). Override the default with the environment variable `AIDER_SHOW_DIFFS` (default: 0 for False, 1 for True).
    - `--no-auto-commits`: Disable auto commit of changes. Override the default with the environment variable `AIDER_AUTO_COMMITS` (default: 1 for enabled, 0 for disabled).
    =======
    - `--input-history-file INPUT_HISTORY_FILE`: Specify the chat input history file (default: .aider.input.history). Override the default with the environment variable `AIDER_INPUT_HISTORY_FILE`.
    - `--chat-history-file CHAT_HISTORY_FILE`: Specify the chat history file (default: .aider.chat.history.md). Override the default with the environment variable `AIDER_CHAT_HISTORY_FILE`.
    - `--model MODEL`: Specify the model to use for the main chat (default: gpt-4). Override the default with the environment variable `AIDER_MODEL`.
    - `-3`: Use gpt-3.5-turbo model for the main chat (basically won't work). No environment variable override.
    - `--no-pretty`: Disable pretty, colorized output. Override the default with the environment variable `AIDER_PRETTY` (default: 1 for enabled, 0 for disabled).
    - `--apply FILE`: Apply the changes from the given file instead of running the chat (debug).
    - `--no-auto-commits`: Disable auto commit of changes. Override the default with the environment variable `AIDER_AUTO_COMMITS` (default: 1 for enabled, 0 for disabled).
    - `--show-diffs`: Show diffs when committing changes (default: False). Override the default with the environment variable `AIDER_SHOW_DIFFS` (default: 0 for False, 1 for True).
    - `--yes`: Always say yes to every confirmation (default: False).
    >>>>>>> UPDATED
    

> Applied edit to README.md  
> Commit 024f45e aider: Updated command line arguments in main() and updated README.md to accurately describe them.

---



## [https://aider.chat/examples/pong.html](https://aider.chat/examples/pong.html)

[](#build-pong-with-aider-and-pygame)Build pong with aider and pygame.
======================================================================

In this chat transcript, the user asks to make a pong game using pygame. After setting up a basic game, the user asks for some customization of the colors and game mechanics.

> $ aider

#### [](#can-you-make-a-simple-game-of-pong-with-pygame)can you make a simple game of pong with pygame?

Sure, I can help you create a simple Pong game using Pygame. First, let’s break down the steps needed to create the game:

1.  Install Pygame library.
2.  Initialize Pygame and create a game window.
3.  Create Paddle and Ball classes.
4.  Initialize the paddles and the ball.
5.  Create the game loop.
6.  Handle user input for paddle movement.
7.  Update the ball position and check for collisions.
8.  Draw the paddles and ball on the screen.
9.  Check for scoring and update the score.
10.  Display the score on the screen.

Now, let’s start with the code. I’ll provide you with the code changes in an _EDIT BLOCK_. Since we are creating a new file, I’ll name it `pong_game.py`.

    pong_game.py
    <<<<<<< ORIGINAL
    =======
    import pygame
    import sys
    
    # Initialize Pygame
    pygame.init()
    
    # Set up the game window
    screen_width = 640
    screen_height = 480
    screen = pygame.display.set_mode((screen_width, screen_height))
    pygame.display.set_caption("Pong")
    
    # Game loop
    running = True
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False
    
        # Update game objects
    
        # Draw game objects
    
        # Update the display
        pygame.display.flip()
    
    # Quit Pygame
    pygame.quit()
    sys.exit()
    >>>>>>> UPDATED
    

This is the basic structure of the game. Now, let’s add the Paddle and Ball classes, handle user input, update the ball position, draw the objects, and handle scoring. I’ll provide the code changes in the next message.

> Allow creation of new file pong\_game.py? y  
> Add pong\_game.py to git? y  
> Applied edit to pong\_game.py  
> Commit 14799cb aider: Added basic Pygame initialization and game loop structure to `pong_game.py`.

#### [](#go-ahead)go ahead

Now, let’s add the Paddle and Ball classes, handle user input, update the ball position, draw the objects, and handle scoring. I’ll provide the code changes in an _EDIT BLOCK_.

    pong_game.py
    <<<<<<< ORIGINAL
    import pygame
    import sys
    
    # Initialize Pygame
    pygame.init()
    
    # Set up the game window
    screen_width = 640
    screen_height = 480
    screen = pygame.display.set_mode((screen_width, screen_height))
    pygame.display.set_caption("Pong")
    =======
    import pygame
    import sys
    import random
    
    # Initialize Pygame
    pygame.init()
    
    # Set up the game window
    screen_width = 640
    screen_height = 480
    screen = pygame.display.set_mode((screen_width, screen_height))
    pygame.display.set_caption("Pong")
    
    # Paddle and Ball classes
    class Paddle(pygame.sprite.Sprite):
        def __init__(self, x, y):
            super().__init__()
            self.width = 10
            self.height = 60
            self.image = pygame.Surface((self.width, self.height))
            self.image.fill((255, 255, 255))
            self.rect = self.image.get_rect()
            self.rect.x = x
            self.rect.y = y
    
        def move(self, dy):
            if self.rect.y + dy >= 0 and self.rect.y + dy <= screen_height - self.height:
                self.rect.y += dy
    
    class Ball(pygame.sprite.Sprite):
        def __init__(self):
            super().__init__()
            self.width = 10
            self.height = 10
            self.image = pygame.Surface((self.width, self.height))
            self.image.fill((255, 255, 255))
            self.rect = self.image.get_rect()
            self.rect.x = screen_width // 2 - self.width // 2
            self.rect.y = screen_height // 2 - self.height // 2
            self.dx = random.choice([-1, 1]) * 4
            self.dy = random.choice([-1, 1]) * 4
    
        def update(self):
            self.rect.x += self.dx
            self.rect.y += self.dy
    
            # Collision with top and bottom
            if self.rect.y <= 0 or self.rect.y >= screen_height - self.height:
                self.dy = -self.dy
    
            # Scoring
            if self.rect.x <= 0 or self.rect.x >= screen_width - self.width:
                self.reset()
    
        def reset(self):
            self.rect.x = screen_width // 2 - self.width // 2
            self.rect.y = screen_height // 2 - self.height // 2
            self.dx = random.choice([-1, 1]) * 4
            self.dy = random.choice([-1, 1]) * 4
    
        def collide_with(self, paddle):
            if self.rect.colliderect(paddle.rect):
                self.dx = -self.dx
    >>>>>>> UPDATED
    

Now, let’s initialize the paddles and the ball, handle user input, update the ball position, draw the objects, and handle scoring.

    pong_game.py
    <<<<<<< ORIGINAL
    # Game loop
    running = True
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False
    
        # Update game objects
    
        # Draw game objects
    
        # Update the display
        pygame.display.flip()
    =======
    # Initialize paddles and ball
    left_paddle = Paddle(10, screen_height // 2 - 30)
    right_paddle = Paddle(screen_width - 20, screen_height // 2 - 30)
    ball = Ball()
    
    # Game loop
    running = True
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False
    
        # Handle user input
        keys = pygame.key.get_pressed()
        if keys[pygame.K_w]:
            left_paddle.move(-5)
        if keys[pygame.K_s]:
            left_paddle.move(5)
        if keys[pygame.K_UP]:
            right_paddle.move(-5)
        if keys[pygame.K_DOWN]:
            right_paddle.move(5)
    
        # Update game objects
        ball.update()
        ball.collide_with(left_paddle)
        ball.collide_with(right_paddle)
    
        # Draw game objects
        screen.fill((0, 0, 0))
        screen.blit(left_paddle.image, left_paddle.rect)
        screen.blit(right_paddle.image, right_paddle.rect)
        screen.blit(ball.image, ball.rect)
    
        # Update the display
        pygame.display.flip()
        pygame.time.delay(16)
    >>>>>>> UPDATED
    

Now, you should have a simple Pong game using Pygame. You can further improve the game by adding a scoring system and displaying the score on the screen.

> Applied edit to pong\_game.py  
> Applied edit to pong\_game.py  
> Commit b20bcee aider: Added Paddle and Ball classes, handled user input, updated ball position, drew objects, and handled scoring.

#### [](#nice-it-works-but-the-ball-moves-way-too-fast)nice, it works. but the ball moves way too fast.

I’m glad it works! Let’s slow down the ball by reducing its speed. We can do this by changing the values of `self.dx` and `self.dy` in the `Ball` class.

    pong_game.py
    <<<<<<< ORIGINAL
            self.dx = random.choice([-1, 1]) * 4
            self.dy = random.choice([-1, 1]) * 4
    =======
            self.dx = random.choice([-1, 1]) * 2
            self.dy = random.choice([-1, 1]) * 2
    >>>>>>> UPDATED
    

This change will reduce the ball’s speed by half. You can adjust the values further if you want the ball to move even slower.

> Applied edit to pong\_game.py  
> Commit f4ceed4 aider: Reduced ball speed by half.

#### [](#can-you-make-the-paddles-a-bit-bigger-and-make-one-paddle-red-and-one-blue)can you make the paddles a bit bigger? and make one paddle red and one blue?

Sure, let’s make the paddles bigger and change their colors. We can do this by modifying the `Paddle` class in the `pong_game.py` file.

    pong_game.py
    <<<<<<< ORIGINAL
            self.width = 10
            self.height = 60
            self.image = pygame.Surface((self.width, self.height))
            self.image.fill((255, 255, 255))
    =======
            self.width = 15
            self.height = 80
            self.image = pygame.Surface((self.width, self.height))
            self.color = (255, 255, 255) if x < screen_width // 2 else (0, 0, 255)
            self.image.fill(self.color)
    >>>>>>> UPDATED
    

Now, let’s change the color of the left paddle to red.

    pong_game.py
    <<<<<<< ORIGINAL
    left_paddle = Paddle(10, screen_height // 2 - 30)
    =======
    left_paddle = Paddle(10, screen_height // 2 - 40)
    left_paddle.color = (255, 0, 0)
    left_paddle.image.fill(left_paddle.color)
    >>>>>>> UPDATED
    

With these changes, the paddles will be larger, and the left paddle will be red while the right paddle will be blue.

> Applied edit to pong\_game.py  
> Applied edit to pong\_game.py  
> Commit 2c645c9 aider: Changed paddle size and color, and set left paddle to red.

#### [](#each-time-the-ball-bounces-off-the-paddle-can-you-make-it-go-10-faster)each time the ball bounces off the paddle, can you make it go 10% faster?

Sure, let’s increase the ball’s speed by 10% each time it bounces off a paddle. We can do this by modifying the `collide_with` method in the `Ball` class.

    pong_game.py
    <<<<<<< ORIGINAL
        def collide_with(self, paddle):
            if self.rect.colliderect(paddle.rect):
                self.dx = -self.dx
    =======
        def collide_with(self, paddle):
            if self.rect.colliderect(paddle.rect):
                self.dx = -self.dx * 1.1
                self.dy *= 1.1
    >>>>>>> UPDATED
    

With this change, the ball’s speed will increase by 10% in both the x and y directions each time it bounces off a paddle.

> Applied edit to pong\_game.py  
> Commit 693faf4 aider: Increased ball speed by 10% in both x and y directions each time it bounces off a paddle.

---



## [https://aider.chat/examples/css-exercises.html](https://aider.chat/examples/css-exercises.html)

[](#complete-a-css-exercise-with-aider)Complete a css exercise with aider
=========================================================================

In this chat transcript, the user asks about the open source [CSS Exercises repo](https://github.com/TheOdinProject/css-exercises) and completes an animation exercise.

> $ aider

#### [](#what-is-this-repo)what is this repo?

Based on the file list provided, it seems like this repository contains a collection of CSS and HTML exercises, solutions, and examples. The exercises cover various topics such as Flexbox, Grid, Animation, Foundations, and Margin & Padding. The repository also includes images and other assets used in the exercises.

#### [](#add-animation03-dropdown-menureadmemd)/add animation/03-dropdown-menu/README.md

> Added animation/03-dropdown-menu/README.md to the chat

Yes, I see the content of the `animation/03-dropdown-menu/README.md` file. It describes an exercise to add animation to a dropdown menu, creating a bounce illusion when the dropdown expands close to its final end state. The desired outcome is shown in a GIF file, and the hints provided suggest using the `transform-origin` property and adding an intermediate step to the keyframe at-rule to achieve the bounce effect.

Is there any specific change or improvement you would like me to make to this file or any other file in the repository?

#### [](#can-you-make-the-changes-suggested-in-the-readme)can you make the changes suggested in the readme?

To make the changes suggested in the `animation/03-dropdown-menu/README.md`, I need to see the contents of the following files:

1.  `animation/03-dropdown-menu/style.css`
2.  `animation/03-dropdown-menu/script.js`

Please provide the contents of these files so I can suggest the necessary changes.

> animation/03-dropdown-menu/style.css  
> animation/03-dropdown-menu/script.js  
> Add these files to the chat? y

Apologies for the oversight. I see the content of the `animation/03-dropdown-menu/style.css` and `animation/03-dropdown-menu/script.js` files now. I will suggest the necessary changes to add the bounce animation to the dropdown menu.

    animation/03-dropdown-menu/style.css
    <<<<<<< ORIGINAL
    .visible {
      display: block;
    }
    =======
    .visible {
      display: block;
      animation: expand 0.3s ease-out;
      transform-origin: top;
    }
    
    @keyframes expand {
      0% {
        transform: scaleY(0);
      }
      80% {
        transform: scaleY(1.1);
      }
      100% {
        transform: scaleY(1);
      }
    }
    >>>>>>> UPDATED
    

These changes add the bounce animation to the dropdown menu by creating a new keyframe animation called `expand`. The `transform-origin` property is set to `top` to make the dropdown menu start transforming from the top. The intermediate step at 80% of the animation creates the bounce illusion.

> Applied edit to animation/03-dropdown-menu/style.css  
> Commit bb3a813 aider: Added bounce animation to dropdown menu.

#### [](#that-worked)that worked!

I’m glad the changes worked for you! If you have any more requests or need assistance with other parts of the code, feel free to ask. I’m here to help!

---



## [https://aider.chat/examples/census.html](https://aider.chat/examples/census.html)

[](#download-analyze-and-plot-us-census-data)Download, analyze and plot US Census data
======================================================================================

Inspired by [Ethan Mollick’s recent blog article about ChatGPT plugins](https://www.oneusefulthing.org/p/it-is-starting-to-get-strange), I used `aider` and GPT-4 to do data analysis of some US Census data. I asked aider how to download census data and to suggest some hypotheses to test. I asked it to write the code to get the data, test one of the hypotheses and provide a summary and plot of the results.

> $ aider  
> Using git repo: .git

#### [](#what-is-a-good-basic-us-census-dataset-to-analyze-for-interesting-patterns)what is a good basic us census dataset to analyze for interesting patterns?

A good basic US Census dataset to analyze for interesting patterns is the American Community Survey (ACS) dataset. The ACS is an ongoing survey conducted by the US Census Bureau that provides vital information on a yearly basis about the US population and its characteristics. The dataset includes information on demographics, social, economic, and housing characteristics.

You can find the ACS dataset on the US Census Bureau’s website: https://www.census.gov/programs-surveys/acs/data.html

Some interesting patterns to analyze in the ACS dataset could include:

1.  Population growth and decline in different regions.
2.  Changes in racial and ethnic composition.
3.  Income inequality and poverty levels.
4.  Educational attainment and its relationship with income.
5.  Housing affordability and homeownership rates.

Remember to consider the dataset’s documentation and guidelines to understand the data and its limitations.

#### [](#do-you-know-how-to-download-american-community-survey-data)do you know how to download American Community Survey data?

Yes, I can guide you on how to download American Community Survey (ACS) data. You can use the Census Bureau’s API to access the data. To do this, you’ll need an API key, which you can obtain from the Census Bureau’s website.

Here’s a Python example using the `requests` library to download ACS data:

1.  Install the `requests` library if you haven’t already:

    pip install requests
    

1.  Use the following code to download ACS data:

    import requests
    
    # Replace 'your_api_key' with your actual API key
    api_key = 'your_api_key'
    
    # Define the API endpoint and parameters
    url = 'https://api.census.gov/data/2019/acs/acs5'
    params = {
        'get': 'NAME,B01001_001E',  # Variables to retrieve (NAME: Geographic area name, B01001_001E: Total population)
        'for': 'state:*',  # Geographic area (all states)
        'key': api_key
    }
    
    # Send the request and parse the response
    response = requests.get(url, params=params)
    data = response.json()
    
    # Print the data
    for row in data:
        print(row)
    

Replace `'your_api_key'` with the API key you obtained from the Census Bureau’s website. This example retrieves the total population (variable `B01001_001E`) for all states. You can modify the `get` and `for` parameters to download different variables and geographic areas.

For more information on available variables and geographic areas, refer to the ACS documentation:

*   Variables: https://api.census.gov/data/2019/acs/acs5/variables.html
*   Geographic Areas: https://api.census.gov/data/2019/acs/acs5/geography.html

#### [](#how-do-i-get-an-api-key)how do i get an api key?

To obtain an API key from the Census Bureau, follow these steps:

1.  Go to the Census Bureau’s API key request page: https://api.census.gov/data/key\_signup.html
    
2.  Fill out the form with your name, email address, organization (if applicable), and a brief description of your intended use of the API.
    
3.  Click the “Request Key” button.
    
4.  You will receive an email containing your API key. It may take a few minutes for the email to arrive. Make sure to check your spam folder if you don’t see it in your inbox.
    

Once you have your API key, you can use it in your Python code to access the American Community Survey data, as shown in the previous example. Replace `'your_api_key'` with the API key you received in the email.

#### [](#please-save-your-download-script-as-getdatapy)please save your download script as `getdata.py`

Here’s the `getdata.py` file with the download script:

    new_file/getdata.py
    <<<<<<< ORIGINAL
    =======
    import requests
    
    # Replace 'your_api_key' with your actual API key
    api_key = 'your_api_key'
    
    # Define the API endpoint and parameters
    url = 'https://api.census.gov/data/2019/acs/acs5'
    params = {
        'get': 'NAME,B01001_001E',  # Variables to retrieve (NAME: Geographic area name, B01001_001E: Total population)
        'for': 'state:*',  # Geographic area (all states)
        'key': api_key
    }
    
    # Send the request and parse the response
    response = requests.get(url, params=params)
    data = response.json()
    
    # Print the data
    for row in data:
        print(row)
    >>>>>>> UPDATED
    

Save this code in a new file named `getdata.py`. Remember to replace `'your_api_key'` with your actual API key obtained from the Census Bureau.

> Allow creation of new file new\_file/getdata.py? y  
> Add new\_file/getdata.py to git? y  
> Applied edit to new\_file/getdata.py  
> Commit afcb9d1 aider: Added `getdata.py` file with download script.

#### [](#add-my-api-key-4ae31ed2a0f0dd62609e51cd95deadbeefe7774f)add my api key: 4ae31ed2a0f0dd62609e51cd95deadbeefe7774f

I will update the API key in the file.

    new_file/getdata.py
    <<<<<<< ORIGINAL
    api_key = 'your_api_key'
    =======
    api_key = '4ae31ed2a0f0dd62609e51cd95deadbeefe7774f'
    >>>>>>> UPDATED
    

> Applied edit to new\_file/getdata.py  
> Commit 1d8b4a6 aider: Updated the API key in new\_file/getdata.py.

#### [](#what-are-some-interesting-hypothesis-that-you-might-be-able-to-test-using-acs-data)what are some interesting hypothesis that you might be able to test using ACS data?

Here are some interesting hypotheses that you can test using ACS (American Community Survey) data:

1.  Relationship between income and education level: Higher education levels lead to higher income.
2.  Impact of population density on housing prices: Higher population density areas have higher housing prices.
3.  Relationship between employment rate and crime rate: Higher employment rates lead to lower crime rates.
4.  Effect of public transportation availability on car ownership: Areas with better public transportation have lower car ownership rates.
5.  Relationship between age distribution and healthcare facilities: Areas with a higher percentage of elderly population have more healthcare facilities.

These are just a few examples. ACS data provides a wealth of information on various demographic, social, economic, and housing characteristics, allowing you to explore many different hypotheses.

#### [](#can-you-download-the-data-to-test-2-impact-of-population-density-on-housing-prices-higher-population-density-areas-have-higher-housing-prices)can you download the data to test #2 Impact of population density on housing prices: Higher population density areas have higher housing prices.

As an AI language model, I cannot directly download or access data. However, I can help you with the code to download the required data for testing hypothesis #2 using the ACS data.

To test the hypothesis, you’ll need to obtain population density and housing price data. You can use the following ACS variables:

*   B01003\_001E: Total population
*   B25077\_001E: Median value of owner-occupied housing units

Here’s the updated code to fetch the required data:

    new_file/getdata.py
    <<<<<<< ORIGINAL
        'get': 'NAME,B01001_001E',  # Variables to retrieve (NAME: Geographic area name, B01001_001E: Total population)
    =======
        'get': 'NAME,B01003_001E,B25077_001E',  # Variables to retrieve (NAME: Geographic area name, B01003_001E: Total population, B25077_001E: Median value of owner-occupied housing units)
    >>>>>>> UPDATED
    

After running the updated code, you’ll have the population and housing price data for each geographic area. You can then analyze the data to test the hypothesis.

> Applied edit to new\_file/getdata.py  
> Commit 81549ab aider: Updated code to fetch population and housing price data for testing hypothesis #2.

#### [](#instead-of-printing-all-the-data-print-a-summary-table-that-shows-whether-the-data-supports-the-hypothesis)instead of printing all the data, print a summary table that shows whether the data supports the hypothesis

To print a summary table, you can use the pandas library to analyze the data and calculate the correlation between population density and housing prices. Here’s how to modify the code:

1.  Import pandas.
2.  Convert the JSON data to a pandas DataFrame.
3.  Calculate the correlation between population density and housing prices.
4.  Print the correlation as a summary table.

Here are the changes to the code:

    new_file/getdata.py
    <<<<<<< ORIGINAL
    import requests
    =======
    import requests
    import pandas as pd
    >>>>>>> UPDATED
    

    new_file/getdata.py
    <<<<<<< ORIGINAL
    data = response.json()
    =======
    data = response.json()
    # Convert the JSON data to a pandas DataFrame
    df = pd.DataFrame(data[1:], columns=data[0])
    df[['B01003_001E', 'B25077_001E']] = df[['B01003_001E', 'B25077_001E']].apply(pd.to_numeric)
    >>>>>>> UPDATED
    

    new_file/getdata.py
    <<<<<<< ORIGINAL
    for row in data:
        print(row)
    =======
    # Calculate the correlation between population density and housing prices
    correlation = df['B01003_001E'].corr(df['B25077_001E'])
    
    # Print the correlation as a summary table
    print("Summary Table:")
    print("Correlation between population density and housing prices:", correlation)
    >>>>>>> UPDATED
    

After applying these changes, the code will print a summary table showing the correlation between population density and housing prices. A positive correlation value indicates that higher population density areas have higher housing prices, supporting the hypothesis.

> Applied edit to new\_file/getdata.py  
> Applied edit to new\_file/getdata.py  
> Applied edit to new\_file/getdata.py  
> Commit 2f4fcd4 aider: Added pandas library to analyze data and calculate correlation between population density and housing prices, and printed the correlation as a summary table.

#### [](#run-python3-newfilegetdatapy)/run python3 new\_file/getdata.py

>     Summary Table:  
>     Correlation between population density and housing prices: 0.16020298445808737  
>     
> 
> Add the output to the chat? y

Great! The script seems to be working as expected. The correlation between population density and housing prices is 0.1602. If you need any further assistance or modifications to the code, please let me know.

#### [](#can-you-also-plot-a-graph-which-would-show-any-correlation)can you also plot a graph which would show any correlation?

To plot a graph showing the correlation between population density and housing prices, we’ll need to modify the `new_file/getdata.py` file. We’ll use the `matplotlib` library to create the plot. If you don’t have it installed, you can install it using `pip install matplotlib`.

Here are the changes to make:

1.  Import the `matplotlib.pyplot` module.
2.  Create a scatter plot of population density (x-axis) and housing prices (y-axis).
3.  Add labels to the axes and a title to the plot.
4.  Display the plot.

Here’s the updated code:

    new_file/getdata.py
    <<<<<<< ORIGINAL
    import requests
    import pandas as pd
    =======
    import requests
    import pandas as pd
    import matplotlib.pyplot as plt
    >>>>>>> UPDATED
    
    ...
    
    new_file/getdata.py
    <<<<<<< ORIGINAL
    print("Summary Table:")
    print("Correlation between population density and housing prices:", correlation)
    =======
    print("Summary Table:")
    print("Correlation between population density and housing prices:", correlation)
    
    # Create a scatter plot of population density and housing prices
    plt.scatter(df['B01003_001E'], df['B25077_001E'])
    plt.xlabel('Population Density')
    plt.ylabel('Housing Prices')
    plt.title('Correlation between Population Density and Housing Prices')
    plt.show()
    >>>>>>> UPDATED
    

This will create a scatter plot of population density and housing prices, which will help visualize the correlation between the two variables.

> Applied edit to new\_file/getdata.py  
> Applied edit to new\_file/getdata.py  
> Commit 9ff3666 aider: Added scatter plot of population density and housing prices to visualize correlation.

---



## [https://aider.chat/examples/asciinema.html](https://aider.chat/examples/asciinema.html)

[](#editing-an-asciinema-cast-file-with-aider)Editing an asciinema cast file with aider
=======================================================================================

The user needs to make some tedious edits to the escape sequences in an `asciinema` screencast file.

> $ aider hello.cast  
> Added hello.cast to the chat

#### [](#when-the-hellopy--prompt-is-displayed-its-including-some-escape-codes-to-add-a-few-blank-lines-below-the-prompt-and-then-bringing-the-cursor-back-up-remove-all-that-just-show-the-prompt-followed-by-a-space-and-leave-the-cursor-showing-right-after-that)when the “hello.py> “ prompt is displayed, it’s including some escape codes to add a few blank lines below the prompt and then bringing the cursor back up. remove all that. just show the prompt followed by a space and leave the cursor showing right after that.

    hello.cast
    <<<<<<< ORIGINAL
    [19.534013, "o", "\u001b[?2004h\u001b[?1l\u001b[?25l\u001b[0m\u001b[?7l\u001b[0m\u001b[J\u001b[0;38;5;28mhello.py>  \u001b[0m\r\r\n\r\r\n\r\r\n\u001b[0;38;5;28m                                                                \r\u001b[64C \r\u001b[3A\u001b[10C\u001b[?7h\u001b[0m\u001b[?12l\u001b[?25h"]
    =======
    [19.534013, "o", "\u001b[?2004h\u001b[?1l\u001b[?25l\u001b[0m\u001b[?7l\u001b[0m\u001b[J\u001b[0;38;5;28mhello.py> \u001b[0m\u001b[?7h\u001b[0m\u001b[?12l\u001b[?25h"]
    >>>>>>> UPDATED
    

> Applied edit to hello.cast  
> Commit a3fa4d2 aider: Removed escape codes to display prompt and cursor correctly.

---



## [https://aider.chat/examples/hello.html](https://aider.chat/examples/hello.html)

[](#hello-aider)Hello aider!
============================

Here is the simplest possible “hello world” example of using aider:

  
  
  

#### [](#change-hello-to-goodbye)change hello to goodbye

To change the output from “hello” to “goodbye”, we need to modify the `hello.py` file.

Here is the change:

    hello.py
    <<<<<<< ORIGINAL
    print("hello")
    =======
    print("goodbye")
    >>>>>>> UPDATED
    

> Applied edit to hello.py  
> Commit 672ae42 aider: Changed output from “hello” to “goodbye” in hello.py.

---



## [https://aider.chat/examples/no-color.html](https://aider.chat/examples/no-color.html)

[](#honor-the-no_color-environment-variable)Honor the NO\_COLOR environment variable
====================================================================================

The user pastes the specification of the NO\_COLOR environment variable protocol from [no-color.org](https://no-color.org) into the aider chat.

Aider figures out which files need to be edited, and asks permission to make changes. It then disables all the color and pretty-printing functions if NO\_COLOR is set, so the tool conforms to the specification.

The user then asks for a test case, which aider adds as well.

> $ aider  
> Using git repo: .git  
> Use /help to see in-chat commands.

#### [](#command-line-software-which-adds-ansi-color-to-its-output-by-default-should-check-for-a-nocolor-environment-variable-that-when-present-and-not-an-empty-string-regardless-of-its-value-prevents-the-addition-of-ansi-color)Command-line software which adds ANSI color to its output by default should check for a NO\_COLOR environment variable that, when present and not an empty string (regardless of its value), prevents the addition of ANSI color.

To implement this feature, we need to modify the `aider/io.py` file. Please make it _read-write_ so I can provide the necessary changes.

> aider/io.py  
> Add these files to the chat? y

Great! Now, I will make the necessary changes to check for the `NO_COLOR` environment variable and disable ANSI color when it is present and not an empty string.

    aider/io.py
    <<<<<<< ORIGINAL
    import os
    =======
    import os
    import os.path
    >>>>>>> UPDATED
    

    aider/io.py
    <<<<<<< ORIGINAL
        def __init__(
            self,
            pretty=True,
            yes=False,
            input_history_file=None,
            chat_history_file=None,
            input=None,
            output=None,
            user_input_color="blue",
            tool_output_color=None,
            tool_error_color="red",
        ):
            self.user_input_color = user_input_color
            self.tool_output_color = tool_output_color
            self.tool_error_color = tool_error_color
            self.input = input
            self.output = output
            self.pretty = pretty
            self.yes = yes
            self.input_history_file = input_history_file
            if chat_history_file is not None:
                self.chat_history_file = Path(chat_history_file)
            else:
                self.chat_history_file = None
    
            if pretty:
                self.console = Console()
            else:
                self.console = Console(force_terminal=True, no_color=True)
    =======
        def __init__(
            self,
            pretty=True,
            yes=False,
            input_history_file=None,
            chat_history_file=None,
            input=None,
            output=None,
            user_input_color="blue",
            tool_output_color=None,
            tool_error_color="red",
        ):
            no_color = os.environ.get("NO_COLOR")
            if no_color is not None and no_color != "":
                pretty = False
    
            self.user_input_color = user_input_color if pretty else None
            self.tool_output_color = tool_output_color if pretty else None
            self.tool_error_color = tool_error_color if pretty else None
            self.input = input
            self.output = output
            self.pretty = pretty
            self.yes = yes
            self.input_history_file = input_history_file
            if chat_history_file is not None:
                self.chat_history_file = Path(chat_history_file)
            else:
                self.chat_history_file = None
    
            self.console = Console(force_terminal=not pretty, no_color=not pretty)
    >>>>>>> UPDATED
    

These changes will make the software check for the `NO_COLOR` environment variable and disable ANSI color when it is present and not an empty string.

> Applied edit to aider/io.py  
> Applied edit to aider/io.py  
> Commit 3218242 aider: Added check for NO\_COLOR environment variable to disable ANSI color.

#### [](#add-a-test)add a test

To add a test for the `NO_COLOR` environment variable, we will create a new test function in the `tests/test_io.py` file. Since this file does not exist, we will create it first.

    tests/test_io.py
    <<<<<<< ORIGINAL
    =======
    import os
    import unittest
    from unittest.mock import patch
    from aider.io import InputOutput
    
    class TestInputOutput(unittest.TestCase):
        def test_no_color_environment_variable(self):
            with patch.dict(os.environ, {"NO_COLOR": "1"}):
                io = InputOutput()
                self.assertFalse(io.pretty)
    
    if __name__ == "__main__":
        unittest.main()
    >>>>>>> UPDATED
    

This test function checks if the `pretty` attribute of the `InputOutput` class is set to `False` when the `NO_COLOR` environment variable is set.

> Allow creation of new file tests/test\_io.py? y  
> Add tests/test\_io.py to git? y  
> Applied edit to tests/test\_io.py  
> Commit 52a9df5 aider: Added a test function to check if the `pretty` attribute of the `InputOutput` class is set to `False` when the `NO_COLOR` environment variable is set.

#### [](#run-pytest)/run pytest

> \============================= test session starts ==============================  
> platform darwin – Python 3.11.3, pytest-7.3.1, pluggy-1.0.0  
> rootdir: /Users/gauthier/Projects/aider  
> collected 25 items
> 
> tests/test\_coder.py …… \[ 24%\]  
> tests/test\_commands.py . \[ 28%\]  
> tests/test\_io.py . \[ 32%\]  
> tests/test\_main.py …. \[ 48%\]  
> tests/test\_repomap.py … \[ 60%\]  
> tests/test\_utils.py ………. \[100%\]
> 
> \============================== 25 passed in 1.41s ==============================
> 
> Add the output to the chat? y

---



## [https://aider.chat/examples/chat-transcript-css.html](https://aider.chat/examples/chat-transcript-css.html)

[](#improve-css-styling-of-chat-transcripts)Improve css styling of chat transcripts
===================================================================================

> $ aider index.html assets/css/style.css  
> Added index.html to the chat  
> Added assets/css/style.css to the chat

#### [](#add-a-rounded-border-to-all-sides-of-the-boxquote)add a rounded border to all sides of the boxquote

    assets/css/style.css
    <<<<<<< ORIGINAL
    .main-content blockquote{padding:0 1rem;margin-left:0;color:#819198;border-left:0.3rem solid #dce6f0}
    =======
    .main-content blockquote{
      padding: 0 1rem;
      margin
    

> ^C KeyboardInterrupt  
> ^C again to quit

#### [](#make-all-the-edits-to-the-embedded-style-tag-in-the-html)make all the edits to the embedded style tag in the html

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border-left-color: #159957;
          }
          .btn {
            display: inline-block;
            width: auto;
          }
          .btn + .btn {
            margin-top: 0;
          }
        </style>
    =======
        <style>
          .main-content blockquote {
            border-left-color: #159957;
            border: 0.3rem solid #dce6f0;
            border-radius: 0.5rem;
          }
          .btn {
            display: inline-block;
            width: auto;
          }
          .btn + .btn {
            margin-top: 0;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit e7a5cb5 aider: Added rounded border to all sides of the boxquote.

#### [](#make-the-blockquote-font-color-the-same-as-the-p-color)make the blockquote font color the same as the p color

> Git repo has uncommitted changes.  
> Commit before the chat proceeds \[y/n/commit message\]? Added note about missing method and incorrect method calls in index.html.  
> Commit 2d31f5b Added note about missing method and incorrect method calls in index.html.

    assets/css/style.css
    <<<<<<< ORIGINAL
    .main-content blockquote{padding:0 1rem;margin-left:0;color:#819198;border-left
    

> ^C KeyboardInterrupt

#### [](#only-edit-indexhtml)only edit index.html

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
          }
          .btn {
            display: inline-block;
            width: auto;
          }
          .btn + .btn {
            margin-top: 0;
          }
        </style>
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            color: #606c71;
          }
          .btn {
            display: inline-block;
            width: auto;
          }
          .btn + .btn {
            margin-top: 0;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit 8645217 aider: Changed blockquote font color to match <p> color in index.html.

#### [](#make-the-blockquote-background-a-lighter-shade-of-the-same-green-as-the-border)make the blockquote background a lighter shade of the same green as the border

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
          }
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
          }
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit 57b7b10 aider: Changed blockquote background color to a lighter shade of green.

#### [](#add-some-space-inside-the-border-of-the-blockquote)add some space inside the border of the blockquote

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
          }
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 1rem;
          }
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit dd7dcb6 aider: Added padding inside the border of the blockquote.

#### [](#can-we-add-a-label-aider-along-the-top-of-the-blockquote-box-only-using-style)can we add a label “aider” along the top of the blockquote box only using style

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 1rem;
          }
        </style>
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 1rem;
            position: relative;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -0.5rem;
            left: 1rem;
            background-color: #e0f2ef;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #159957;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit 0b0e332 aider: Added label “aider” to the top of the blockquote box using style.

#### [](#add-more-padding-on-the-top-of-the-box-and-bring-the-label-into-the-box-so-it-doesnt-intersect-the-border)add more padding on the top of the box and bring the label into the box so it doesn’t intersect the border

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 1rem;
            position: relative;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -0.5rem;
            left: 1rem;
            background-color: #e0f2ef;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #159957;
          }
        </style>
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 1.5rem 1rem 1rem 1rem;
            position: relative;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: 0.5rem;
            left: 1rem;
            background-color: #e0f2ef;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #159957;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit eee902e aider: Added more padding on the top of the box and brought the label into the box so it doesn’t intersect the border.

#### [](#change-all-the-blockquote-colors-to-be-shades-of-blue-instead-of-green-choose-the-blue-based-on-the-blue-in-the-header-gradient)change all the blockquote colors to be shades of blue instead of green. choose the blue based on the blue in the header gradient

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #159957;
            border-radius: 0.5rem;
            background-color: #e0f2ef;
            padding: 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -1.75rem;
            left: -0.5rem;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #159957;
          }
        </style>
    =======
        <style>
          .main-content blockquote {
            border: 0.1rem solid #155799;
            border-radius: 0.5rem;
            background-color: #e0ecf4;
            padding: 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -1.75rem;
            left: -0.5rem;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #155799;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit a26c135 aider: Changed blockquote colors to shades of blue based on the blue in the header gradient.

#### [](#can-you-style-the-aider-label-on-the-blockquote-as-a-tab-that-docks-onto-the-top-of-the-box)can you style the “aider” label on the blockquote as a “tab” that docks onto the top of the box?

    index.html
    <<<<<<< ORIGINAL
          .main-content blockquote {
            border: 0.1rem solid #155799;
            border-radius: 0.5rem;
            background-color: #e0ecf4;
            padding: 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -1.75rem;
            left: -0.5rem;
            padding: 0 0.5rem;
            font-weight: bold;
            color: #155799;
          }
    =======
          .main-content blockquote {
            border: 0.1rem solid #155799;
            border-radius: 0.5rem;
            background-color: #e0ecf4;
            padding: 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -0.5rem;
            left: 0;
            padding: 0.25rem 0.5rem;
            font-weight: bold;
            color: #155799;
            background-color: #e0ecf4;
            border-top-left-radius: 0.5rem;
            border-top-right-radius: 0.5rem;
            border: 0.1rem solid #155799;
            border-bottom: none;
          }
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit 292eda3 aider: Styled the “aider” label on the blockquote as a “tab” that docks onto the top of the box.

#### [](#apply-the-same-box-around-the-h4-element)apply the same box around the h4 element

    index.html
    <<<<<<< ORIGINAL
        <style>
          .main-content blockquote {
            border: 0.1rem solid #155799;
            border-radius: 0.5rem;
            background-color: #e0ecf4;
            padding: 1.25rem 0.75rem 0.75rem 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -1rem;
            left: 0.5;
            padding: 0rem 0.5rem;
            font-weight: bold;
            color: #155799;
            background-color: #e0ecf4;
            border: 0.05rem solid #155799;
            border-radius: 0.5rem;
          }
        </style>
    =======
        <style>
          .main-content blockquote, .main-content h4 {
            border: 0.1rem solid #155799;
            border-radius: 0.5rem;
            background-color: #e0ecf4;
            padding: 1.25rem 0.75rem 0.75rem 0.75rem;
            position: relative;
            margin-top: 2rem;
          }
          .main-content blockquote::before {
            content: "aider";
            display: inline-block;
            position: absolute;
            top: -1rem;
            left: 0.5;
            padding: 0rem 0.5rem;
            font-weight: bold;
            color: #155799;
            background-color: #e0ecf4;
            border: 0.05rem solid #155799;
            border-radius: 0.5rem;
          }
        </style>
    >>>>>>> UPDATED
    

> Applied edit to index.html  
> Commit 6a8cd27 aider: Added box around h4 element.

---



## [https://aider.chat/examples/semantic-search-replace.html](https://aider.chat/examples/semantic-search-replace.html)

[](#semantic-search--replace-code-with-aider)Semantic search & replace code with aider
======================================================================================

In this chat transcript, the user asks to modify a series of function calls.

Notice that it isn’t replacing exact strings. Making the change requires dealing with various formatting and semantic differences in the calls that it is updating.

Some edits were elided from this transcript for brevity.

> $ aider aider/coder.py  
> Added aider/coder.py to the chat

#### [](#replace-all-the-selfconsoleprint-calls-that-contain-red-with-calls-to-selfiotoolerror-with-red-removed-from-the-string)replace all the self.console.print() calls that contain \[red\] with calls to self.io.tool\_error() with \[red\] removed from the string

    aider/coder.py
    <<<<<<< ORIGINAL
                self.console.print(
                    f"[red]This tool will almost certainly fail to work with {main_model}"
                )
    =======
                self.io.tool_error(f"This tool will almost certainly fail to work with {main_model}")
    >>>>>>> UPDATED
    

    aider/coder.py
    <<<<<<< ORIGINAL
                self.console.print("[red]Files are not in a git repo.")
    =======
                self.io.tool_error("Files are not in a git repo.")
    >>>>>>> UPDATED
    

    aider/coder.py
    <<<<<<< ORIGINAL
                self.console.print("[red]Malformed ORIGINAL/UPDATE blocks, retrying...")
                self.console.print("[red]", Text(err))
    =======
                self.io.tool_error("Malformed ORIGINAL/UPDATE blocks, retrying...")
                self.io.tool_error(Text(err))
    >>>>>>> UPDATED
    

Please note that I couldn’t find the `self.io.tool_error()` method in the provided code. You may need to create this method in the appropriate class or provide the correct method name to replace the `self.console.print()` calls.

> Applied edit to aider/coder.py  
> Applied edit to aider/coder.py  
> Applied edit to aider/coder.py  
> Commit 919cfc2 aider: Replaced all self.console.print() calls with self.io.tool\_error() calls with \[red\] removed from the string.

---



## [https://aider.chat/docs/more-info.html](https://aider.chat/docs/more-info.html)

[](#more-info)More info
=======================

See below for more info about aider, including some advanced topics.

* * *

Table of contents
-----------------

*   [Git integration](/docs/git.html)
*   [Supported languages](/docs/languages.html)
*   [Repository map](/docs/repomap.html)
*   [Scripting aider](/docs/scripting.html)
*   [Infinite output](/docs/more/infinite-output.html)
*   [Edit formats](/docs/more/edit-formats.html)
*   [Analytics](/docs/more/analytics.html)
*   [Privacy policy](/docs/legal/privacy.html)

---



## [https://aider.chat/docs/git.html](https://aider.chat/docs/git.html)

[](#git-integration)Git integration
===================================

Aider works best with code that is part of a git repo. Aider is tightly integrated with git, which makes it easy to:

*   Use the `/undo` command to instantly undo any AI changes that you don’t like.
*   Go back in the git history to review the changes that aider made to your code
*   Manage a series of aider’s changes on a git branch

Aider uses git in these ways:

*   It asks to create a git repo if you launch it in a directory without one.
*   Whenever aider edits a file, it commits those changes with a descriptive commit message. This makes it easy to undo or review aider’s changes.
*   Aider takes special care before editing files that already have uncommitted changes (dirty files). Aider will first commit any preexisting changes with a descriptive commit message. This keeps your edits separate from aider’s edits, and makes sure you never lose your work if aider makes an inappropriate change.

[](#in-chat-commands)In-chat commands
-------------------------------------

Aider also allows you to use [in-chat commands](/docs/usage/commands.html) to perform git operations:

*   `/diff` will show all the file changes since the last message you sent.
*   `/undo` will undo and discard the last change.
*   `/commit` to commit all dirty changes with a sensible commit message.
*   `/git` will let you run raw git commands to do more complex management of your git history.

You can also manage your git history outside of aider with your preferred git tools.

[](#disabling-git-integration)Disabling git integration
-------------------------------------------------------

While it is not recommended, you can disable aider’s use of git in a few ways:

*   `--no-auto-commits` will stop aider from git committing each of its changes.
*   `--no-dirty-commits` will stop aider from committing dirty files before applying its edits.
*   `--no-git` will completely stop aider from using git on your files. You should ensure you are keeping sensible backups of the files you are working with.

[](#commit-messages)Commit messages
-----------------------------------

Aider sends the `--weak-model` a copy of the diffs and the chat history and asks it to produce a commit message. By default, aider creates commit messages which follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).

You can customize the [commit prompt](https://github.com/Aider-AI/aider/blob/main/aider/prompts.py#L5) with the `--commit-prompt` option. You can place that on the command line, or [configure it via a config file or environment variables](https://aider.chat/docs/config.html).

[](#commit-attribution)Commit attribution
-----------------------------------------

Aider marks commits that it either authored or committed.

*   If aider authored the changes in a commit, they will have “(aider)” appended to the git author and git committer name metadata.
*   If aider simply committed changes (found in dirty files), the commit will have “(aider)” appended to the git committer name metadata.

You can use `--no-attribute-author` and `--no-attribute-committer` to disable modification of the git author and committer name fields.

Additionally, you can use the following options to prefix commit messages:

*   `--attribute-commit-message-author`: Prefix commit messages with ‘aider: ‘ if aider authored the changes.
*   `--attribute-commit-message-committer`: Prefix all commit messages with ‘aider: ‘, regardless of whether aider authored the changes or not.

Both of these options are disabled by default, but can be useful for easily identifying changes made by aider.

---



## [https://aider.chat/docs/languages.html](https://aider.chat/docs/languages.html)

[](#supported-languages)Supported languages
===========================================

Aider should work well with most popular coding languages. This is because top LLMs are fluent in most mainstream languages, and familiar with popular libraries, packages and frameworks.

Aider has specific support for linting many languages. By default, aider runs the built in linter any time a file is edited. If it finds syntax errors, aider will offer to fix them for you. This helps catch small code issues and quickly fix them.

Aider also does code analysis to help the LLM navigate larger code bases by producing a [repository map](https://aider.chat/docs/repomap.html). Aider can currently produce repository maps for many popular mainstream languages, listed below.

[](#how-to-add-support-for-another-language)How to add support for another language
-----------------------------------------------------------------------------------

Aider should work quite well for other languages, even those without repo map or linter support. You should really try coding with aider before assuming it needs better support for your language.

That said, if aider already has support for linting your language, then it should be possible to add repo map support. To build a repo map, aider needs the `tags.scm` file from the given language’s tree-sitter grammar. If you can find and share that file in a [GitHub issue](https://github.com/Aider-AI/aider/issues), then it may be possible to add repo map support.

If aider doesn’t support linting, it will be complicated to add linting and repo map support. That is because aider relies on [py-tree-sitter-languages](https://github.com/grantjenks/py-tree-sitter-languages) to provide pre-packaged versions of tree-sitter parsers for many languages.

Aider needs to be easy for users to install in many environments, and it is probably too complex to add dependencies on additional individual tree-sitter parsers.

Language

File extension

Repo map

Linter

bash

.bash

 

✓

c

.c

✓

✓

c\_sharp

.cs

✓

✓

commonlisp

.cl

 

✓

cpp

.cc

✓

✓

cpp

.cpp

✓

✓

css

.css

 

✓

dockerfile

.dockerfile

 

✓

dot

.dot

 

✓

elisp

.el

✓

✓

elixir

.ex

✓

✓

elm

.elm

✓

✓

embedded\_template

.et

 

✓

erlang

.erl

 

✓

go

.go

✓

✓

gomod

.gomod

 

✓

hack

.hack

 

✓

haskell

.hs

 

✓

hcl

.hcl

 

✓

html

.html

 

✓

java

.java

✓

✓

javascript

.js

✓

✓

javascript

.mjs

✓

✓

jsdoc

.jsdoc

 

✓

json

.json

 

✓

julia

.jl

 

✓

kotlin

.kt

✓

✓

lua

.lua

 

✓

make

.mk

 

✓

objc

.m

 

✓

ocaml

.ml

✓

✓

perl

.pl

 

✓

php

.php

✓

✓

python

.py

✓

✓

ql

.ql

✓

✓

r

.R

 

✓

r

.r

 

✓

regex

.regex

 

✓

rst

.rst

 

✓

ruby

.rb

✓

✓

rust

.rs

✓

✓

scala

.scala

 

✓

sql

.sql

 

✓

sqlite

.sqlite

 

✓

toml

.toml

 

✓

tsq

.tsq

 

✓

typescript

.ts

✓

✓

typescript

.tsx

✓

✓

yaml

.yaml

 

✓

---



## [https://aider.chat/docs/repomap.html](https://aider.chat/docs/repomap.html)

[](#repository-map)Repository map
=================================

Aider uses a **concise map of your whole git repository** that includes the most important classes and functions along with their types and call signatures. This helps aider understand the code it’s editing and how it relates to the other parts of the codebase. The repo map also helps aider write new code that respects and utilizes existing libraries, modules and abstractions found elsewhere in the codebase.

[](#using-a-repo-map-to-provide-context)Using a repo map to provide context
---------------------------------------------------------------------------

Aider sends a **repo map** to the LLM along with each change request from the user. The repo map contains a list of the files in the repo, along with the key symbols which are defined in each file. It shows how each of these symbols are defined, by including the critical lines of code for each definition.

Here’s a part of the repo map of aider’s repo, for [base\_coder.py](https://github.com/Aider-AI/aider/blob/main/aider/coders/base_coder.py) and [commands.py](https://github.com/Aider-AI/aider/blob/main/aider/commands.py) :

    aider/coders/base_coder.py:
    ⋮...
    │class Coder:
    │    abs_fnames = None
    ⋮...
    │    @classmethod
    │    def create(
    │        self,
    │        main_model,
    │        edit_format,
    │        io,
    │        skip_model_availabily_check=False,
    │        **kwargs,
    ⋮...
    │    def abs_root_path(self, path):
    ⋮...
    │    def run(self, with_message=None):
    ⋮...
    
    aider/commands.py:
    ⋮...
    │class Commands:
    │    voice = None
    │
    ⋮...
    │    def get_commands(self):
    ⋮...
    │    def get_command_completions(self, cmd_name, partial):
    ⋮...
    │    def run(self, inp):
    ⋮...
    

Mapping out the repo like this provides some key benefits:

*   The LLM can see classes, methods and function signatures from everywhere in the repo. This alone may give it enough context to solve many tasks. For example, it can probably figure out how to use the API exported from a module just based on the details shown in the map.
*   If it needs to see more code, the LLM can use the map to figure out which files it needs to look at. The LLM can ask to see these specific files, and aider will offer to add them to the chat context.

[](#optimizing-the-map)Optimizing the map
-----------------------------------------

Of course, for large repositories even just the repo map might be too large for the LLM’s context window. Aider solves this problem by sending just the **most relevant** portions of the repo map. It does this by analyzing the full repo map using a graph ranking algorithm, computed on a graph where each source file is a node and edges connect files which have dependencies. Aider optimizes the repo map by selecting the most important parts of the codebase which will fit into the active token budget.

The token budget is influenced by the `--map-tokens` switch, which defaults to 1k tokens. Aider adjusts the size of the repo map dynamically based on the state of the chat. It will usually stay within that setting’s value. But it does expand the repo map significantly at times, especially when no files have been added to the chat and aider needs to understand the entire repo as best as possible.

The sample map shown above doesn’t contain _every_ class, method and function from those files. It only includes the most important identifiers, the ones which are most often referenced by other portions of the code. These are the key pieces of context that the LLM needs to know to understand the overall codebase.

[](#more-info)More info
-----------------------

Please check the [repo map article on aider’s blog](https://aider.chat/2023/10/22/repomap.html) for more information on aider’s repository map and how it is constructed.

---



## [https://aider.chat/docs/scripting.html](https://aider.chat/docs/scripting.html)

[](#scripting-aider)Scripting aider
===================================

You can script aider via the command line or python.

[](#command-line)Command line
-----------------------------

Aider takes a `--message` argument, where you can give it a natural language instruction. It will do that one thing, apply the edits to the files and then exit. So you could do:

    aider --message "make a script that prints hello" hello.js
    

Or you can write simple shell scripts to apply the same instruction to many files:

    for FILE in *.py ; do
        aider --message "add descriptive docstrings to all the functions" $FILE
    done
    

Use `aider --help` to see all the [command line options](/docs/config/options.html), but these are useful for scripting:

    --stream, --no-stream
                          Enable/disable streaming responses (default: True) [env var:
                          AIDER_STREAM]
    --message COMMAND, --msg COMMAND, -m COMMAND
                          Specify a single message to send GPT, process reply then exit
                          (disables chat mode) [env var: AIDER_MESSAGE]
    --message-file MESSAGE_FILE, -f MESSAGE_FILE
                          Specify a file containing the message to send GPT, process reply,
                          then exit (disables chat mode) [env var: AIDER_MESSAGE_FILE]
    --yes                 Always say yes to every confirmation [env var: AIDER_YES]
    --auto-commits, --no-auto-commits
                          Enable/disable auto commit of GPT changes (default: True) [env var:
                          AIDER_AUTO_COMMITS]
    --dirty-commits, --no-dirty-commits
                          Enable/disable commits when repo is found dirty (default: True) [env
                          var: AIDER_DIRTY_COMMITS]
    --dry-run, --no-dry-run
                          Perform a dry run without modifying files (default: False) [env var:
                          AIDER_DRY_RUN]
    --commit              Commit all pending changes with a suitable commit message, then exit
                          [env var: AIDER_COMMIT]
    

[](#python)Python
-----------------

You can also script aider from python:

    from aider.coders import Coder
    from aider.models import Model
    
    # This is a list of files to add to the chat
    fnames = ["greeting.py"]
    
    model = Model("gpt-4-turbo")
    
    # Create a coder object
    coder = Coder.create(main_model=model, fnames=fnames)
    
    # This will execute one instruction on those files and then return
    coder.run("make a script that prints hello world")
    
    # Send another instruction
    coder.run("make it say goodbye")
    
    # You can run in-chat "/" commands too
    coder.run("/tokens")
    
    

See the [Coder.create() and Coder.**init**() methods](https://github.com/Aider-AI/aider/blob/main/aider/coders/base_coder.py) for all the supported arguments.

It can also be helpful to set the equivalent of `--yes` by doing this:

    from aider.io import InputOutput
    io = InputOutput(yes=True)
    # ...
    coder = Coder.create(model=model, fnames=fnames, io=io)
    

The python scripting API is not officially supported or documented, and could change in future releases without providing backwards compatibility.

---



## [https://aider.chat/docs/more/infinite-output.html](https://aider.chat/docs/more/infinite-output.html)

[](#infinite-output)Infinite output
===================================

LLM providers limit how much output a model can generate from a single request. This is usually called the output token limit.

Aider is able to work around this limit with models that support “prefilling” the assistant response. When you use aider with a model that supports prefill, you will see “infinite output” noted in the announcement lines displayed at launch:

    Aider v0.58.0
    Main model: claude-3-5-sonnet-20240620 with diff edit format, prompt cache, infinite output
    

Models that support prefill can be primed to think they started their response with a specific piece of text. You can put words in their mouth, and they will continue generating text from that point forward.

When aider is collecting code edits from a model and it hits the output token limit, aider simply initiates another LLM request with the partial response prefilled. This prompts the model to continue where it left off, generating more of the desired response. This prefilling of the partially completed response can be repeated, allowing for very long outputs. Joining the text across these output limit boundaries requires some heuristics, but is typically fairly reliable.

Aider supports “infinite output” for models that support “prefill”, such as:

*   anthropic.claude-3-5-haiku-20241022-v1:0
*   anthropic.claude-3-5-sonnet-20241022-v2:0
*   claude-3-5-haiku-20241022
*   claude-3-5-sonnet-20240620
*   claude-3-5-sonnet-20241022
*   claude-3-haiku-20240307
*   claude-3-opus-20240229
*   claude-3-sonnet-20240229
*   codestral/codestral-2405
*   codestral/codestral-latest
*   deepseek/deepseek-chat
*   deepseek/deepseek-coder
*   deepseek/deepseek-reasoner
*   eu.anthropic.claude-3-5-haiku-20241022-v1:0
*   eu.anthropic.claude-3-5-sonnet-20241022-v2:0
*   mistral/codestral-2405
*   mistral/codestral-latest
*   mistral/codestral-mamba-latest
*   mistral/mistral-large-2402
*   mistral/mistral-large-2407
*   mistral/mistral-large-2411
*   mistral/mistral-large-latest
*   mistral/mistral-medium
*   mistral/mistral-medium-2312
*   mistral/mistral-medium-latest
*   mistral/mistral-small
*   mistral/mistral-small-latest
*   mistral/mistral-tiny
*   mistral/open-codestral-mamba
*   mistral/open-mistral-7b
*   mistral/open-mistral-nemo
*   mistral/open-mistral-nemo-2407
*   mistral/open-mixtral-8x22b
*   mistral/open-mixtral-8x7b
*   mistral/pixtral-12b-2409
*   mistral/pixtral-large-2411
*   mistral/pixtral-large-latest
*   openrouter/anthropic/claude-3.5-sonnet
*   us.anthropic.claude-3-5-haiku-20241022-v1:0
*   us.anthropic.claude-3-5-sonnet-20241022-v2:0
*   vertex\_ai/claude-3-5-haiku
*   vertex\_ai/claude-3-5-haiku@20241022
*   vertex\_ai/claude-3-5-sonnet
*   vertex\_ai/claude-3-5-sonnet-v2
*   vertex\_ai/claude-3-5-sonnet-v2@20241022
*   vertex\_ai/claude-3-5-sonnet@20240620
*   vertex\_ai/claude-3-haiku
*   vertex\_ai/claude-3-haiku@20240307
*   vertex\_ai/claude-3-opus
*   vertex\_ai/claude-3-opus@20240229
*   vertex\_ai/claude-3-sonnet
*   vertex\_ai/claude-3-sonnet@20240229

---



## [https://aider.chat/docs/more/edit-formats.html](https://aider.chat/docs/more/edit-formats.html)

[](#edit-formats)Edit formats
=============================

Aider uses various “edit formats” to let LLMs edit source files. Different models work better or worse with different edit formats. Aider is configured to use the optimal format for most popular, common models. You can always force use of a specific edit format with the `--edit-format` switch.

[](#whole)whole
---------------

The “whole” edit format is the simplest possible editing format. The LLM is instructed to return a full, updated copy of each source file that needs changes. While simple, it can be slow and costly because the LLM has to return the _entire file_ even if just a few lines are edited.

The whole format expects the file path just before the fenced file content:

    show_greeting.py
    ```
    import sys
    
    def greeting(name):
        print("Hey", name)
    
    if __name__ == '__main__':
        greeting(sys.argv[1])
    ```
    

[](#diff)diff
-------------

The “diff” edit format asks the LLM to specify file edits as a series of search/replace blocks. This is an efficient format, because the model only needs to return parts of the file which have changes.

Edits are formatted using a syntax similar to the git merge conflict resolution markings, with the file path right before a fenced block:

    mathweb/flask/app.py
    ```
    <<<<<<< SEARCH
    from flask import Flask
    =======
    import math
    from flask import Flask
    >>>>>>> REPLACE
    ```
    

[](#diff-fenced)diff-fenced
---------------------------

The “diff-fenced” edit format is based on the diff format, but the file path is placed inside the fence. It is primarily used with the Gemini family of models, which often fail to conform to the fencing approach specified in the diff format.

    ```
    mathweb/flask/app.py
    <<<<<<< SEARCH
    from flask import Flask
    =======
    import math
    from flask import Flask
    >>>>>>> REPLACE
    ```
    

[](#udiff)udiff
---------------

The “udiff” edit format is based on the widely used unified diff format, but [modified and simplified](/2023/12/21/unified-diffs.html). This is an efficient format, because the model only needs to return parts of the file which have changes.

It was mainly used to the GPT-4 Turbo family of models, because it reduced their “lazy coding” tendencies. With other edit formats the GPT-4 Turbo models tended to elide large sections of code and replace them with “# … original code here …” style comments.

    ```diff
    --- mathweb/flask/app.py
    +++ mathweb/flask/app.py
    @@ ... @@
    -class MathWeb:
    +import sympy
    +
    +class MathWeb:
    ```
    

[](#editor-diff-and-editor-whole)editor-diff and editor-whole
-------------------------------------------------------------

These are streamlined versions of the diff and whole formats, intended to be used with `--editor-edit-format` when using [architect mode](/docs/usage/modes.html). The actual edit format is the same, but aider uses a simpler prompt that is more narrowly focused on just editing the file as opposed to solving the coding task. The architect model resolves the coding task and provides plain text instructions about which file changes need to be made. The editor interprets those instructions to produce the syntactically correct diff or whole edits.

---



## [https://aider.chat/docs/more/analytics.html](https://aider.chat/docs/more/analytics.html)

[](#analytics)Analytics
=======================

Aider can collect anonymous analytics to help improve aider’s ability to work with LLMs, edit code and complete user requests.

[](#opt-in-anonymous-no-personal-info)Opt-in, anonymous, no personal info
-------------------------------------------------------------------------

Analytics are only collected if you agree and opt-in. Aider respects your privacy and never collects your code, chat messages, keys or personal info.

Aider collects information on:

*   which LLMs are used and with how many tokens,
*   which of aider’s edit formats are used,
*   how often features and commands are used,
*   information about exceptions and errors,
*   etc

These analytics are associated with an anonymous, randomly generated UUID4 user identifier.

This information helps improve aider by identifying which models, edit formats, features and commands are most used. It also helps uncover bugs that users are experiencing, so that they can be fixed in upcoming releases.

[](#disabling-analytics)Disabling analytics
-------------------------------------------

You can opt out of analytics forever by running this command one time:

    aider --analytics-disable
    

[](#enabling-analytics)Enabling analytics
-----------------------------------------

The `--[no-]analytics` switch controls whether analytics are enabled for the current session:

*   `--analytics` will turn on analytics for the current session. This will _not_ have any effect if you have permanently disabled analytics with `--analytics-disable`. If this is the first time you have enabled analytics, aider will confirm you wish to opt-in to analytics.
*   `--no-analytics` will turn off analytics for the current session.
*   By default, if you don’t provide `--analytics` or `--no-analytics`, aider will enable analytics for a random subset of users. This will never happen if you have permanently disabled analytics with `--analytics-disable`. Randomly selected users will be asked if they wish to opt-in to analytics.

[](#opting-in)Opting in
-----------------------

The first time analytics are enabled, you will need to agree to opt-in.

    aider --analytics
    
    Aider respects your privacy and never collects your code, prompts, chats, keys or any personal
    info.
    For more info: https://aider.chat/docs/more/analytics.html
    Allow collection of anonymous analytics to help improve aider? (Y)es/(N)o [Yes]:
    

If you say “no”, analytics will be permanently disabled.

[](#details-about-data-being-collected)Details about data being collected
-------------------------------------------------------------------------

### [](#sample-analytics-data)Sample analytics data

To get a better sense of what type of data is collected, you can review some [sample analytics logs](https://github.com/aider-ai/aider/blob/main/aider/website/assets/sample-analytics.jsonl). These are the last 1,000 analytics events from the author’s personal use of aider, updated regularly.

### [](#analytics-code)Analytics code

Since aider is open source, all the places where aider collects analytics are visible in the source code. They can be viewed using [GitHub search](https://github.com/search?q=repo%3Aaider-ai%2Faider+%22.event%28%22&type=code).

### [](#logging-and-inspecting-analytics)Logging and inspecting analytics

You can get a full log of the analytics that aider is collecting, in case you would like to audit or inspect this data.

    aider --analytics-log filename.jsonl
    

If you want to just log analytics without reporting them, you can do:

    aider --analytics-log filename.jsonl --no-analytics
    

[](#reporting-issues)Reporting issues
-------------------------------------

If you have concerns about any of the analytics that aider is collecting or our data practices please contact us by opening a [GitHub Issue](https://github.com/aider-ai/aider/issues).

[](#privacy-policy)Privacy policy
---------------------------------

Please see aider’s [privacy policy](/docs/legal/privacy.html) for more details.

---



## [https://aider.chat/docs/legal/privacy.html](https://aider.chat/docs/legal/privacy.html)

[](#privacy-policy)Privacy policy
=================================

[Aider AI LLC](/docs/faq.html#what-is-aider-ai-llc) (“Aider,” “we,” “our,” and/or “us”) values the privacy of individuals who use our website, programming tools, and related services (collectively, our “Services”). This privacy policy (the “Privacy Policy”) explains how we collect, use, and disclose information from users of our Services. By using our Services, you agree to the collection, use, disclosure, and procedures this Privacy Policy describes.

### [](#information-we-collect)Information We Collect

We may collect a variety of information from or about you or your devices from various sources, as described below.

### [](#a-information-you-provide-to-us)A. Information You Provide to Us.

**Communications.** If you contact us directly, we may receive additional information about you, such as your name, email address, the contents of a message or attachments that you may send to us, and other information you choose to provide.

### [](#b-information-we-collect-when-you-use-our-services)B. Information We Collect When You Use Our Services.

**Device Information.** We may receive information about the device and software you use to access our Services, including IP address, device type, device identifiers, web browser type and version, and operating system version.

**Usage Information.** We may automatically receive information about your interactions with our Services, like the pages or other content you view, referrer information (the website you visited before coming to our Services), and the dates and times of your visits.

**Analytics Information.** If you use our programming tools, we may receive information about your interactions with the tools, such as how often certain features or commands are used, information about exceptions and errors, and which large language models are used. This information is associated with a randomly generated identifier, not any directly identifiable user information such as your name or email address. Please see the “Your Choices” section below for information on how to disable the collection of this information.

**Information from Cookies and Other Tracking Technologies.** We and our third-party partners may collect information about your activities on our Services using cookies, pixel tags, SDKs, or other tracking technologies. Our third-party partners, such as analytics and security partners, may also use these technologies to collect information about your online activities over time and across different services.

### [](#how-we-use-the-information-we-collect)How We Use the Information We Collect

We use the information we collect:

*   To provide, maintain, improve, and enhance our Services;
*   To understand and analyze how you use our Services and develop new products, services, features, and functionality;
*   To communicate with you, provide you with updates and other information relating to our Services, provide information that you request, respond to comments and questions, and otherwise provide customer support;
*   To generate anonymized or aggregate data containing only de-identified, non-personal information that we may use for any lawful purposes such as to publish reports;
*   To find and prevent fraud and abuse, and respond to trust and safety issues that may arise;
*   For compliance purposes, including enforcing our legal rights, or as may be required by applicable laws and regulations or requested by any judicial process or governmental agency; and
*   For other purposes for which we provide specific notice at the time the information is collected.

### [](#how-we-disclose-the-information-we-collect)How We Disclose the Information We Collect

**Affiliates.** We may disclose any information we receive to our current or future affiliates for any of the purposes described in this Privacy Policy.

**Vendors and Service Providers.** We may disclose any information we receive to vendors and service providers retained in connection with the provision of our Services.

**Analytics Partners.** We may use analytics services to collect and process certain analytics data to improve our Services, such as by improving the ability of our programming tools to work with LLMs, edit code, and complete user requests.

**As Required By Law and Similar Disclosures.** We may access, preserve, and disclose your information if we believe doing so is required or appropriate to: (a) comply with law enforcement requests and legal process, such as a court order or subpoena; (b) respond to your requests; or (c) protect your, our, or others’ rights, property, or safety. For the avoidance of doubt, the disclosure of your information may occur if you post any objectionable content on or through the Services.

**Merger, Sale, or Other Asset Transfers.** We may transfer your information to service providers, advisors, potential transactional partners, or other third parties in connection with the consideration, negotiation, or completion of a corporate transaction in which we are acquired by or merged with another company or we sell, liquidate, or transfer all or a portion of our assets. The use of your information following any of these events will be governed by the provisions of this Privacy Policy in effect at the time the applicable information was collected.

**Consent.** We may also disclose your information with your permission.

### [](#your-choices)Your Choices

**Analytics Information.** You can turn off analytics collection when using our programming tools. Please visit this [documentation page](/docs/more/analytics.html) for more information about the data collected and your options.

### [](#third-parties)Third Parties

Our Services may contain links to other websites, products, or services that we do not own or operate. We are not responsible for the privacy practices of these third parties. Please be aware that this Privacy Policy does not apply to your activities on these third-party services or any information you disclose to these third parties. We encourage you to read their privacy policies before providing any information to them.

### [](#security)Security

We make reasonable efforts to protect your information by using physical and electronic safeguards designed to improve the security of the information we maintain. However, because no electronic transmission or storage of information can be entirely secure, we can make no guarantees as to the security or privacy of your information.

### [](#childrens-privacy)Children’s Privacy

We do not knowingly collect, maintain, or use personal information from children under 18 years of age, and no part of our Service(s) is directed to children. If you learn that a child has provided us with personal information in violation of this Privacy Policy, then you may alert us at privacy@aider.chat.

### [](#international-visitors)International Visitors

Our Services are hosted in the United States and intended for visitors located within the United States. If you choose to use the Services from the European Union or other regions of the world with laws governing data collection and use that may differ from U.S. law, then please note that you are transferring your personal information outside of those regions to the U.S. for storage and processing. We may also transfer your data from the U.S. to other countries or regions in connection with storage and processing of data, fulfilling your requests, and operating the Services. By providing any information, including personal information, on or to the Services, you consent to such transfer, storage, and processing.

### [](#changes-to-this-privacy-policy)Changes to this Privacy Policy

We will post any adjustments to the Privacy Policy on this page, and the revised version will be effective when it is posted. If we materially change the ways in which we use or disclose personal information previously collected from you through the Services, we will notify you through the Services, by email, or other communication.

### [](#contact-information)Contact Information

If you have any questions, comments, or concerns about our processing activities, please email us at privacy@aider.chat.

* * *

Last updated December 06, 2024.

---



## [https://aider.chat/docs/faq.html](https://aider.chat/docs/faq.html)

[](#faq)FAQ
===========

*   [How can I add ALL the files to the chat?](#how-can-i-add-all-the-files-to-the-chat)
*   [Can I use aider in a large (mono) repo?](#can-i-use-aider-in-a-large-mono-repo)
*   [Can I use aider with multiple git repos at once?](#can-i-use-aider-with-multiple-git-repos-at-once)
*   [How do I turn on the repository map?](#how-do-i-turn-on-the-repository-map)
*   [How do I include the git history in the context?](#how-do-i-include-the-git-history-in-the-context)
*   [How can I run aider locally from source code?](#how-can-i-run-aider-locally-from-source-code)
*   [Can I change the system prompts that aider uses?](#can-i-change-the-system-prompts-that-aider-uses)
*   [What LLMs do you use to build aider?](#what-llms-do-you-use-to-build-aider)
*   [How are the “aider wrote xx% of code” stats computed?](#how-are-the-aider-wrote-xx-of-code-stats-computed)
*   [Why does aider sometimes stop highlighting code in its replies?](#why-does-aider-sometimes-stop-highlighting-code-in-its-replies)
*   [Why is the LLM speaking to me in an unexpected language?](#why-is-the-llm-speaking-to-me-in-an-unexpected-language)
*   [Can I share my aider chat transcript?](#can-i-share-my-aider-chat-transcript)
*   [Can I edit files myself while aider is running?](#can-i-edit-files-myself-while-aider-is-running)
*   [What is Aider AI LLC?](#what-is-aider-ai-llc)

Use `/help <question>` to [ask for help about using aider](/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.

[](#how-can-i-add-all-the-files-to-the-chat)How can I add ALL the files to the chat?
------------------------------------------------------------------------------------

People regularly ask about how to add **many or all of their repo’s files** to the chat. This is probably not a good idea and will likely do more harm than good.

The best approach is think about which files need to be changed to accomplish the task you are working on. Just add those files to the chat.

Usually when people want to add “all the files” it’s because they think it will give the LLM helpful context about the overall code base. Aider will automatically give the LLM a bunch of additional context about the rest of your git repo. It does this by analyzing your entire codebase in light of the current chat to build a compact [repository map](https://aider.chat/2023/10/22/repomap.html).

Adding a bunch of files that are mostly irrelevant to the task at hand will often distract or confuse the LLM. The LLM will give worse coding results, and sometimese even fail to correctly edit files. Addings extra files will also increase your token costs.

Again, it’s usually best to just add the files to the chat that will need to be modified. If you still wish to add lots of files to the chat, you can:

*   Use a wildcard when you launch aider: `aider src/*.py`
*   Use a wildcard with the in-chat `/add` command: `/add src/*.py`
*   Give the `/add` command a directory name and it will recursively add every file under that dir: `/add src`

[](#can-i-use-aider-in-a-large-mono-repo)Can I use aider in a large (mono) repo?
--------------------------------------------------------------------------------

Aider will work in any size repo, but is not optimized for quick performance and response time in very large repos. There are some things you can do to improve performance.

Be sure to check the [general usage tips](/docs/usage/tips.html) before considering this large-repo specific advice. To get the best results from aider you want to be thoughtful about how you add files to the chat, regardless of your repo size.

You can change into a sub directory of your repo that contains the code you want to work on and use the `--subtree-only` switch. This will tell aider to ignore the repo outside of the directory you start in.

You can also create a `.aiderignore` file to tell aider to ignore parts of the repo that aren’t relevant to your task. This file conforms to `.gitignore` syntax and conventions. For example, to focus only on specific directories in a monorepo, you could create a `.aiderignore` file with:

    # Ignore everything
    /*
    
    # Allow specific directories and their contents
    !foo/
    !bar/
    !baz/
    
    # Allow nested files under these directories
    !foo/**
    !bar/**
    !baz/**
    

You can use `--aiderignore <filename>` to name a specific file to use for ignore patterns. You might have a few of these handy for when you want to work on frontend, backend, etc portions of your repo.

[](#can-i-use-aider-with-multiple-git-repos-at-once)Can I use aider with multiple git repos at once?
----------------------------------------------------------------------------------------------------

Currently aider can only work with one repo at a time.

There are some things you can try if you need to work with multiple interrelated repos:

*   You can run aider in repo-A where you need to make a change and use `/read` to add some files read-only from another repo-B. This can let aider see key functions or docs from the other repo.
*   You can run `aider --show-repo-map > map.md` within each repo to create repo maps. You could then run aider in repo-A and use `/read ../path/to/repo-B/map.md` to share a high level map of the other repo.
*   You can use aider to write documentation about a repo. Inside each repo, you could run `aider docs.md` and work with aider to write some markdown docs. Then while using aider to edit repo-A you can `/read ../path/to/repo-B/docs.md` to read in those docs from the other repo.
*   In repo A, ask aider to write a small script that demonstrates the functionality you want to use in repo B. Then when you’re using aider in repo B, you can `/read` in that script.

[](#how-do-i-turn-on-the-repository-map)How do I turn on the repository map?
----------------------------------------------------------------------------

Depending on the LLM you are using, aider may launch with the repo map disabled by default:

    Repo-map: disabled
    

This is because weaker models get easily overwhelmed and confused by the content of the repo map. They sometimes mistakenly try to edit the code in the repo map. The repo map is usually disabled for a good reason.

If you would like to force it on, you can run aider with `--map-tokens 1024`.

[](#how-do-i-include-the-git-history-in-the-context)How do I include the git history in the context?
----------------------------------------------------------------------------------------------------

When starting a fresh aider session, you can include recent git history in the chat context. This can be useful for providing the LLM with information about recent changes. To do this:

1.  Use the `/run` command with `git diff` to show recent changes:
    
        /run git diff HEAD~1
        
    
    This will include the diff of the last commit in the chat history.
    
2.  To include diffs from multiple commits, increase the number after the tilde:
    
        /run git diff HEAD~3
        
    
    This will show changes from the last three commits.
    

Remember, the chat history already includes recent changes made during the current session, so this tip is most useful when starting a new aider session and you want to provide context about recent work.

You can also use aider to review PR branches:

    /run git diff one-branch..another-branch
    
    ...
    
    Add 6.9k tokens of command output to the chat? (Y)es/(N)o [Yes]: Yes
    
    /ask Are there any problems with the way this change works with the FooBar class?
    

The `/git` command will not work for this purpose, as its output is not included in the chat.

[](#how-can-i-run-aider-locally-from-source-code)How can I run aider locally from source code?
----------------------------------------------------------------------------------------------

To run the project locally, follow these steps:

    # Clone the repository
    git clone git@github.com:Aider-AI/aider.git
    
    # Navigate to the project directory
    cd aider
    
    # It's recommended to make a virtual environment
    
    # Install aider in editable/development mode, 
    # so it runs from the latest copy of these source files
    python -m pip install -e .
    
    # Run the local version of aider
    python -m aider
    

[](#can-i-change-the-system-prompts-that-aider-uses)Can I change the system prompts that aider uses?
----------------------------------------------------------------------------------------------------

The most convenient way to add custom instructions is to use a [conventions file](https://aider.chat/docs/usage/conventions.html).

But, aider is set up to support different actual system prompts and edit formats in a modular way. If you look in the `aider/coders` subdirectory, you’ll see there’s a base coder with base prompts, and then there are a number of different specific coder implementations.

If you’re thinking about experimenting with system prompts this document about [benchmarking GPT-3.5 and GPT-4 on code editing](https://aider.chat/docs/benchmarks.html) might be useful background.

While it’s not well documented how to add new coder subsystems, you may be able to modify an existing implementation or use it as a template to add another.

To get started, try looking at and modifying these files.

The wholefile coder is currently used by GPT-3.5 by default. You can manually select it with `--edit-format whole`.

*   wholefile\_coder.py
*   wholefile\_prompts.py

The editblock coder is currently used by GPT-4o by default. You can manually select it with `--edit-format diff`.

*   editblock\_coder.py
*   editblock\_prompts.py

The universal diff coder is currently used by GPT-4 Turbo by default. You can manually select it with `--edit-format udiff`.

*   udiff\_coder.py
*   udiff\_prompts.py

When experimenting with coder backends, it helps to run aider with `--verbose --no-pretty` so you can see all the raw information being sent to/from the LLM in the conversation.

You can also refer to the [instructions for installing a development version of aider](https://aider.chat/docs/install/optional.html#install-the-development-version-of-aider).

[](#what-llms-do-you-use-to-build-aider)What LLMs do you use to build aider?
----------------------------------------------------------------------------

Aider writes a lot of its own code, usually about 70% of the new code in each release. People often ask which LLMs I use with aider, when writing aider. Below is a table showing the models I have used recently, extracted from the [public log](https://github.com/aider-ai/aider/blob/main/aider/website/assets/sample-analytics.jsonl) of my [aider analytics](https://aider.chat/docs/more/analytics.html).

Model Name

Total Tokens

Percent

deepseek/deepseek-chat

1,272,856

52.9%

claude-3-5-sonnet-20241022

769,815

32.0%

deepseek/REDACTED

308,841

12.8%

o1

25,121

1.0%

claude-3-5-haiku-20241022

10,083

0.4%

gemini/gemini-exp-1206

10,068

0.4%

mistral/codestral-latest

8,137

0.3%

gpt-4o

1,775

0.1%

o1-preview

175

0.0%

Some models show as REDACTED, because they are new or unpopular models. Aider’s analytics only records the names of “well known” LLMs.

[](#how-are-the-aider-wrote-xx-of-code-stats-computed)How are the “aider wrote xx% of code” stats computed?
-----------------------------------------------------------------------------------------------------------

[Aider is tightly integrated with git](/docs/git.html) so all of aider’s code changes are committed to the repo with proper attribution. The [stats are computed](https://github.com/Aider-AI/aider/blob/main/scripts/blame.py) by doing something like `git blame` on the repo, and counting up who wrote all the new lines of code in each release. Only lines in source code files are counted, not documentation or prompt files.

[](#why-does-aider-sometimes-stop-highlighting-code-in-its-replies)Why does aider sometimes stop highlighting code in its replies?
----------------------------------------------------------------------------------------------------------------------------------

Aider displays the markdown responses that are coming back from the LLM. Usually, the LLM will reply with code in a markdown “code block” with triple backtick fences, like this:

    Here's some code:
    
    ```
    print("hello")
    ```
    

But if you’ve added files to the chat that contain triple backticks, aider needs to tell the LLM to use a different set of fences. Otherwise, the LLM can’t safely include your code’s triple backticks inside the code blocks that it returns with edits. Aider will use fences like `<source>...</source>` in this case.

A side effect of this is that the code that aider outputs may no longer be properly highlighted. You will most often notice this if you add markdown files to you chats that contain code blocks.

[](#why-is-the-llm-speaking-to-me-in-an-unexpected-language)Why is the LLM speaking to me in an unexpected language?
--------------------------------------------------------------------------------------------------------------------

Aider goes to some effort to prompt the model to use the language that is configured for your system. But LLMs aren’t fully reliable, and they sometimes decide to speak in an unexpected language. Claude is especially fond of speaking French.

You can explicitly set the language that aider tells the model to use with `--chat-language <language>`. But the LLM may not comply.

[](#can-i-share-my-aider-chat-transcript)Can I share my aider chat transcript?
------------------------------------------------------------------------------

Yes, you can now share aider chat logs in a pretty way.

1.  Copy the markdown logs you want to share from `.aider.chat.history.md` and make a github gist. Or publish the raw markdown logs on the web any way you’d like.
    
        https://gist.github.com/Aider-AI/2087ab8b64034a078c0a209440ac8be0
        
    
2.  Take the gist URL and append it to:
    
        https://aider.chat/share/?mdurl=
        
    

This will give you a URL like this, which shows the chat history like you’d see in a terminal:

    https://aider.chat/share/?mdurl=https://gist.github.com/Aider-AI/2087ab8b64034a078c0a209440ac8be0
    

[](#can-i-edit-files-myself-while-aider-is-running)Can I edit files myself while aider is running?
--------------------------------------------------------------------------------------------------

Yes. Aider always reads the latest copy of files from the file system when you send each message.

While you’re waiting for aider’s reply to complete, it’s probably unwise to edit files that you’ve added to the chat. Your edits and aider’s edits might conflict.

[](#what-is-aider-ai-llc)What is Aider AI LLC?
----------------------------------------------

Aider AI LLC is the company behind the aider AI coding tool. Aider is [open source and available on GitHub](https://github.com/Aider-AI/aider) under an [Apache 2.0 license](https://github.com/Aider-AI/aider/blob/main/LICENSE.txt).

---



## [https://aider.chat/HISTORY.html](https://aider.chat/HISTORY.html)

[](#release-history)Release history
===================================

The above [stats are based on the git commit history](/docs/faq.html#how-are-the-aider-wrote-xx-of-code-stats-computed) of the aider repo.

[](#release-notes)Release notes
-------------------------------

### [](#aider-v0722)Aider v0.72.2

*   Harden against user/assistant turn order problems which cause R1 errors.
*   Added environment variable AIDER\_SANITY\_CHECK\_TURNS for turn order validation.

### [](#aider-v0721)Aider v0.72.1

*   Fix model metadata for `openrouter/deepseek/deepseek-r1`

### [](#aider-v0720)Aider v0.72.0

*   Support for DeepSeek R1.
    *   Use shortcut: `--model r1`
    *   Also via OpenRouter: `--model openrouter/deepseek/deepseek-r1`
*   Added Kotlin syntax support to repo map, by Paul Walker.
*   Added `--line-endings` for file writing, by Titusz Pan.
*   Added examples\_as\_sys\_msg=True for GPT-4o models, improves benchmark scores.
*   Bumped all dependencies, to pick up litellm support for o1 system messages.
*   Bugfix for turn taking when reflecting lint/test errors.
*   Aider wrote 52% of the code in this release.

### [](#aider-v0711)Aider v0.71.1

*   Fix permissions issue in Docker images.
*   Added read-only file announcements.
*   Bugfix: ASCII fallback for unicode errors.
*   Bugfix: integer indices for list slicing in repomap calculations.

### [](#aider-v0710)Aider v0.71.0

*   Prompts to help DeepSeek work better when alternating between `/ask` and `/code`.
*   Streaming pretty LLM responses is smoother and faster for long replies.
*   Streaming automatically turns of for model that don’t support it
    *   Can now switch to/from `/model o1` and a streaming model
*   Pretty output remains enabled even when editing files with triple-backtick fences
*   Bare `/ask`, `/code` and `/architect` commands now switch the chat mode.
*   Increased default size of the repomap.
*   Increased max chat history tokens limit from 4k to 8k.
*   Turn off fancy input and watch files if terminal is dumb.
*   Added support for custom voice format and input device settings.
*   Disabled Streamlit email prompt, by apaz-cli.
*   Docker container runs as non-root user.
*   Fixed lint command handling of nested spaced strings, by Aaron Weisberg.
*   Added token count feedback when adding command output to chat.
*   Improved error handling for large audio files with automatic format conversion.
*   Improved handling of git repo index errors, by Krazer.
*   Improved unicode handling in console output with ASCII fallback.
*   Added AssertionError, AttributeError to git error handling.
*   Aider wrote 60% of the code in this release.

### [](#aider-v0700)Aider v0.70.0

*   Full support for o1 models.
*   Watch files now honors `--subtree-only`, and only watches that subtree.
*   Improved prompting for watch files, to work more reliably with more models.
*   New install methods via uv, including one-liners.
*   Support for openrouter/deepseek/deepseek-chat model.
*   Better error handling when interactive commands are attempted via `/load` or `--load`.
*   Display read-only files with abs path if its shorter than rel path.
*   Ask 10% of users to opt-in to analytics.
*   Bugfix for auto-suggest.
*   Gracefully handle unicode errors in git path names.
*   Aider wrote 74% of the code in this release.

### [](#aider-v0691)Aider v0.69.1

*   Fix for gemini model names in model metadata.
*   Show hints about AI! and AI? when user makes AI comments.
*   Support for running without git installed.
*   Improved environment variable setup messages on Windows.

### [](#aider-v0690)Aider v0.69.0

*   [Watch files](https://aider.chat/docs/usage/watch.html) improvements:
    *   Use `# ... AI?` comments to trigger aider and ask questions about your code.
    *   Now watches _all_ files, not just certain source files.
    *   Use `# AI comments`, `// AI comments`, or `-- AI comments` to give aider instructions in any text file.
*   Full support for Gemini Flash 2.0 Exp:
    *   `aider --model flash` or `aider --model gemini/gemini-2.0-flash-exp`
*   [New `--multiline` flag and `/multiline-mode` command](https://aider.chat/docs/usage/commands.html#entering-multi-line-chat-messages) makes ENTER a soft newline and META-ENTER send the message, by @miradnanali.
*   `/copy-context <instructions>` now takes optional “instructions” when [copying code context to the clipboard](https://aider.chat/docs/usage/copypaste.html#copy-aiders-code-context-to-your-clipboard-paste-into-the-web-ui).
*   Improved clipboard error handling with helpful requirements install info.
*   Ask 5% of users if they want to opt-in to analytics.
*   `/voice` now lets you edit the transcribed text before sending.
*   Disabled auto-complete in Y/N prompts.
*   Aider wrote 68% of the code in this release.

### [](#aider-v0680)Aider v0.68.0

*   [Aider works with LLM web chat UIs](https://aider.chat/docs/usage/copypaste.html).
    *   New `--copy-paste` mode.
    *   New `/copy-context` command.
*   [Set API keys and other environment variables for all providers from command line or yaml conf file](https://aider.chat/docs/config/aider_conf.html#storing-llm-keys).
    *   New `--api-key provider=key` setting.
    *   New `--set-env VAR=value` setting.
*   Added bash and zsh support to `--watch-files`.
*   Better error messages when missing dependencies for Gemini and Bedrock models.
*   Control-D now properly exits the program.
*   Don’t count token costs when API provider returns a hard error.
*   Bugfix so watch files works with files that don’t have tree-sitter support.
*   Bugfix so o1 models can be used as weak model.
*   Updated shell command prompt.
*   Added docstrings for all Coders.
*   Reorganized command line arguments with improved help messages and grouping.
*   Use the exact `sys.python` for self-upgrades.
*   Added experimental Gemini models.
*   Aider wrote 71% of the code in this release.

### [](#aider-v0670)Aider v0.67.0

*   [Use aider in your IDE or editor](https://aider.chat/docs/usage/watch.html).
    *   Run `aider --watch-files` and it will watch for instructions you add to your source files.
    *   One-liner `# ...` or `// ...` comments that start or end with “AI” are instructions to aider.
    *   When aider sees “AI!” it reads and follows all the instructions in AI comments.
*   Support for new Amazon Bedrock Nova models.
*   When `/run` or `/test` have non-zero exit codes, pre-fill “Fix that” into the next message prompt.
*   `/diff` now invokes `git diff` to use your preferred diff tool.
*   Added Ctrl-Z support for process suspension.
*   Spinner now falls back to ASCII art if fancy symbols throw unicode errors.
*   `--read` now expands `~` home dirs.
*   Enabled exception capture in analytics.
*   [Aider wrote 61% of the code in this release.](https://aider.chat/HISTORY.html)

### [](#aider-v0660)Aider v0.66.0

*   PDF support for Sonnet and Gemini models.
*   Added `--voice-input-device` to select audio input device for voice recording, by @preynal.
*   Added `--timeout` option to configure API call timeouts.
*   Set cwd to repo root when running shell commands.
*   Added Ctrl-Up/Down keyboard shortcuts for per-message history navigation.
*   Improved error handling for failed .gitignore file operations.
*   Improved error handling for input history file permissions.
*   Improved error handling for analytics file access.
*   Removed spurious warning about disabling pretty in VSCode.
*   Removed broken support for Dart.
*   Bugfix when scraping URLs found in chat messages.
*   Better handling of **version** import errors.
*   Improved `/drop` command to support substring matching for non-glob patterns.
*   Aider wrote 82% of the code in this release.

### [](#aider-v0651)Aider v0.65.1

*   Bugfix to `--alias`.

### [](#aider-v0650)Aider v0.65.0

*   Added `--alias` config to define [custom model aliases](https://aider.chat/docs/config/model-aliases.html).
*   Added `--[no-]detect-urls` flag to disable detecting and offering to scrape URLs found in the chat.
*   Ollama models now default to an 8k context window.
*   Added [RepoMap support for Dart language](https://aider.chat/docs/languages.html) by @malkoG.
*   Ask 2.5% of users if they want to opt-in to [analytics](https://aider.chat/docs/more/analytics.html).
*   Skip suggesting files that share names with files already in chat.
*   `/editor` returns and prefill the file content into the prompt, so you can use `/editor` to compose messages that start with `/commands`, etc.
*   Enhanced error handling for analytics.
*   Improved handling of UnknownEditFormat exceptions with helpful documentation links.
*   Bumped dependencies to pick up grep-ast 0.4.0 for Dart language support.
*   Aider wrote 81% of the code in this release.

### [](#aider-v0641)Aider v0.64.1

*   Disable streaming for o1 on OpenRouter.

### [](#aider-v0640)Aider v0.64.0

*   Added [`/editor` command](https://aider.chat/docs/usage/commands.html) to open system editor for writing prompts, by @thehunmonkgroup.
*   Full support for `gpt-4o-2024-11-20`.
*   Stream o1 models by default.
*   `/run` and suggested shell commands are less mysterious and now confirm that they “Added XX lines of output to the chat.”
*   Ask 1% of users if they want to opt-in to [analytics](https://aider.chat/docs/more/analytics.html).
*   Added support for [optional multiline input tags](https://aider.chat/docs/usage/commands.html#entering-multi-line-chat-messages) with matching closing tags.
*   Improved [model settings configuration](https://aider.chat/docs/config/adv-model-settings.html#global-extra-params) with support for global `extra_params` for `litellm.completion()`.
*   Architect mode now asks to add files suggested by the LLM.
*   Fixed bug in fuzzy model name matching.
*   Added Timeout exception to handle API provider timeouts.
*   Added `--show-release-notes` to control release notes display on first run of new version.
*   Save empty dict to cache file on model metadata download failure, to delay retry.
*   Improved error handling and code formatting.
*   Aider wrote 74% of the code in this release.

### [](#aider-v0632)Aider v0.63.2

*   Fixed bug in fuzzy model name matching when litellm provider info is missing.
*   Modified model metadata file loading to allow override of resource file.
*   Allow recursive loading of dirs using `--read`.
*   Updated dependency versions to pick up litellm fix for ollama models.
*   Added exponential backoff retry when writing files to handle editor file locks.
*   Updated Qwen 2.5 Coder 32B model configuration.

### [](#aider-v0631)Aider v0.63.1

*   Fixed bug in git ignored file handling.
*   Improved error handling for git operations.

### [](#aider-v0630)Aider v0.63.0

*   Support for Qwen 2.5 Coder 32B.
*   `/web` command just adds the page to the chat, without triggering an LLM response.
*   Improved prompting for the user’s preferred chat language.
*   Improved handling of LiteLLM exceptions.
*   Bugfix for double-counting tokens when reporting cache stats.
*   Bugfix for the LLM creating new files.
*   Other small bug fixes.
*   Aider wrote 55% of the code in this release.

### [](#aider-v0620)Aider v0.62.0

*   Full support for Claude 3.5 Haiku
    *   Scored 75% on [aider’s code editing leaderboard](https://aider.chat/docs/leaderboards/).
    *   Almost as good as Sonnet at much lower cost.
    *   Launch with `--haiku` to use it.
*   Easily apply file edits from ChatGPT, Claude or other web apps
    *   Chat with ChatGPT or Claude via their web app.
    *   Give it your source files and ask for the changes you want.
    *   Use the web app’s “copy response” button to copy the entire reply from the LLM.
    *   Run `aider --apply-clipboard-edits file-to-edit.js`.
    *   Aider will edit your file with the LLM’s changes.
*   Bugfix for creating new files.
*   Aider wrote 84% of the code in this release.

### [](#aider-v0610)Aider v0.61.0

*   Load and save aider slash-commands to files:
    *   `/save <fname>` command will make a file of `/add` and `/read-only` commands that recreate the current file context in the chat.
    *   `/load <fname>` will replay the commands in the file.
    *   You can use `/load` to run any arbitrary set of slash-commands, not just `/add` and `/read-only`.
    *   Use `--load <fname>` to run a list of commands on launch, before the interactive chat begins.
*   Anonymous, opt-in [analytics](https://aider.chat/docs/more/analytics.html) with no personal data sharing.
*   Aider follows litellm’s `supports_vision` attribute to enable image support for models.
*   Bugfix for when diff mode flexibly handles the model using the wrong filename.
*   Displays filenames in sorted order for `/add` and `/read-only`.
*   New `--no-fancy-input` switch disables prompt toolkit input, now still available with `--no-pretty`.
*   Override browser config with `--no-browser` or `--no-gui`.
*   Offer to open documentation URLs when errors occur.
*   Properly support all o1 models, regardless of provider.
*   Improved layout of filenames above input prompt.
*   Better handle corrupted repomap tags cache.
*   Improved handling of API errors, especially when accessing the weak model.
*   Aider wrote 68% of the code in this release.

### [](#aider-v0601)Aider v0.60.1

*   Enable image support for Sonnet 10/22.
*   Display filenames in sorted order.

### [](#aider-v0600)Aider v0.60.0

*   Full support for Sonnet 10/22, the new SOTA model on aider’s code editing benchmark.
    *   Aider uses Sonnet 10/22 by default.
*   Improved formatting of added and read-only files above chat prompt, by @jbellis.
*   Improved support for o1 models by more flexibly parsing their nonconforming code edit replies.
*   Corrected diff edit format prompt that only the first match is replaced.
*   Stronger whole edit format prompt asking for clean file names.
*   Now offers to add `.env` to the `.gitignore` file.
*   Ships with a small model metadata json file to handle models not yet updated in litellm.
*   Model settings for o1 models on azure.
*   Bugfix to properly include URLs in `/help` RAG results.
*   Aider wrote 49% of the code in this release.

### [](#aider-v0591)Aider v0.59.1

*   Check for obsolete `yes: true` in yaml config, show helpful error.
*   Model settings for openrouter/anthropic/claude-3.5-sonnet:beta

### [](#aider-v0590)Aider v0.59.0

*   Improvements to `/read-only`:
    *   Now supports shell-style auto-complete of the full file system.
    *   Still auto-completes the full paths of the repo files like `/add`.
    *   Now supports globs like `src/**/*.py`
*   Renamed `--yes` to `--yes-always`.
    *   Now uses `AIDER_YES_ALWAYS` env var and `yes-always:` yaml key.
    *   Existing YAML and .env files will need to be updated.
    *   Can still abbreviate to `--yes` on the command line.
*   Config file now uses standard YAML list syntax with \` - list entries\`, one per line.
*   `/settings` now includes the same announcement lines that would print at launch.
*   Sanity checks the `--editor-model` on launch now, same as main and weak models.
*   Added `--skip-sanity-check-repo` switch to speedup launch in large repos.
*   Bugfix so architect mode handles Control-C properly.
*   Repo-map is deterministic now, with improved caching logic.
*   Improved commit message prompt.
*   Aider wrote 77% of the code in this release.

### [](#aider-v0581)Aider v0.58.1

*   Fixed bug where cache warming pings caused subsequent user messages to trigger a tight loop of LLM requests.

### [](#aider-v0580)Aider v0.58.0

*   [Use a pair of Architect/Editor models for improved coding](https://aider.chat/2024/09/26/architect.html)
    *   Use a strong reasoning model like o1-preview as your Architect.
    *   Use a cheaper, faster model like gpt-4o as your Editor.
*   New `--o1-preview` and `--o1-mini` shortcuts.
*   Support for new Gemini 002 models.
*   Better support for Qwen 2.5 models.
*   Many confirmation questions can be skipped for the rest of the session with “(D)on’t ask again” response.
*   Autocomplete for `/read-only` supports the entire filesystem.
*   New settings for completion menu colors.
*   New `/copy` command to copy the last LLM response to the clipboard.
*   Renamed `/clipboard` to `/paste`.
*   Will now follow HTTP redirects when scraping urls.
*   New `--voice-format` switch to send voice audio as wav/mp3/webm, by @mbailey.
*   ModelSettings takes `extra_params` dict to specify any extras to pass to `litellm.completion()`.
*   Support for cursor shapes when in vim mode.
*   Numerous bug fixes.
*   Aider wrote 53% of the code in this release.

### [](#aider-v0571)Aider v0.57.1

*   Fixed dependency conflict between aider-chat\[help\] and \[playwright\].

### [](#aider-v0570)Aider v0.57.0

*   Support for OpenAI o1 models:
    *   o1-preview now works well with diff edit format.
    *   o1-preview with diff now matches SOTA leaderboard result with whole edit format.
    *   `aider --model o1-mini`
    *   `aider --model o1-preview`
*   On Windows, `/run` correctly uses PowerShell or cmd.exe.
*   Support for new 08-2024 Cohere models, by @jalammar.
*   Can now recursively add directories with `/read-only`.
*   User input prompts now fall back to simple `input()` if `--no-pretty` or a Windows console is not available.
*   Improved sanity check of git repo on startup.
*   Improvements to prompt cache chunking strategy.
*   Removed “No changes made to git tracked files”.
*   Numerous bug fixes for corner case crashes.
*   Updated all dependency versions.
*   Aider wrote 70% of the code in this release.

### [](#aider-v0560)Aider v0.56.0

*   Enables prompt caching for Sonnet via OpenRouter by @fry69
*   Enables 8k output tokens for Sonnet via VertexAI and DeepSeek V2.5.
*   New `/report` command to open your browser with a pre-populated GitHub Issue.
*   New `--chat-language` switch to set the spoken language.
*   Now `--[no-]suggest-shell-commands` controls both prompting for and offering to execute shell commands.
*   Check key imports on launch, provide helpful error message if dependencies aren’t available.
*   Renamed `--models` to `--list-models` by @fry69.
*   Numerous bug fixes for corner case crashes.
*   Aider wrote 56% of the code in this release.

### [](#aider-v0550)Aider v0.55.0

*   Only print the pip command when self updating on Windows, without running it.
*   Converted many error messages to warning messages.
*   Added `--tool-warning-color` setting.
*   Blanket catch and handle git errors in any `/command`.
*   Catch and handle glob errors in `/add`, errors writing files.
*   Disabled built in linter for typescript.
*   Catch and handle terminals which don’t support pretty output.
*   Catch and handle playwright and pandoc errors.
*   Catch `/voice` transcription exceptions, show the WAV file so the user can recover it.
*   Aider wrote 53% of the code in this release.

### [](#aider-v05412)Aider v0.54.12

*   Switched to `vX.Y.Z.dev` version naming.

### [](#aider-v05411)Aider v0.54.11

*   Improved printed pip command output on Windows.

### [](#aider-v05410)Aider v0.54.10

*   Bugfix to test command in platform info.

### [](#aider-v0549)Aider v0.54.9

*   Include important devops files in the repomap.
*   Print quoted pip install commands to the user.
*   Adopt setuptools\_scm to provide dev versions with git hashes.
*   Share active test and lint commands with the LLM.
*   Catch and handle most errors creating new files, reading existing files.
*   Catch and handle most git errors.
*   Added –verbose debug output for shell commands.

### [](#aider-v0548)Aider v0.54.8

*   Startup QOL improvements:
    *   Sanity check the git repo and exit gracefully on problems.
    *   Pause for confirmation after model sanity check to allow user to review warnings.
*   Bug fix for shell commands on Windows.
*   Do not fuzzy match filenames when LLM is creating a new file, by @ozapinq
*   Numerous corner case bug fixes submitted via new crash report -> GitHub Issue feature.
*   Crash reports now include python version, OS, etc.

### [](#aider-v0547)Aider v0.54.7

*   Offer to submit a GitHub issue pre-filled with uncaught exception info.
*   Bugfix for infinite output.

### [](#aider-v0546)Aider v0.54.6

*   New `/settings` command to show active settings.
*   Only show cache warming status update if `--verbose`.

### [](#aider-v0545)Aider v0.54.5

*   Bugfix for shell commands on Windows.
*   Refuse to make git repo in $HOME, warn user.
*   Don’t ask again in current session about a file the user has said not to add to the chat.
*   Added `--update` as an alias for `--upgrade`.

### [](#aider-v0544)Aider v0.54.4

*   Bugfix to completions for `/model` command.
*   Bugfix: revert home dir special case.

### [](#aider-v0543)Aider v0.54.3

*   Dependency `watchdog<5` for docker image.

### [](#aider-v0542)Aider v0.54.2

*   When users launch aider in their home dir, help them find/create a repo in a subdir.
*   Added missing `pexpect` dependency.

### [](#aider-v0540)Aider v0.54.0

*   Added model settings for `gemini/gemini-1.5-pro-exp-0827` and `gemini/gemini-1.5-flash-exp-0827`.
*   Shell and `/run` commands can now be interactive in environments where a pty is available.
*   Optionally share output of suggested shell commands back to the LLM.
*   New `--[no-]suggest-shell-commands` switch to configure shell commands.
*   Performance improvements for autocomplete in large/mono repos.
*   New `--upgrade` switch to install latest version of aider from pypi.
*   Bugfix to `--show-prompt`.
*   Disabled automatic reply to the LLM on `/undo` for all models.
*   Removed pager from `/web` output.
*   Aider wrote 64% of the code in this release.

### [](#aider-v0530)Aider v0.53.0

*   [Keep your prompt cache from expiring](https://aider.chat/docs/usage/caching.html#preventing-cache-expiration) with `--cache-keepalive-pings`.
    *   Pings the API every 5min to keep the cache warm.
*   You can now bulk accept/reject a series of add url and run shell confirmations.
*   Improved matching of filenames from S/R blocks with files in chat.
*   Stronger prompting for Sonnet to make edits in code chat mode.
*   Stronger prompting for the LLM to specify full file paths.
*   Improved shell command prompting.
*   Weak model now uses `extra_headers`, to support Anthropic beta features.
*   New `--install-main-branch` to update to the latest dev version of aider.
*   Improved error messages on attempt to add not-git subdir to chat.
*   Show model metadata info on `--verbose`.
*   Improved warnings when LLMs env variables aren’t set.
*   Bugfix to windows filenames which contain `\_`.
*   Aider wrote 59% of the code in this release.

### [](#aider-v0521)Aider v0.52.1

*   Bugfix for NameError when applying edits.

### [](#aider-v0520)Aider v0.52.0

*   Aider now offers to run shell commands:
    *   Launch a browser to view updated html/css/js.
    *   Install new dependencies.
    *   Run DB migrations.
    *   Run the program to exercise changes.
    *   Run new test cases.
*   `/read` and `/drop` now expand `~` to the home dir.
*   Show the active chat mode at aider prompt.
*   New `/reset` command to `/drop` files and `/clear` chat history.
*   New `--map-multiplier-no-files` to control repo map size multiplier when no files are in the chat.
    *   Reduced default multiplier to 2.
*   Bugfixes and improvements to auto commit sequencing.
*   Improved formatting of token reports and confirmation dialogs.
*   Default OpenAI model is now `gpt-4o-2024-08-06`.
*   Bumped dependencies to pickup litellm bugfixes.
*   Aider wrote 68% of the code in this release.

### [](#aider-v0510)Aider v0.51.0

*   Prompt caching for Anthropic models with `--cache-prompts`.
    *   Caches the system prompt, repo map and `/read-only` files.
*   Repo map recomputes less often in large/mono repos or when caching enabled.
    *   Use `--map-refresh <always|files|manual|auto>` to configure.
*   Improved cost estimate logic for caching.
*   Improved editing performance on Jupyter Notebook `.ipynb` files.
*   Show which config yaml file is loaded with `--verbose`.
*   Bumped dependency versions.
*   Bugfix: properly load `.aider.models.metadata.json` data.
*   Bugfix: Using `--msg /ask ...` caused an exception.
*   Bugfix: litellm tokenizer bug for images.
*   Aider wrote 56% of the code in this release.

### [](#aider-v0501)Aider v0.50.1

*   Bugfix for provider API exceptions.

### [](#aider-v0500)Aider v0.50.0

*   Infinite output for DeepSeek Coder, Mistral models in addition to Anthropic’s models.
*   New `--deepseek` switch to use DeepSeek Coder.
*   DeepSeek Coder uses 8k token output.
*   New `--chat-mode <mode>` switch to launch in ask/help/code modes.
*   New `/code <message>` command request a code edit while in `ask` mode.
*   Web scraper is more robust if page never idles.
*   Improved token and cost reporting for infinite output.
*   Improvements and bug fixes for `/read` only files.
*   Switched from `setup.py` to `pyproject.toml`, by @branchvincent.
*   Bug fix to persist files added during `/ask`.
*   Bug fix for chat history size in `/tokens`.
*   Aider wrote 66% of the code in this release.

### [](#aider-v0491)Aider v0.49.1

*   Bugfix to `/help`.

### [](#aider-v0490)Aider v0.49.0

*   Add read-only files to the chat context with `/read` and `--read`, including from outside the git repo.
*   `/diff` now shows diffs of all changes resulting from your request, including lint and test fixes.
*   New `/clipboard` command to paste images or text from the clipboard, replaces `/add-clipboard-image`.
*   Now shows the markdown scraped when you add a url with `/web`.
*   When [scripting aider](https://aider.chat/docs/scripting.html) messages can now contain in-chat `/` commands.
*   Aider in docker image now suggests the correct command to update to latest version.
*   Improved retries on API errors (was easy to test during Sonnet outage).
*   Added `--mini` for `gpt-4o-mini`.
*   Bugfix to keep session cost accurate when using `/ask` and `/help`.
*   Performance improvements for repo map calculation.
*   `/tokens` now shows the active model.
*   Enhanced commit message attribution options:
    *   New `--attribute-commit-message-author` to prefix commit messages with ‘aider: ‘ if aider authored the changes, replaces `--attribute-commit-message`.
    *   New `--attribute-commit-message-committer` to prefix all commit messages with ‘aider: ‘.
*   Aider wrote 61% of the code in this release.

### [](#aider-v0481)Aider v0.48.1

*   Added `openai/gpt-4o-2024-08-06`.
*   Worked around litellm bug that removes OpenRouter app headers when using `extra_headers`.
*   Improved progress indication during repo map processing.
*   Corrected instructions for upgrading the docker container to latest aider version.
*   Removed obsolete 16k token limit on commit diffs, use per-model limits.

### [](#aider-v0480)Aider v0.48.0

*   Performance improvements for large/mono repos.
*   Added `--subtree-only` to limit aider to current directory subtree.
    *   Should help with large/mono repo performance.
*   New `/add-clipboard-image` to add images to the chat from your clipboard.
*   Use `--map-tokens 1024` to use repo map with any model.
*   Support for Sonnet’s 8k output window.
    *   [Aider already supported infinite output from Sonnet.](https://aider.chat/2024/07/01/sonnet-not-lazy.html)
*   Workaround litellm bug for retrying API server errors.
*   Upgraded dependencies, to pick up litellm bug fixes.
*   Aider wrote 44% of the code in this release.

### [](#aider-v0471)Aider v0.47.1

*   Improvements to conventional commits prompting.

### [](#aider-v0470)Aider v0.47.0

*   [Commit message](https://aider.chat/docs/git.html#commit-messages) improvements:
    *   Added Conventional Commits guidelines to commit message prompt.
    *   Added `--commit-prompt` to customize the commit message prompt.
    *   Added strong model as a fallback for commit messages (and chat summaries).
*   [Linting](https://aider.chat/docs/usage/lint-test.html) improvements:
    *   Ask before fixing lint errors.
    *   Improved performance of `--lint` on all dirty files in repo.
    *   Improved lint flow, now doing code edit auto-commit before linting.
    *   Bugfix to properly handle subprocess encodings (also for `/run`).
*   Improved [docker support](https://aider.chat/docs/install/docker.html):
    *   Resolved permission issues when using `docker run --user xxx`.
    *   New `paulgauthier/aider-full` docker image, which includes all extras.
*   Switching to code and ask mode no longer summarizes the chat history.
*   Added graph of aider’s contribution to each release.
*   Generic auto-completions are provided for `/commands` without a completion override.
*   Fixed broken OCaml tags file.
*   Bugfix in `/run` add to chat approval logic.
*   Aider wrote 58% of the code in this release.

### [](#aider-v0461)Aider v0.46.1

*   Downgraded stray numpy dependency back to 1.26.4.

### [](#aider-v0460)Aider v0.46.0

*   New `/ask <question>` command to ask about your code, without making any edits.
*   New `/chat-mode <mode>` command to switch chat modes:
    *   ask: Ask questions about your code without making any changes.
    *   code: Ask for changes to your code (using the best edit format).
    *   help: Get help about using aider (usage, config, troubleshoot).
*   Add `file: CONVENTIONS.md` to `.aider.conf.yml` to always load a specific file.
    *   Or `file: [file1, file2, file3]` to always load multiple files.
*   Enhanced token usage and cost reporting. Now works when streaming too.
*   Filename auto-complete for `/add` and `/drop` is now case-insensitive.
*   Commit message improvements:
    *   Updated commit message prompt to use imperative tense.
    *   Fall back to main model if weak model is unable to generate a commit message.
*   Stop aider from asking to add the same url to the chat multiple times.
*   Updates and fixes to `--no-verify-ssl`:
    *   Fixed regression that broke it in v0.42.0.
    *   Disables SSL certificate verification when `/web` scrapes websites.
*   Improved error handling and reporting in `/web` scraping functionality
*   Fixed syntax error in Elm’s tree-sitter scm file (by @cjoach).
*   Handle UnicodeEncodeError when streaming text to the terminal.
*   Updated dependencies to latest versions.
*   Aider wrote 45% of the code in this release.

### [](#aider-v0451)Aider v0.45.1

*   Use 4o-mini as the weak model wherever 3.5-turbo was used.

### [](#aider-v0450)Aider v0.45.0

*   GPT-4o mini scores similar to the original GPT 3.5, using whole edit format.
*   Aider is better at offering to add files to the chat on Windows.
*   Bugfix corner cases for `/undo` with new files or new repos.
*   Now shows last 4 characters of API keys in `--verbose` output.
*   Bugfix to precedence of multiple `.env` files.
*   Bugfix to gracefully handle HTTP errors when installing pandoc.
*   Aider wrote 42% of the code in this release.

### [](#aider-v0440)Aider v0.44.0

*   Default pip install size reduced by 3-12x.
*   Added 3 package extras, which aider will offer to install when needed:
    *   `aider-chat[help]`
    *   `aider-chat[browser]`
    *   `aider-chat[playwright]`
*   Improved regex for detecting URLs in user chat messages.
*   Bugfix to globbing logic when absolute paths are included in `/add`.
*   Simplified output of `--models`.
*   The `--check-update` switch was renamed to `--just-check-updated`.
*   The `--skip-check-update` switch was renamed to `--[no-]check-update`.
*   Aider wrote 29% of the code in this release (157/547 lines).

### [](#aider-v0434)Aider v0.43.4

*   Added scipy back to main requirements.txt.

### [](#aider-v0433)Aider v0.43.3

*   Added build-essentials back to main Dockerfile.

### [](#aider-v0432)Aider v0.43.2

*   Moved HuggingFace embeddings deps into \[hf-embed\] extra.
*   Added \[dev\] extra.

### [](#aider-v0431)Aider v0.43.1

*   Replace the torch requirement with the CPU only version, because the GPU versions are huge.

### [](#aider-v0430)Aider v0.43.0

*   Use `/help <question>` to [ask for help about using aider](https://aider.chat/docs/troubleshooting/support.html), customizing settings, troubleshooting, using LLMs, etc.
*   Allow multiple use of `/undo`.
*   All config/env/yml/json files now load from home, git root, cwd and named command line switch.
*   New `$HOME/.aider/caches` dir for app-wide expendable caches.
*   Default `--model-settings-file` is now `.aider.model.settings.yml`.
*   Default `--model-metadata-file` is now `.aider.model.metadata.json`.
*   Bugfix affecting launch with `--no-git`.
*   Aider wrote 9% of the 424 lines edited in this release.

### [](#aider-v0420)Aider v0.42.0

*   Performance release:
    *   5X faster launch!
    *   Faster auto-complete in large git repos (users report ~100X speedup)!

### [](#aider-v0410)Aider v0.41.0

*   [Allow Claude 3.5 Sonnet to stream back >4k tokens!](https://aider.chat/2024/07/01/sonnet-not-lazy.html)
    *   It is the first model capable of writing such large coherent, useful code edits.
    *   Do large refactors or generate multiple files of new code in one go.
*   Aider now uses `claude-3-5-sonnet-20240620` by default if `ANTHROPIC_API_KEY` is set in the environment.
*   [Enabled image support](https://aider.chat/docs/usage/images-urls.html) for 3.5 Sonnet and for GPT-4o & 3.5 Sonnet via OpenRouter (by @yamitzky).
*   Added `--attribute-commit-message` to prefix aider’s commit messages with “aider:”.
*   Fixed regression in quality of one-line commit messages.
*   Automatically retry on Anthropic `overloaded_error`.
*   Bumped dependency versions.

### [](#aider-v0406)Aider v0.40.6

*   Fixed `/undo` so it works regardless of `--attribute` settings.

### [](#aider-v0405)Aider v0.40.5

*   Bump versions to pickup latest litellm to fix streaming issue with Gemini
    *   https://github.com/BerriAI/litellm/issues/4408

### [](#aider-v0401)Aider v0.40.1

*   Improved context awareness of repomap.
*   Restored proper `--help` functionality.

### [](#aider-v0400)Aider v0.40.0

*   Improved prompting to discourage Sonnet from wasting tokens emitting unchanging code (#705).
*   Improved error info for token limit errors.
*   Options to suppress adding “(aider)” to the [git author and committer names](https://aider.chat/docs/git.html#commit-attribution).
*   Use `--model-settings-file` to customize per-model settings, like use of repo-map (by @caseymcc).
*   Improved invocation of flake8 linter for python code.

### [](#aider-v0390)Aider v0.39.0

*   Use `--sonnet` for Claude 3.5 Sonnet, which is the top model on [aider’s LLM code editing leaderboard](https://aider.chat/docs/leaderboards/#claude-35-sonnet-takes-the-top-spot).
*   All `AIDER_xxx` environment variables can now be set in `.env` (by @jpshack-at-palomar).
*   Use `--llm-history-file` to log raw messages sent to the LLM (by @daniel-vainsencher).
*   Commit messages are no longer prefixed with “aider:”. Instead the git author and committer names have “(aider)” added.

### [](#aider-v0380)Aider v0.38.0

*   Use `--vim` for [vim keybindings](https://aider.chat/docs/usage/commands.html#vi) in the chat.
*   [Add LLM metadata](https://aider.chat/docs/llms/warnings.html#specifying-context-window-size-and-token-costs) via `.aider.models.json` file (by @caseymcc).
*   More detailed [error messages on token limit errors](https://aider.chat/docs/troubleshooting/token-limits.html).
*   Single line commit messages, without the recent chat messages.
*   Ensure `--commit --dry-run` does nothing.
*   Have playwright wait for idle network to better scrape js sites.
*   Documentation updates, moved into website/ subdir.
*   Moved tests/ into aider/tests/.

### [](#aider-v0370)Aider v0.37.0

*   Repo map is now optimized based on text of chat history as well as files added to chat.
*   Improved prompts when no files have been added to chat to solicit LLM file suggestions.
*   Aider will notice if you paste a URL into the chat, and offer to scrape it.
*   Performance improvements the repo map, especially in large repos.
*   Aider will not offer to add bare filenames like `make` or `run` which may just be words.
*   Properly override `GIT_EDITOR` env for commits if it is already set.
*   Detect supported audio sample rates for `/voice`.
*   Other small bug fixes.

### [](#aider-v0360)Aider v0.36.0

*   [Aider can now lint your code and fix any errors](https://aider.chat/2024/05/22/linting.html).
    *   Aider automatically lints and fixes after every LLM edit.
    *   You can manually lint-and-fix files with `/lint` in the chat or `--lint` on the command line.
    *   Aider includes built in basic linters for all supported tree-sitter languages.
    *   You can also configure aider to use your preferred linter with `--lint-cmd`.
*   Aider has additional support for running tests and fixing problems.
    *   Configure your testing command with `--test-cmd`.
    *   Run tests with `/test` or from the command line with `--test`.
    *   Aider will automatically attempt to fix any test failures.

### [](#aider-v0350)Aider v0.35.0

*   Aider now uses GPT-4o by default.
    *   GPT-4o tops the [aider LLM code editing leaderboard](https://aider.chat/docs/leaderboards/) at 72.9%, versus 68.4% for Opus.
    *   GPT-4o takes second on [aider’s refactoring leaderboard](https://aider.chat/docs/leaderboards/#code-refactoring-leaderboard) with 62.9%, versus Opus at 72.3%.
*   Added `--restore-chat-history` to restore prior chat history on launch, so you can continue the last conversation.
*   Improved reflection feedback to LLMs using the diff edit format.
*   Improved retries on `httpx` errors.

### [](#aider-v0340)Aider v0.34.0

*   Updated prompting to use more natural phrasing about files, the git repo, etc. Removed reliance on read-write/read-only terminology.
*   Refactored prompting to unify some phrasing across edit formats.
*   Enhanced the canned assistant responses used in prompts.
*   Added explicit model settings for `openrouter/anthropic/claude-3-opus`, `gpt-3.5-turbo`
*   Added `--show-prompts` debug switch.
*   Bugfix: catch and retry on all litellm exceptions.

### [](#aider-v0330)Aider v0.33.0

*   Added native support for [Deepseek models](https://aider.chat/docs/llms.html#deepseek) using `DEEPSEEK_API_KEY` and `deepseek/deepseek-chat`, etc rather than as a generic OpenAI compatible API.

### [](#aider-v0320)Aider v0.32.0

*   [Aider LLM code editing leaderboards](https://aider.chat/docs/leaderboards/) that rank popular models according to their ability to edit code.
    *   Leaderboards include GPT-3.5/4 Turbo, Opus, Sonnet, Gemini 1.5 Pro, Llama 3, Deepseek Coder & Command-R+.
*   Gemini 1.5 Pro now defaults to a new diff-style edit format (diff-fenced), enabling it to work better with larger code bases.
*   Support for Deepseek-V2, via more a flexible config of system messages in the diff edit format.
*   Improved retry handling on errors from model APIs.
*   Benchmark outputs results in YAML, compatible with leaderboard.

### [](#aider-v0310)Aider v0.31.0

*   [Aider is now also AI pair programming in your browser!](https://aider.chat/2024/05/02/browser.html) Use the `--browser` switch to launch an experimental browser based version of aider.
*   Switch models during the chat with `/model <name>` and search the list of available models with `/models <query>`.

### [](#aider-v0301)Aider v0.30.1

*   Adding missing `google-generativeai` dependency

### [](#aider-v0300)Aider v0.30.0

*   Added [Gemini 1.5 Pro](https://aider.chat/docs/llms.html#free-models) as a recommended free model.
*   Allow repo map for “whole” edit format.
*   Added `--models <MODEL-NAME>` to search the available models.
*   Added `--no-show-model-warnings` to silence model warnings.

### [](#aider-v0292)Aider v0.29.2

*   Improved [model warnings](https://aider.chat/docs/llms.html#model-warnings) for unknown or unfamiliar models

### [](#aider-v0291)Aider v0.29.1

*   Added better support for groq/llama3-70b-8192

### [](#aider-v0290)Aider v0.29.0

*   Added support for [directly connecting to Anthropic, Cohere, Gemini and many other LLM providers](https://aider.chat/docs/llms.html).
*   Added `--weak-model <model-name>` which allows you to specify which model to use for commit messages and chat history summarization.
*   New command line switches for working with popular models:
    *   `--4-turbo-vision`
    *   `--opus`
    *   `--sonnet`
    *   `--anthropic-api-key`
*   Improved “whole” and “diff” backends to better support [Cohere’s free to use Command-R+ model](https://aider.chat/docs/llms.html#cohere).
*   Allow `/add` of images from anywhere in the filesystem.
*   Fixed crash when operating in a repo in a detached HEAD state.
*   Fix: Use the same default model in CLI and python scripting.

### [](#aider-v0280)Aider v0.28.0

*   Added support for new `gpt-4-turbo-2024-04-09` and `gpt-4-turbo` models.
    *   Benchmarked at 61.7% on Exercism benchmark, comparable to `gpt-4-0613` and worse than the `gpt-4-preview-XXXX` models. See [recent Exercism benchmark results](https://aider.chat/2024/03/08/claude-3.html).
    *   Benchmarked at 34.1% on the refactoring/laziness benchmark, significantly worse than the `gpt-4-preview-XXXX` models. See [recent refactor bencmark results](https://aider.chat/2024/01/25/benchmarks-0125.html).
    *   Aider continues to default to `gpt-4-1106-preview` as it performs best on both benchmarks, and significantly better on the refactoring/laziness benchmark.

### [](#aider-v0270)Aider v0.27.0

*   Improved repomap support for typescript, by @ryanfreckleton.
*   Bugfix: Only /undo the files which were part of the last commit, don’t stomp other dirty files
*   Bugfix: Show clear error message when OpenAI API key is not set.
*   Bugfix: Catch error for obscure languages without tags.scm file.

### [](#aider-v0261)Aider v0.26.1

*   Fixed bug affecting parsing of git config in some environments.

### [](#aider-v0260)Aider v0.26.0

*   Use GPT-4 Turbo by default.
*   Added `-3` and `-4` switches to use GPT 3.5 or GPT-4 (non-Turbo).
*   Bug fix to avoid reflecting local git errors back to GPT.
*   Improved logic for opening git repo on launch.

### [](#aider-v0250)Aider v0.25.0

*   Issue a warning if user adds too much code to the chat.
    *   https://aider.chat/docs/faq.html#how-can-i-add-all-the-files-to-the-chat
*   Vocally refuse to add files to the chat that match `.aiderignore`
    *   Prevents bug where subsequent git commit of those files will fail.
*   Added `--openai-organization-id` argument.
*   Show the user a FAQ link if edits fail to apply.
*   Made past articles part of https://aider.chat/blog/

### [](#aider-v0241)Aider v0.24.1

*   Fixed bug with cost computations when –no-steam in effect

### [](#aider-v0240)Aider v0.24.0

*   New `/web <url>` command which scrapes the url, turns it into fairly clean markdown and adds it to the chat.
*   Updated all OpenAI model names, pricing info
*   Default GPT 3.5 model is now `gpt-3.5-turbo-0125`.
*   Bugfix to the `!` alias for `/run`.

### [](#aider-v0230)Aider v0.23.0

*   Added support for `--model gpt-4-0125-preview` and OpenAI’s alias `--model gpt-4-turbo-preview`. The `--4turbo` switch remains an alias for `--model gpt-4-1106-preview` at this time.
*   New `/test` command that runs a command and adds the output to the chat on non-zero exit status.
*   Improved streaming of markdown to the terminal.
*   Added `/quit` as alias for `/exit`.
*   Added `--skip-check-update` to skip checking for the update on launch.
*   Added `--openrouter` as a shortcut for `--openai-api-base https://openrouter.ai/api/v1`
*   Fixed bug preventing use of env vars `OPENAI_API_BASE, OPENAI_API_TYPE, OPENAI_API_VERSION, OPENAI_API_DEPLOYMENT_ID`.

### [](#aider-v0220)Aider v0.22.0

*   Improvements for unified diff editing format.
*   Added ! as an alias for /run.
*   Autocomplete for /add and /drop now properly quotes filenames with spaces.
*   The /undo command asks GPT not to just retry reverted edit.

### [](#aider-v0211)Aider v0.21.1

*   Bugfix for unified diff editing format.
*   Added –4turbo and –4 aliases for –4-turbo.

### [](#aider-v0210)Aider v0.21.0

*   Support for python 3.12.
*   Improvements to unified diff editing format.
*   New `--check-update` arg to check if updates are available and exit with status code.

### [](#aider-v0200)Aider v0.20.0

*   Add images to the chat to automatically use GPT-4 Vision, by @joshuavial
    
*   Bugfixes:
    
    *   Improved unicode encoding for `/run` command output, by @ctoth
    *   Prevent false auto-commits on Windows, by @ctoth

### [](#aider-v0191)Aider v0.19.1

*   Removed stray debug output.

### [](#aider-v0190)Aider v0.19.0

*   [Significantly reduced “lazy” coding from GPT-4 Turbo due to new unified diff edit format](https://aider.chat/docs/unified-diffs.html)
    *   Score improves from 20% to 61% on new “laziness benchmark”.
    *   Aider now uses unified diffs by default for `gpt-4-1106-preview`.
*   New `--4-turbo` command line switch as a shortcut for `--model gpt-4-1106-preview`.

### [](#aider-v0181)Aider v0.18.1

*   Upgraded to new openai python client v1.3.7.

### [](#aider-v0180)Aider v0.18.0

*   Improved prompting for both GPT-4 and GPT-4 Turbo.
    *   Far fewer edit errors from GPT-4 Turbo (`gpt-4-1106-preview`).
    *   Significantly better benchmark results from the June GPT-4 (`gpt-4-0613`). Performance leaps from 47%/64% up to 51%/71%.
*   Fixed bug where in-chat files were marked as both read-only and ready-write, sometimes confusing GPT.
*   Fixed bug to properly handle repos with submodules.

### [](#aider-v0170)Aider v0.17.0

*   Support for OpenAI’s new 11/06 models:
    *   gpt-4-1106-preview with 128k context window
    *   gpt-3.5-turbo-1106 with 16k context window
*   [Benchmarks for OpenAI’s new 11/06 models](https://aider.chat/docs/benchmarks-1106.html)
*   Streamlined [API for scripting aider, added docs](https://aider.chat/docs/faq.html#can-i-script-aider)
*   Ask for more concise SEARCH/REPLACE blocks. [Benchmarked](https://aider.chat/docs/benchmarks.html) at 63.9%, no regression.
*   Improved repo-map support for elisp.
*   Fixed crash bug when `/add` used on file matching `.gitignore`
*   Fixed misc bugs to catch and handle unicode decoding errors.

### [](#aider-v0163)Aider v0.16.3

*   Fixed repo-map support for C#.

### [](#aider-v0162)Aider v0.16.2

*   Fixed docker image.

### [](#aider-v0161)Aider v0.16.1

*   Updated tree-sitter dependencies to streamline the pip install process

### [](#aider-v0160)Aider v0.16.0

*   [Improved repository map using tree-sitter](https://aider.chat/docs/repomap.html)
*   Switched from “edit block” to “search/replace block”, which reduced malformed edit blocks. [Benchmarked](https://aider.chat/docs/benchmarks.html) at 66.2%, no regression.
*   Improved handling of malformed edit blocks targeting multiple edits to the same file. [Benchmarked](https://aider.chat/docs/benchmarks.html) at 65.4%, no regression.
*   Bugfix to properly handle malformed `/add` wildcards.

### [](#aider-v0150)Aider v0.15.0

*   Added support for `.aiderignore` file, which instructs aider to ignore parts of the git repo.
*   New `--commit` cmd line arg, which just commits all pending changes with a sensible commit message generated by gpt-3.5.
*   Added universal ctags and multiple architectures to the [aider docker image](https://aider.chat/docs/install/docker.html)
*   `/run` and `/git` now accept full shell commands, like: `/run (cd subdir; ls)`
*   Restored missing `--encoding` cmd line switch.

### [](#aider-v0142)Aider v0.14.2

*   Easily [run aider from a docker image](https://aider.chat/docs/install/docker.html)
*   Fixed bug with chat history summarization.
*   Fixed bug if `soundfile` package not available.

### [](#aider-v0141)Aider v0.14.1

*   /add and /drop handle absolute filenames and quoted filenames
*   /add checks to be sure files are within the git repo (or root)
*   If needed, warn users that in-chat file paths are all relative to the git repo
*   Fixed /add bug in when aider launched in repo subdir
*   Show models supported by api/key if requested model isn’t available

### [](#aider-v0140)Aider v0.14.0

*   [Support for Claude2 and other LLMs via OpenRouter](https://aider.chat/docs/faq.html#accessing-other-llms-with-openrouter) by @joshuavial
*   Documentation for [running the aider benchmarking suite](https://github.com/Aider-AI/aider/tree/main/benchmark)
*   Aider now requires Python >= 3.9

### [](#aider-v0130)Aider v0.13.0

*   [Only git commit dirty files that GPT tries to edit](https://aider.chat/docs/faq.html#how-did-v0130-change-git-usage)
*   Send chat history as prompt/context for Whisper voice transcription
*   Added `--voice-language` switch to constrain `/voice` to transcribe to a specific language
*   Late-bind importing `sounddevice`, as it was slowing down aider startup
*   Improved –foo/–no-foo switch handling for command line and yml config settings

### [](#aider-v0120)Aider v0.12.0

*   [Voice-to-code](https://aider.chat/docs/usage/voice.html) support, which allows you to code with your voice.
*   Fixed bug where /diff was causing crash.
*   Improved prompting for gpt-4, refactor of editblock coder.
*   [Benchmarked](https://aider.chat/docs/benchmarks.html) at 63.2% for gpt-4/diff, no regression.

### [](#aider-v0111)Aider v0.11.1

*   Added a progress bar when initially creating a repo map.
*   Fixed bad commit message when adding new file to empty repo.
*   Fixed corner case of pending chat history summarization when dirty committing.
*   Fixed corner case of undefined `text` when using `--no-pretty`.
*   Fixed /commit bug from repo refactor, added test coverage.
*   [Benchmarked](https://aider.chat/docs/benchmarks.html) at 53.4% for gpt-3.5/whole (no regression).

### [](#aider-v0110)Aider v0.11.0

*   Automatically summarize chat history to avoid exhausting context window.
*   More detail on dollar costs when running with `--no-stream`
*   Stronger GPT-3.5 prompt against skipping/eliding code in replies (51.9% [benchmark](https://aider.chat/docs/benchmarks.html), no regression)
*   Defend against GPT-3.5 or non-OpenAI models suggesting filenames surrounded by asterisks.
*   Refactored GitRepo code out of the Coder class.

### [](#aider-v0101)Aider v0.10.1

*   /add and /drop always use paths relative to the git root
*   Encourage GPT to use language like “add files to the chat” to ask users for permission to edit them.

### [](#aider-v0100)Aider v0.10.0

*   Added `/git` command to run git from inside aider chats.
*   Use Meta-ENTER (Esc+ENTER in some environments) to enter multiline chat messages.
*   Create a `.gitignore` with `.aider*` to prevent users from accidentally adding aider files to git.
*   Check pypi for newer versions and notify user.
*   Updated keyboard interrupt logic so that 2 ^C in 2 seconds always forces aider to exit.
*   Provide GPT with detailed error if it makes a bad edit block, ask for a retry.
*   Force `--no-pretty` if aider detects it is running inside a VSCode terminal.
*   [Benchmarked](https://aider.chat/docs/benchmarks.html) at 64.7% for gpt-4/diff (no regression)

### [](#aider-v090)Aider v0.9.0

*   Support for the OpenAI models in [Azure](https://aider.chat/docs/faq.html#azure)
*   Added `--show-repo-map`
*   Improved output when retrying connections to the OpenAI API
*   Redacted api key from `--verbose` output
*   Bugfix: recognize and add files in subdirectories mentioned by user or GPT
*   [Benchmarked](https://aider.chat/docs/benchmarks.html) at 53.8% for gpt-3.5-turbo/whole (no regression)

### [](#aider-v083)Aider v0.8.3

*   Added `--dark-mode` and `--light-mode` to select colors optimized for terminal background
*   Install docs link to [NeoVim plugin](https://github.com/joshuavial/aider.nvim) by @joshuavial
*   Reorganized the `--help` output
*   Bugfix/improvement to whole edit format, may improve coding editing for GPT-3.5
*   Bugfix and tests around git filenames with unicode characters
*   Bugfix so that aider throws an exception when OpenAI returns InvalidRequest
*   Bugfix/improvement to /add and /drop to recurse selected directories
*   Bugfix for live diff output when using “whole” edit format

### [](#aider-v082)Aider v0.8.2

*   Disabled general availability of gpt-4 (it’s rolling out, not 100% available yet)

### [](#aider-v081)Aider v0.8.1

*   Ask to create a git repo if none found, to better track GPT’s code changes
*   Glob wildcards are now supported in `/add` and `/drop` commands
*   Pass `--encoding` into ctags, require it to return `utf-8`
*   More robust handling of filepaths, to avoid 8.3 windows filenames
*   Added [FAQ](https://aider.chat/docs/faq.html)
*   Marked GPT-4 as generally available
*   Bugfix for live diffs of whole coder with missing filenames
*   Bugfix for chats with multiple files
*   Bugfix in editblock coder prompt

### [](#aider-v080)Aider v0.8.0

*   [Benchmark comparing code editing in GPT-3.5 and GPT-4](https://aider.chat/docs/benchmarks.html)
*   Improved Windows support:
    *   Fixed bugs related to path separators in Windows
    *   Added a CI step to run all tests on Windows
*   Improved handling of Unicode encoding/decoding
    *   Explicitly read/write text files with utf-8 encoding by default (mainly benefits Windows)
    *   Added `--encoding` switch to specify another encoding
    *   Gracefully handle decoding errors
*   Added `--code-theme` switch to control the pygments styling of code blocks (by @kwmiebach)
*   Better status messages explaining the reason when ctags is disabled

### [](#aider-v072)Aider v0.7.2:

*   Fixed a bug to allow aider to edit files that contain triple backtick fences.

### [](#aider-v071)Aider v0.7.1:

*   Fixed a bug in the display of streaming diffs in GPT-3.5 chats

### [](#aider-v070)Aider v0.7.0:

*   Graceful handling of context window exhaustion, including helpful tips.
*   Added `--message` to give GPT that one instruction and then exit after it replies and any edits are performed.
*   Added `--no-stream` to disable streaming GPT responses.
    *   Non-streaming responses include token usage info.
    *   Enables display of cost info based on OpenAI advertised pricing.
*   Coding competence benchmarking tool against suite of programming tasks based on Execism’s python repo.
    *   https://github.com/exercism/python
*   Major refactor in preparation for supporting new function calls api.
*   Initial implementation of a function based code editing backend for 3.5.
    *   Initial experiments show that using functions makes 3.5 less competent at coding.
*   Limit automatic retries when GPT returns a malformed edit response.

### [](#aider-v062)Aider v0.6.2

*   Support for `gpt-3.5-turbo-16k`, and all OpenAI chat models
*   Improved ability to correct when gpt-4 omits leading whitespace in code edits
*   Added `--openai-api-base` to support API proxies, etc.

### [](#aider-v050)Aider v0.5.0

*   Added support for `gpt-3.5-turbo` and `gpt-4-32k`.
*   Added `--map-tokens` to set a token budget for the repo map, along with a PageRank based algorithm for prioritizing which files and identifiers to include in the map.
*   Added in-chat command `/tokens` to report on context window token usage.
*   Added in-chat command `/clear` to clear the conversation history.

---



## [https://aider.chat/docs/leaderboards/](https://aider.chat/docs/leaderboards/)

[](#aider-llm-leaderboards)Aider LLM Leaderboards
=================================================

Aider works best with LLMs which are good at _editing_ code, not just good at writing code. To evaluate an LLM’s editing skill, aider uses benchmarks that assess a model’s ability to consistently follow the system prompt to successfully edit code.

The leaderboards report the results from a number of popular LLMs. While [aider can connect to almost any LLM](/docs/llms.html), it works best with models that score well on the benchmarks.

The [original aider code editing leaderboard](edit.html) has been replaced by this new, much more challenging [polyglot leaderboard](https://aider.chat/2024/12/21/polyglot.html).

[](#polyglot-leaderboard)Polyglot leaderboard
---------------------------------------------

[Aider’s polyglot benchmark](/docs/benchmarks.html#the-benchmark) asks the LLM to edit source files to complete 225 coding exercises from Exercism. It contains exercises in many popular programming languages: C++, Go, Java, JavaScript, Python and Rust. The 225 exercises were purposely selected to be the _hardest_ that Exercism offered in those languages, to provide a strong coding challenge to LLMs.

This benchmark measures the LLM’s coding ability in popular languages, and whether it can write new code that integrates into existing code. The model also has to successfully apply all its changes to the source file without human intervention.

Model

Percent completed correctly

Percent using correct edit format

Command

Edit format

DeepSeek R1 + claude-3-5-sonnet-20241022

64.0%

100.0%

`aider --architect --model r1 --editor-model sonnet`

architect

o1-2024-12-17 (high)

61.7%

91.5%

`aider --model openrouter/openai/o1`

diff

DeepSeek R1

56.9%

96.9%

`aider --model deepseek/deepseek-reasoner`

diff

claude-3-5-sonnet-20241022

51.6%

99.6%

`aider --model claude-3-5-sonnet-20241022`

diff

DeepSeek Chat V3

48.4%

98.7%

`aider --model deepseek/deepseek-chat`

diff

gemini-exp-1206

38.2%

98.2%

`aider --model gemini/gemini-exp-1206`

whole

o1-mini-2024-09-12

32.9%

96.9%

`aider --model o1-mini`

whole

claude-3-5-haiku-20241022

28.0%

91.1%

`aider --model claude-3-5-haiku-20241022`

diff

gpt-4o-2024-08-06

23.1%

94.2%

`aider --model gpt-4o-2024-08-06`

diff

gemini-2.0-flash-exp

22.2%

100.0%

`aider --model gemini/gemini-2.0-flash-exp`

whole

gpt-4o-2024-11-20

18.2%

95.1%

`aider --model gpt-4o-2024-11-20`

diff

DeepSeek Chat V2.5

17.8%

92.9%

`aider --model deepseek/deepseek-chat`

diff

Qwen2.5-Coder-32B-Instruct

16.4%

99.6%

`aider --model openai/Qwen2.5-Coder-32B-Instruct`

whole

yi-lightning

12.9%

92.9%

`aider --model openai/yi-lightning`

whole

Codestral 25.01

11.1%

100.0%

`aider --model mistral/codestral-latest`

whole

Qwen2.5-Coder-32B-Instruct

8.0%

71.6%

`aider --model openai/Qwen/Qwen2.5-Coder-32B-Instruct # via hyperbolic`

diff

gpt-4o-mini-2024-07-18

3.6%

100.0%

`aider --model gpt-4o-mini-2024-07-18`

whole

### [](#aider-polyglot-benchmark-results)Aider polyglot benchmark results

By Paul Gauthier, last updated January 20, 2025.

* * *

Table of contents
-----------------

*   [Code editing leaderboard](/docs/leaderboards/edit.html)
*   [Refactoring leaderboard](/docs/leaderboards/refactor.html)
*   [Scores by release date](/docs/leaderboards/by-release-date.html)
*   [Benchmark notes](/docs/leaderboards/notes.html)
*   [Contributing results](/docs/leaderboards/contrib.html)

---



## [https://aider.chat/docs/leaderboards/edit.html](https://aider.chat/docs/leaderboards/edit.html)

[](#code-editing-leaderboard)Code editing leaderboard
=====================================================

This old [aider code editing leaderboard](edit.html) has been replaced by the new, much more challenging [polyglot leaderboard](/docs/leaderboards/).

[Aider’s code editing benchmark](/docs/benchmarks.html#the-benchmark) asks the LLM to edit python source files to complete 133 small coding exercises from Exercism. This measures the LLM’s coding ability, and whether it can write new code that integrates into existing code. The model also has to successfully apply all its changes to the source file without human intervention.

Model

Percent completed correctly

Percent using correct edit format

Command

Edit format

o1

84.2%

99.2%

`aider --model openrouter/openai/o1`

diff

claude-3-5-sonnet-20241022

84.2%

99.2%

`aider --model anthropic/claude-3-5-sonnet-20241022`

diff

gemini-exp-1206 (whole)

80.5%

100.0%

`aider --model gemini/gemini-exp-1206`

whole

o1-preview

79.7%

93.2%

`aider --model o1-preview`

diff

claude-3.5-sonnet-20240620

77.4%

99.2%

`aider --model claude-3.5-sonnet-20240620`

diff

claude-3-5-haiku-20241022

75.2%

95.5%

`aider --model anthropic/claude-3-5-haiku-20241022`

diff

ollama/qwen2.5-coder:32b

72.9%

100.0%

`aider --model ollama/qwen2.5-coder:32b`

whole

DeepSeek Coder V2 0724

72.9%

97.7%

`aider --model deepseek/deepseek-coder`

diff

gpt-4o-2024-05-13

72.9%

96.2%

`aider`

diff

DeepSeek-V2.5-1210

72.2%

99.2%

`aider --model deepseek/deepseek-chat`

diff

openai/chatgpt-4o-latest

72.2%

97.0%

`aider --model openai/chatgpt-4o-latest`

diff

DeepSeek V2.5

72.2%

96.2%

`aider --deepseek`

diff

gpt-4o-2024-11-20

71.4%

99.2%

`aider --model openai/gpt-4o-2024-11-20`

diff

Qwen2.5-Coder-32B-Instruct

71.4%

94.7%

`aider --model openai/hf:Qwen/Qwen2.5-Coder-32B-Instruct --openai-api-base https://glhf.chat/api/openai/v1`

diff

gpt-4o-2024-08-06

71.4%

98.5%

`aider --model openai/gpt-4o-2024-08-06`

diff

o1-mini (whole)

70.7%

90.0%

`aider --model o1-mini`

whole

gemini-2.0-flash-exp

69.9%

97.0%

`aider --model gemini/gemini-2.0-flash-exp`

diff

DeepSeek Chat V2 0628

69.9%

97.7%

`aider --model deepseek/deepseek-chat`

diff

gemini-exp-1206 (diff)

69.2%

84.2%

`aider --model gemini/gemini-exp-1206`

diff

Qwen2.5-Coder-14B-Instruct

69.2%

100.0%

`aider --model openai/Qwen2.5-Coder-14B-Instruct`

whole

claude-3-opus-20240229

68.4%

100.0%

`aider --opus`

diff

gpt-4-0613

67.7%

100.0%

`aider -4`

diff

Dracarys2-72B-Instruct

66.9%

100.0%

`(via glhf.chat)`

whole

gemini-1.5-pro-exp-0827

66.9%

94.7%

`aider --model gemini/gemini-1.5-pro-exp-0827`

diff-fenced

llama-3.1-405b-instruct (whole)

66.2%

100.0%

`aider --model openrouter/meta-llama/llama-3.1-405b-instruct`

whole

gpt-4-0314

66.2%

93.2%

`aider --model gpt-4-0314`

diff

gpt-4-0125-preview

66.2%

97.7%

`aider --model gpt-4-0125-preview`

udiff

yi-lightning

65.4%

97.0%

`aider --model openai/yi-lightning`

whole

openrouter/qwen/qwen-2.5-coder-32b-instruct

65.4%

84.2%

`aider --model openrouter/qwen/qwen-2.5-coder-32b-instruct`

diff

Mistral Large (2411)

65.4%

96.2%

`aider --model mistral/mistral-large-latest`

diff

gemini-1.5-pro-002

65.4%

96.2%

`aider --model gemini/gemini-1.5-pro-002`

diff-fenced

qwen-2.5-72b-instruct (bf16)

65.4%

96.2%

`aider --model openrouter/qwen/qwen-2.5-72b-instruct`

diff

gpt-4-1106-preview

65.4%

92.5%

`aider --model gpt-4-1106-preview`

udiff

ollama/Qwen2.5.1-Coder-7B-Instruct-GGUF:Q8\_0-32k

63.9%

100.0%

`aider --model ollama/Qwen2.5.1-Coder-7B-Instruct-GGUF:Q8_0-32k`

whole

nousresearch/hermes-3-llama-3.1-405b

63.9%

100.0%

`aider --model openrouter/nousresearch/hermes-3-llama-3.1-405b`

whole

llama-3.1-405b-instruct (diff)

63.9%

92.5%

`aider --model openrouter/meta-llama/llama-3.1-405b-instruct`

diff

gpt-4-turbo-2024-04-09 (udiff)

63.9%

97.0%

`aider --gpt-4-turbo`

udiff

ollama/qwen2.5-coder:14b

61.7%

98.5%

`aider --model ollama/qwen2.5-coder:14b`

whole

o1-mini

61.1%

100.0%

`aider --model o1-mini`

diff

gemini-exp-1114

60.9%

85.7%

`aider --model gemini/gemini-exp-1114`

diff

Mistral Large 2 (2407)

60.2%

100.0%

`aider --model mistral/mistral-large-2407`

whole

llama-3.3-70b-instruct

59.4%

88.7%

`aider --model openrouter/meta-llama/llama-3.3-70b-instruct`

diff

ollama/qwen2.5:32b-instruct-q8\_0

58.6%

100.0%

`aider --model ollama/qwen2.5:32b-instruct-q8_0`

whole

Grok-2

58.6%

98.5%

`aider --model openrouter/x-ai/grok-2`

whole

llama-3.1-70b-instruct

58.6%

100.0%

`aider --model fireworks_ai/accounts/fireworks/models/llama-v3p1-70b-instruct`

whole

gemini-exp-1121

57.9%

83.5%

`aider --model gemini/gemini-exp-1121`

diff

Qwen2.5-Coder-7B-Instruct

57.9%

100.0%

`aider --model openai/Qwen2.5-Coder-7B-Instruct`

whole

gpt-3.5-turbo-0301

57.9%

100.0%

`aider --model gpt-3.5-turbo-0301`

whole

gpt-4-turbo-2024-04-09 (diff)

57.6%

100.0%

`aider --model gpt-4-turbo-2024-04-09`

diff

gemini-1.5-pro-001

57.1%

87.2%

`aider --model gemini/gemini-1.5-pro-latest`

diff-fenced

gpt-3.5-turbo-1106

56.1%

100.0%

`aider --model gpt-3.5-turbo-1106`

whole

gpt-4o-mini

55.6%

100.0%

`aider --model gpt-4o-mini`

whole

Qwen2 72B Instruct

55.6%

100.0%

`aider --model together_ai/qwen/Qwen2-72B-Instruct`

whole

Llama-3.1-Nemotron-70B-Instruct-HF

54.9%

99.2%

`(via glhf.chat)`

whole

Grok-2-mini

54.9%

100.0%

`aider --model openrouter/x-ai/grok-2-mini`

whole

claude-3-sonnet-20240229

54.9%

100.0%

`aider --sonnet`

whole

Nova Pro

54.1%

100.0%

`aider --model bedrock/us.amazon.nova-pro-v1:0`

whole

ollama/qwen2.5:32b

54.1%

100.0%

`aider --model ollama/qwen2.5:32b`

whole

Yi Coder 9B Chat

54.1%

100.0%

`aider --model openai/hf:01-ai/Yi-Coder-9B-Chat --openai-api-base https://glhf.chat/api/openai/v1`

whole

gemini-1.5-flash-exp-0827

52.6%

100.0%

`aider --model gemini/gemini-1.5-flash-exp-0827`

whole

qwen2.5-coder:7b-instruct-q8\_0

51.9%

100.0%

`aider --model ollama/qwen2.5-coder:7b-instruct-q8_0`

whole

gemini-1.5-flash-002 (0924)

51.1%

100.0%

`aider --model gemini/gemini-1.5-flash-002`

whole

codestral-2405

51.1%

100.0%

`aider --model mistral/codestral-2405`

whole

gpt-3.5-turbo-0613

50.4%

100.0%

`aider --model gpt-3.5-turbo-0613`

whole

gpt-3.5-turbo-0125

50.4%

100.0%

`aider -3`

whole

qwen2:72b-instruct-q8\_0

49.6%

100.0%

`aider --model ollama/qwen2:72b-instruct-q8_0`

whole

llama3-70b-8192

49.2%

73.5%

`aider --model groq/llama3-70b-8192`

diff

Codestral-22B-v0.1-Q4\_K\_M

48.1%

100.0%

`aider --model Codestral-22B-v0.1-Q4_K_M`

whole

codestral:22b-v0.1-q8\_0

48.1%

100.0%

`aider --model ollama/codestral:22b-v0.1-q8_0`

whole

claude-3-haiku-20240307

47.4%

100.0%

`aider --model claude-3-haiku-20240307`

whole

ollama/codestral

45.9%

98.5%

`aider --model ollama/codestral`

whole

yi-coder:9b-chat-q4\_0

45.1%

100.0%

`aider --model ollama/yi-coder:9b-chat-q4_0`

whole

gemini-1.5-flash-latest

44.4%

100.0%

`aider --model gemini/gemini-1.5-flash-latest`

whole

WizardLM-2 8x22B

44.4%

100.0%

`aider --model openrouter/microsoft/wizardlm-2-8x22b`

whole

ollama/yi-coder:9b-chat-fp16

43.6%

99.2%

`aider --model ollama/yi-coder:9b-chat-fp16`

whole

Reflection-70B

42.1%

100.0%

`(not currently supported)`

whole

Qwen2.5-Coder-3B-Instruct

39.1%

100.0%

`aider --model openai/Qwen2.5-Coder-3B-Instruct`

whole

ollama/mistral-small

38.3%

99.2%

`aider --model ollama/mistral-small`

whole

gemini-1.5-flash-8b-exp-0924

38.3%

100.0%

`aider --model gemini/gemini-1.5-flash-8b-exp-0924`

whole

Command R (08-24)

38.3%

100.0%

`aider --model command-r-08-2024`

whole

Command R+ (08-24)

38.3%

100.0%

`aider --model command-r-plus-08-2024`

whole

gemini-1.5-flash-8b-exp-0827

38.3%

100.0%

`aider --model gemini/gemini-1.5-flash-8b-exp-0827`

whole

llama-3.1-8b-instruct

37.6%

100.0%

`aider --model fireworks_ai/accounts/fireworks/models/llama-v3p1-8b-instruct`

whole

qwen1.5-110b-chat

37.6%

100.0%

`aider --model together_ai/qwen/qwen1.5-110b-chat`

whole

gemma2:27b-instruct-q8\_0

36.1%

100.0%

`aider --model ollama/gemma2:27b-instruct-q8_0`

whole

codeqwen:7b-chat-v1.5-q8\_0

34.6%

100.0%

`aider --model ollama/codeqwen:7b-chat-v1.5-q8_0`

whole

ollama/mistral-nemo:12b-instruct-2407-q4\_K\_M

33.1%

100.0%

`aider --model ollama/mistral-nemo:12b-instruct-2407-q4_K_M`

whole

ollama/codegeex4

32.3%

97.0%

`aider --model ollama/codegeex4`

whole

Qwen2.5-Coder-1.5B-Instruct

31.6%

100.0%

`aider --model openai/Qwen2.5-Coder-1.5B-Instruct`

whole

command-r-plus

31.6%

100.0%

`aider --model command-r-plus`

whole

ollama/hermes3:8b-llama3.1-fp16

30.1%

98.5%

`aider --model ollama/hermes3:8b-llama3.1-fp16`

whole

ollama/wojtek/opencodeinterpreter:6.7b

30.1%

91.0%

`aider --model ollama/wojtek/opencodeinterpreter:6.7b`

whole

o1-mini-2024-09-12

27.1%

95.6%

`aider --model o1-mini`

whole

ollama/tulu3

26.3%

100.0%

`aider --model ollama/tulu3`

whole

ollama/llama3.2:3b-instruct-fp16

26.3%

97.0%

`aider --model ollama/llama3.2:3b-instruct-fp16`

whole

ollama/hermes3

22.6%

98.5%

`aider --model ollama/hermes3`

whole

ollama/granite3-dense:8b

20.3%

78.9%

`aider --model ollama/granite3-dense:8b`

whole

Qwen2.5-Coder-0.5B-Instruct

14.3%

100.0%

`aider --model openai/Qwen2.5-Coder-0.5B-Instruct`

whole

[](#notes-on-benchmarking-results)Notes on benchmarking results
---------------------------------------------------------------

The key benchmarking results are:

*   **Percent completed correctly** - Measures what percentage of the coding tasks that the LLM completed successfully. To complete a task, the LLM must solve the programming assignment _and_ edit the code to implement that solution.
*   **Percent using correct edit format** - Measures the percent of coding tasks where the LLM complied with the edit format specified in the system prompt. If the LLM makes edit mistakes, aider will give it feedback and ask for a fixed copy of the edit. The best models can reliably conform to the edit format, without making errors.

[](#notes-on-the-edit-format)Notes on the edit format
-----------------------------------------------------

Aider uses different “edit formats” to collect code edits from different LLMs. The “whole” format is the easiest for an LLM to use, but it uses a lot of tokens and may limit how large a file can be edited. Models which can use one of the diff formats are much more efficient, using far fewer tokens. Models that use a diff-like format are able to edit larger files with less cost and without hitting token limits.

Aider is configured to use the best edit format for the popular OpenAI and Anthropic models and the [other models recommended on the LLM page](/docs/llms.html). For lesser known models aider will default to using the “whole” editing format since it is the easiest format for an LLM to use.

[](#contributing-benchmark-results)Contributing benchmark results
-----------------------------------------------------------------

Contributions of benchmark results are welcome! See the [benchmark README](https://github.com/Aider-AI/aider/blob/main/benchmark/README.md) for information on running aider’s code editing benchmarks. Submit results by opening a PR with edits to the [benchmark results data files](https://github.com/Aider-AI/aider/blob/main/aider/website/_data/).

By Paul Gauthier, last updated January 16, 2025.

---



## [https://aider.chat/docs/leaderboards/refactor.html](https://aider.chat/docs/leaderboards/refactor.html)

[](#refactoring-leaderboard)Refactoring leaderboard
---------------------------------------------------

[Aider’s refactoring benchmark](https://github.com/Aider-AI/refactor-benchmark) asks the LLM to refactor 89 large methods from large python classes. This is a more challenging benchmark, which tests the model’s ability to output long chunks of code without skipping sections or making mistakes. It was developed to provoke and measure [GPT-4 Turbo’s “lazy coding” habit](/2023/12/21/unified-diffs.html).

The refactoring benchmark requires a large context window to work with large source files. Therefore, results are available for fewer models.

Model

Percent completed correctly

Percent using correct edit format

Command

Edit format

claude-3-5-sonnet-20241022

92.1%

91.0%

`aider --sonnet`

diff

o1-preview

75.3%

57.3%

`aider --model o1-preview`

diff

claude-3-opus-20240229

72.3%

79.5%

`aider --opus`

diff

claude-3.5-sonnet-20240620

64.0%

76.4%

`aider --sonnet`

diff

gpt-4o

62.9%

53.9%

`aider`

diff

gpt-4-1106-preview

50.6%

39.3%

`aider --model gpt-4-1106-preview`

udiff

gpt-4o-2024-08-06

49.4%

89.9%

`aider --model openai/gpt-4o-2024-08-06`

diff

gemini/gemini-1.5-pro-latest

49.4%

7.9%

`aider --model gemini/gemini-1.5-pro-latest`

diff-fenced

o1-mini

44.9%

29.2%

`aider --model o1-mini`

diff

gpt-4-turbo-2024-04-09 (udiff)

34.1%

30.7%

`aider --gpt-4-turbo`

udiff

gpt-4-0125-preview

33.7%

47.2%

`aider --model gpt-4-0125-preview`

udiff

DeepSeek Coder V2 0724 (deprecated)

32.6%

59.6%

`aider --model deepseek/deepseek-coder`

diff

DeepSeek Chat V2.5

31.5%

67.4%

`aider --deepseek`

diff

gpt-4-turbo-2024-04-09 (diff)

21.4%

6.8%

`aider --model gpt-4-turbo-2024-04-09`

diff

By Paul Gauthier, last updated January 16, 2025.

---



## [https://aider.chat/docs/leaderboards/by-release-date.html](https://aider.chat/docs/leaderboards/by-release-date.html)

[](#llm-code-editing-skill-by-model-release-date)LLM code editing skill by model release date
---------------------------------------------------------------------------------------------

[](https://aider.chat/assets/models-over-time.svg)

---



## [https://aider.chat/docs/leaderboards/notes.html](https://aider.chat/docs/leaderboards/notes.html)

[](#benchmark-notes)Benchmark notes
===================================

[](#notes-on-benchmarking-results)Notes on benchmarking results
---------------------------------------------------------------

The key benchmarking results are:

*   **Percent completed correctly** - Measures what percentage of the coding tasks that the LLM completed successfully. To complete a task, the LLM must solve the programming assignment _and_ edit the code to implement that solution.
*   **Percent using correct edit format** - Measures the percent of coding tasks where the LLM complied with the edit format specified in the system prompt. If the LLM makes edit mistakes, aider will give it feedback and ask for a fixed copy of the edit. The best models can reliably conform to the edit format, without making errors.

[](#notes-on-the-edit-format)Notes on the edit format
-----------------------------------------------------

Aider uses different “edit formats” to collect code edits from different LLMs. The “whole” format is the easiest for an LLM to use, but it uses a lot of tokens and may limit how large a file can be edited. Models which can use one of the diff formats are much more efficient, using far fewer tokens. Models that use a diff-like format are able to edit larger files with less cost and without hitting token limits.

Aider is configured to use the best edit format for the popular OpenAI and Anthropic models and the [other models recommended on the LLM page](/docs/llms.html). For lesser known models aider will default to using the “whole” editing format since it is the easiest format for an LLM to use.

---



## [https://aider.chat/docs/leaderboards/contrib.html](https://aider.chat/docs/leaderboards/contrib.html)

[](#contributing-results)Contributing results
=============================================

Contributions of benchmark results are welcome! See the [benchmark README](https://github.com/Aider-AI/aider/blob/main/benchmark/README.md) for information on running aider’s code editing benchmarks. Submit results by opening a PR with edits to the [benchmark results data files](https://github.com/Aider-AI/aider/blob/main/aider/website/_data/).

---



## [https://aider.chat/blog/](https://aider.chat/blog/)

Aider blog
==========

[R1+Sonnet set SOTA on aider's polyglot benchmark](/2025/01/24/r1-sonnet.html)
------------------------------------------------------------------------------

R1+Sonnet has set a new SOTA on the aider polyglot benchmark. At 14X less cost compared to o1.[

](/2025/01/24/r1-sonnet.html)

JAN 24, 2025

[Using uv as an installer](/2025/01/15/uv.html)
-----------------------------------------------

Reliably packaging & distributing python CLI tools is hard. Aider uses uv in novel ways to make it easy to install the aider CLI, its dependencies and python 3.12. All in an isolated env.

JAN 15, 2025

[o1 tops aider's new polyglot leaderboard](/2024/12/21/polyglot.html)
---------------------------------------------------------------------

o1 scores the top result on aider's new multi-language, more challenging coding benchmark.[

](/2024/12/21/polyglot.html)

DEC 21, 2024

[QwQ is a code architect, not an editor](/2024/12/03/qwq.html)
--------------------------------------------------------------

QwQ is reasoning model like o1, and needs to be used as an architect with another model as editor.[

](/2024/12/03/qwq.html)

DEC 3, 2024

[Details matter with open source models](/2024/11/21/quantization.html)
-----------------------------------------------------------------------

Open source LLMs are becoming very powerful, but pay attention to how you (or your provider) are serving the model. It can affect code editing skill.[

](/2024/11/21/quantization.html)

NOV 21, 2024

[Separating code reasoning and editing](/2024/09/26/architect.html)
-------------------------------------------------------------------

An Architect model describes how to solve the coding problem, and an Editor model translates that into file edits. This Architect/Editor approach produces SOTA benchmark results.[

](/2024/09/26/architect.html)

SEP 26, 2024

[o1-preview is SOTA on the aider leaderboard](/2024/09/12/o1.html)
------------------------------------------------------------------

Preliminary benchmark results for the new OpenAI o1 models.

SEP 12, 2024

[Sonnet seems as good as ever](/2024/08/26/sonnet-seems-fine.html)
------------------------------------------------------------------

Sonnet's score on the aider code editing benchmark has been stable since it launched.[

](/2024/08/26/sonnet-seems-fine.html)

AUG 26, 2024

[LLMs are bad at returning code in JSON](/2024/08/14/code-in-json.html)
-----------------------------------------------------------------------

LLMs write worse code if you ask them to return the code wrapped in JSON via a tool function call.[

](/2024/08/14/code-in-json.html)

AUG 14, 2024

[Coding with Llama 3.1, new DeepSeek Coder & Mistral Large](/2024/07/25/new-models.html)
----------------------------------------------------------------------------------------

Summary of code editing skill for the new models, with Sonnet and GPT-3.5 for scale.[

](/2024/07/25/new-models.html)

JUL 25, 2024

[Sonnet is the opposite of lazy](/2024/07/01/sonnet-not-lazy.html)
------------------------------------------------------------------

Claude 3.5 Sonnet can easily write more good code than fits in one 4k token API response.[

](/2024/07/01/sonnet-not-lazy.html)

JUL 1, 2024

[Aider is SOTA for both SWE Bench and SWE Bench Lite](/2024/06/02/main-swe-bench.html)
--------------------------------------------------------------------------------------

Aider sets SOTA for the main SWE Bench, after recently setting SOTA for the Lite version.[

](/2024/06/02/main-swe-bench.html)

JUN 2, 2024

[Aider has written 7% of its own code (outdated, now 70%)](/2024/05/24/self-assembly.html)
------------------------------------------------------------------------------------------

This article is quite out dated. Aider is currently writing about 70% of the new code in each release.[

](/2024/05/24/self-assembly.html)

MAY 24, 2024

[How aider scored SOTA 26.3% on SWE Bench Lite](/2024/05/22/swe-bench-lite.html)
--------------------------------------------------------------------------------

Aider achieved this result mainly through its existing features that focus on static code analysis, reliable LLM code editing, and pragmatic UX for AI pair programming.[

](/2024/05/22/swe-bench-lite.html)

MAY 22, 2024

[Linting code for LLMs with tree-sitter](/2024/05/22/linting.html)
------------------------------------------------------------------

Aider now lints code after every LLM edit and automatically fixes errors, using tree-sitter and AST-aware code context.[

](/2024/05/22/linting.html)

MAY 22, 2024

[Drawing graphs with aider, GPT-4o and matplotlib](/2024/05/13/models-over-time.html)
-------------------------------------------------------------------------------------

Use GPT-4o to draw graphs with matplotlib, including adjusting styles and making visual changes. You get the graph, but you also get the code in your repo.[

](/2024/05/13/models-over-time.html)

MAY 13, 2024

[Aider in your browser](/2024/05/02/browser.html)
-------------------------------------------------

Aider has an experimental browser UI, allowing you to collaborate with LLMs on code in your local git repo.[

](/2024/05/02/browser.html)

MAY 2, 2024

[GPT-4 Turbo with Vision is a step backwards for coding](/2024/04/09/gpt-4-turbo.html)
--------------------------------------------------------------------------------------

OpenAI's GPT-4 Turbo with Vision model scores worse on aider's code editing benchmarks than all the previous GPT-4 models. In particular, it seems much more prone to "lazy coding" than the existing GPT-4 Turbo "preview" models.[

](/2024/04/09/gpt-4-turbo.html)

APR 9, 2024

[Claude 3 beats GPT-4 on Aider's code editing benchmark](/2024/03/08/claude-3.html)
-----------------------------------------------------------------------------------

Claude 3 Opus outperforms all of OpenAI's models on Aider's code editing benchmark, making it the best available model for pair programming with AI.[

](/2024/03/08/claude-3.html)

MAR 8, 2024

[The January GPT-4 Turbo is lazier than the last version](/2024/01/25/benchmarks-0125.html)
-------------------------------------------------------------------------------------------

The new \`gpt-4-0125-preview\` model is quantiatively lazier at coding than previous GPT-4 versions, according to a new "laziness" benchmark.[

](/2024/01/25/benchmarks-0125.html)

JAN 25, 2024

[Unified diffs make GPT-4 Turbo 3X less lazy](/2023/12/21/unified-diffs.html)
-----------------------------------------------------------------------------

GPT-4 Turbo has a problem with lazy coding, which can be signiciantly improved by asking for code changes formatted as unified diffs.[

](/2023/12/21/unified-diffs.html)

DEC 21, 2023

[Speed benchmarks of GPT-4 Turbo and gpt-3.5-turbo-1106](/2023/11/06/benchmarks-speed-1106.html)
------------------------------------------------------------------------------------------------

This report provides a detailed comparison of the speed of GPT-4 Turbo and gpt-3.5-turbo-1106 models based on the aider benchmarking suite.[

](/2023/11/06/benchmarks-speed-1106.html)

NOV 6, 2023

[Code editing benchmarks for OpenAI's "1106" models](/2023/11/06/benchmarks-1106.html)
--------------------------------------------------------------------------------------

A quantitative comparison of the code editing capabilities of the new GPT-3.5 and GPT-4 versions that were released in Nov 2023.[

](/2023/11/06/benchmarks-1106.html)

NOV 6, 2023

[Building a better repository map with tree sitter](/2023/10/22/repomap.html)
-----------------------------------------------------------------------------

Tree-sitter allows aider to build a repo map that better summarizes large code bases.[

](/2023/10/22/repomap.html)

OCT 22, 2023

[GPT code editing benchmarks](/2023/07/02/benchmarks.html)
----------------------------------------------------------

Benchmarking GPT-3.5 and GPT-4 code editing skill using a new code editing benchmark suite based on the Exercism python exercises.[

](/2023/07/02/benchmarks.html)

JUL 2, 2023

[Improving GPT-4's codebase understanding with ctags](/2023/05/25/ctags.html)
-----------------------------------------------------------------------------

Using ctags to build a "repository map" to increase GPT-4's ability to understand a large code base.[

](/2023/05/25/ctags.html)

MAY 25, 2023

---



## [https://aider.chat/#aider-is-ai-pair-programming-in-your-terminal](https://aider.chat/#aider-is-ai-pair-programming-in-your-terminal)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/#getting-started](https://aider.chat/#getting-started)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/#features](https://aider.chat/#features)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/#top-tier-performance](https://aider.chat/#top-tier-performance)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/2024/06/02/main-swe-bench.html](https://aider.chat/2024/06/02/main-swe-bench.html)

June 02, 2024

[](#aider-is-sota-for-both-swe-bench-and-swe-bench-lite)Aider is SOTA for both SWE Bench and SWE Bench Lite
===========================================================================================================

Aider scored 18.9% on the main [SWE Bench benchmark](https://www.swebench.com), achieving a state-of-the-art result. The current top leaderboard entry is 13.8% from Amazon Q Developer Agent. The best result reported elsewhere seems to be [13.9% from Devin](https://www.cognition.ai/post/swe-bench-technical-report).

This result on the main SWE Bench builds on [aider’s recent SOTA result on the easier SWE Bench Lite](https://aider.chat/2024/05/22/swe-bench-lite.html).

[](https://aider.chat/assets/swe_bench.svg)

**All of aider’s results reported here are pass@1 results, obtained without using the SWE Bench `hints_text`.** Aider was benchmarked on the same [570 randomly selected SWE Bench problems](https://github.com/CognitionAI/devin-swebench-results/tree/main/output_diffs) that were used in the [Devin evaluation](https://www.cognition.ai/post/swe-bench-technical-report). See the [references](#references) for more details on the data presented in this chart.

[](#interactive-not-agentic)Interactive, not agentic
----------------------------------------------------

Aider achieved this result mainly through its existing features that focus on static code analysis, reliable LLM code editing, and pragmatic UX for automatically fixing linting and testing errors. Aider intentionally has quite limited and narrow “agentic behavior” to avoid long delays, high token costs and the need for users to repeatedly code review incorrect solutions. It’s also worth noting that aider currently does not use RAG, vector search, tools or give the LLM access to search the web or unilaterally execute code.

Aider is first and foremost an interactive tool for engineers to get real work done in real code bases using a chat interface. Aider provides a pair programming UX where users can ask for a change and see code edits performed in real-time. Aider can also offer additional help like fixing lint or test errors, but the user is always in full interactive control. This allows them to quickly steer misunderstandings back on course and avoid wasting time and token costs.

[](#benchmark-methodology)Benchmark methodology
-----------------------------------------------

Benchmarking was conducted as follows:

*   Aider with GPT-4o was launched in each problem’s git repository with the problem statement submitted as the opening chat message from “the user”.
*   After that aider ran as normal, except all of aider’s suggestions were always accepted without user approval.
*   A [simple harness](https://github.com/Aider-AI/aider-swe-bench#the-aider-agent) was used to retry the SWE Bench problem if aider produced code that wasn’t _plausibly correct_. Plausibly correct means that aider reported that it had successfully edited the repo without causing syntax errors or breaking any _pre-existing_ tests.
*   If the solution from aider with GPT-4o wasn’t plausible, the harness launched aider to try again from scratch using Claude 3 Opus.
*   If no plausible solution was found after those two tries, the harness picked the “most plausible” solution with the fewest edit/lint/test problems.

It’s important to be clear that _aider and the benchmark harness only had access to the pre-existing tests in each problem’s repo_. The held out “acceptance tests” were _only_ used after benchmarking to compute statistics on which problems aider correctly resolved.

This is the same approach that was used for [aider’s recent SOTA result on SWE Bench Lite](https://aider.chat/2024/05/22/swe-bench-lite.html). For the Lite benchmark, aider alternated between GPT-4o and Opus for up to six total attempts. To manage the cost of running the main SWE Bench benchmark, aider was limited to two total attempts: one with GPT-4o and one with Opus.

For a detailed discussion of the benchmark methodology, see the [article about aider’s SWE Bench Lite results](https://aider.chat/2024/05/22/swe-bench-lite.html). Also, the [aider SWE Bench repository on GitHub](https://github.com/Aider-AI/aider-swe-bench) contains the harness and statistics code used for the benchmarks.

The benchmarking process was similar to how a developer might use aider to resolve a GitHub issue:

*   They could launch aider in their repo with the command below, which tells aider they want to accept every suggestion and to use pytest to run tests.
    *   `aider --yes --test-cmd pytest`
*   They could start the chat by pasting in the URL or text of a GitHub issue. Aider will pull in the URL’s content and then try and resolve the issue.
*   If aider doesn’t produce code that lints and tests clean, the user might decide to [use git to revert the changes](https://aider.chat/docs/git.html), and try again with `aider --opus`.

[](#aider-with-gpt-4o-alone-was-sota)Aider with GPT-4o alone was SOTA
---------------------------------------------------------------------

Using aider with GPT-4o to make a single attempt at resolving each problem achieved a score of 17.0%. This was itself a state-of-the-art result, before being surpassed by the main result being reported here that used aider with both GPT-4o & Opus.

[](#aider-with-gpt-4o--opus)Aider with GPT-4o & Opus
----------------------------------------------------

The benchmark harness started by using aider with GPT-4o to try and resolve each problem. For problems where this didn’t produce a plausible solution, the harness tried again using aider with Opus. So at most, two attempts were made for each problem.

The table below breaks down the proposed solutions that were found from each attempt at the 570 problems. A proposed solution is either:

*   A plausible solution where aider reported no outstanding errors from editing, linting and testing.
*   Or, the “most plausible” solution generated by either attempt, with the [fewest outstanding editing, linting or testing errors](https://aider.chat/2024/05/22/swe-bench-lite.html#finding-a-plausible-solution).

The table also provides details on the 108 solutions that were ultimately verified as correctly resolving their issue.

Attempt

Agent

Number of  
proposed  
solutions

Percent of  
proposed  
solutions

Number of  
correctly  
resolved  
solutions

Percent of  
correctly  
resolved  
solutions

Score on  
SWE Bench  
Lite

1

Aider with GPT-4o

419

73.5%

87

80.6%

15.3%

2

Aider with Opus

151

26.5%

21

19.4%

3.7%

**Total**

 

**570**

**100%**

**108**

**100%**

**18.9%**

[](#non-plausible-but-correct-solutions)Non-plausible but correct solutions?
----------------------------------------------------------------------------

A solution doesn’t actually have to be plausible in order to correctly resolve the issue. Recall that plausible is simply defined as aider reporting that it successfully completed all file edits, repaired and resolved any linting errors and resolved any test failures. But there are many reasons why aider might fail to do those things and yet still produce a solution that will pass acceptance testing:

*   There may have been pre-existing failing tests in the repo, before aider even started working on the SWE Bench problem. Aider may not have resolved such issues, and yet they may not be relevant to the acceptance testing. The SWE Bench acceptance testing just confirms that tests pass or fail in the same pattern as the “gold patch” developed by a human to resolve the problem. Some tests may fail during acceptance testing, and that’s ok as long as they failed for the gold patch too.
*   There may have been pre-existing linting problems in the repo. If lingering linting issues affected code paths that are not well tested, they may not impact acceptance testing.
*   Aider may have reported file editing errors because it thought the LLM specified edits that it wasn’t able to successfully apply. This can only happen when the LLM specified edits in a way that doesn’t comply with the editing instructions in the system prompt. Given that the LLM isn’t complying with the system prompt, it may have become confused and asked for redundant or otherwise irrelevant edits. Such outstanding edit errors might not be fatal for acceptance testing.
*   Etc.

Keeping all this in mind, we can understand why GPT-4o accounts for 15.3% of the benchmark score in the table above, but benchmarking with just one attempt of aider with GPT-4o scored 17.0%. When an Opus attempt is allowed after GPT-4o, it may propose some _incorrect_ solutions which are “more plausible” than some of GPT-4o’s non-plausible solutions. These more plausible, incorrect solutions can eclipse some of the earlier non-plausible correct solutions that GPT-4o generated. This is why GPT-4o’s score in the table showing the combined GPT-4o & Opus results (15.3%) is lower than the result from just one try using aider with GPT-4o (17.0%).

For these reasons, adding additional attempts is not guaranteed to monotonically increase the number of resolved problems. New solutions may resolve some new problems but they may also eclipse and discard some of the previous non-plausible correct solutions.

Luckily, the net effect of additional attempts usually increases or at least maintains the number of resolved solutions. This was the case for all the attempts made in both this main SWE Bench result and the earlier Lite result.

[](#computing-the-benchmark-score)Computing the benchmark score
---------------------------------------------------------------

The benchmark harness produced one proposed solution for each of the 570 SWE Bench problems.

A separate evaluation script was used to test each of these solutions with the full test suite, including the held out acceptance tests. For this final acceptance testing, any edits that aider made to tests were discarded. This ensured that the correct, unmodified test suite was used for acceptance testing. The evaluation script compared each proposed solution’s test results with results from testing the “gold” patch that was developed by a human to correctly resolve the issue. If they matched, the proposed solution correctly resolved the issue.

These acceptance tests were only ever run outside of aider and the benchmark harness, and only to compute statistics about the correctly resolved instances. They were never run, used, or even visible during aider’s attempts to resolve the problems.

Aider correctly resolved 108 out of 570 SWE Bench instances that were benchmarked, or 18.9%.

[](#acknowledgments)Acknowledgments
-----------------------------------

Much thanks to the team behind the [SWE Bench](https://www.swebench.com) family of AI coding benchmarks. Also thanks to Albert Örwall who has [dockerized the SWE Bench evaluation scripts](https://github.com/aorwall/SWE-bench-docker) making it faster, easier, and more reliable to run the acceptance tests.

[](#references)References
-------------------------

All of aider’s results reported here are pass@1 results, obtained without using the SWE Bench `hints_text`.

The “aider agent” internally makes multiple “attempts” at solving the problem, but it picks and returns one single candidate solution. Only that one candidate solution is evaluated with the acceptance tests and contributes to the benchmark score. Thus it is a pass@1 result.

This is contrast to a pass@N result for N>1, where N attempts are made and all N solutions are evaluated by the acceptance tests. If _any_ of the N solution pass, that counts as a pass@N success.

Below are the references for the other pass@1 unhinted SWE-Bench results displayed in the graph at the beginning of this article.

*   [13.9% Devin, benchmarked on 570 instances.](https://www.cognition.ai/post/swe-bench-technical-report)
*   [13.8% Amazon Q Developer Agent, benchmarked on 2,294 instances.](https://www.swebench.com)
*   [12.5% SWE- Agent + GPT-4, benchmarked on 2,294 instances.](https://www.swebench.com)
*   [10.6% AutoCode Rover, benchmarked on 2,294 instances.](https://arxiv.org/pdf/2404.05427v2)
*   [10.5% SWE- Agent + Opus, benchmarked on 2,294 instances.](https://www.swebench.com)

The graph contains average pass@1 results for AutoCodeRover. The [AutoCodeRover GitHub page](https://github.com/nus-apr/auto-code-rover) features their pass@3 results without being clearly labeled. Table 2 of their [paper](https://arxiv.org/pdf/2404.05427v2) reports an `ACR-avg` result of 10.59% which is an average pass@1 result.

---



## [https://aider.chat/#more-info](https://aider.chat/#more-info)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---



## [https://aider.chat/#kind-words-from-users](https://aider.chat/#kind-words-from-users)

[](#aider-is-ai-pair-programming-in-your-terminal)Aider is AI pair programming in your terminal
===============================================================================================

Aider lets you pair program with LLMs, to edit code in your local git repository. Start a new project or work with an existing code base. Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

 Your browser does not support the video tag.

[](https://discord.gg/Tv2uQnR88V)[](https://aider.chat/docs/install.html)

[](#getting-started)Getting started
-----------------------------------

If you already have python 3.8-3.13 installed, you can get started quickly like this:

    python -m pip install aider-install
    aider-install
    
    # Change directory into your code base
    cd /to/your/project
    
    # Work with Claude 3.5 Sonnet on your code
    aider --model sonnet --anthropic-api-key your-key-goes-here
    
    # Work with GPT-4o on your code
    aider --model gpt-4o --openai-api-key your-key-goes-here
    

See the [installation instructions](https://aider.chat/docs/install.html) and [usage documentation](https://aider.chat/docs/usage.html) for more details.

[](#features)Features
---------------------

*   Run aider with the files you want to edit: `aider <file1> <file2> ...`
*   Ask for changes:
    *   Add new features or test cases.
    *   Describe a bug.
    *   Paste in an error message or or GitHub issue URL.
    *   Refactor code.
    *   Update docs.
*   Aider will edit your files to complete your request.
*   Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
*   [Use aider inside your favorite editor or IDE](https://aider.chat/docs/usage/watch.html).
*   Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more…
*   Aider can edit multiple files at once for complex requests.
*   Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
*   Edit files in your editor or IDE while chatting with aider, and it will always use the latest version. Pair program with AI.
*   [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
*   [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
*   [Code with your voice](https://aider.chat/docs/usage/voice.html).
*   Aider works best with Claude 3.5 Sonnet, DeepSeek V3, o1 & GPT-4o and can [connect to almost any LLM](https://aider.chat/docs/llms.html).

[](#top-tier-performance)Top tier performance
---------------------------------------------

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html). SWE Bench is a challenging software engineering benchmark where aider solved _real_ GitHub issues from popular open source projects like django, scikitlearn, matplotlib, etc.

[](#more-info)More info
-----------------------

*   [Documentation](https://aider.chat/)
*   [Installation](https://aider.chat/docs/install.html)
*   [Usage](https://aider.chat/docs/usage.html)
*   [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
*   [Connecting to LLMs](https://aider.chat/docs/llms.html)
*   [Configuration](https://aider.chat/docs/config.html)
*   [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
*   [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
*   [GitHub](https://github.com/Aider-AI/aider)
*   [Discord](https://discord.gg/Tv2uQnR88V)
*   [Blog](https://aider.chat/blog/)

[](#kind-words-from-users)Kind words from users
-----------------------------------------------

*   _The best free open source AI coding assistant._ – [IndyDevDan](https://youtu.be/YALpX8oOn78)
*   _The best AI coding assistant so far._ – [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
*   _Aider … has easily quadrupled my coding productivity._ – [SOLAR\_FIELDS](https://news.ycombinator.com/item?id=36212100)
*   _It’s a cool workflow… Aider’s ergonomics are perfect for me._ – [qup](https://news.ycombinator.com/item?id=38185326)
*   _It’s really like having your senior developer live right in your Git repo - truly amazing!_ – [rappster](https://github.com/Aider-AI/aider/issues/124)
*   _What an amazing tool. It’s incredible._ – [valyagolev](https://github.com/Aider-AI/aider/issues/6#issue-1722897858)
*   _Aider is such an astounding thing!_ – [cgrothaus](https://github.com/Aider-AI/aider/issues/82#issuecomment-1631876700)
*   _It was WAY faster than I would be getting off the ground and making the first few working versions._ – [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
*   _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ – [derwiki](https://news.ycombinator.com/item?id=38205643)
*   _It’s just amazing. It is freeing me to do things I felt were out my comfort zone before._ – [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
*   _This project is stellar._ – [funkytaco](https://github.com/Aider-AI/aider/issues/112#issuecomment-1637429008)
*   _Amazing project, definitely the best AI coding assistant I’ve used._ – [joshuavial](https://github.com/Aider-AI/aider/issues/84)
*   _I absolutely love using Aider … It makes software development feel so much lighter as an experience._ – [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
*   _I have been recovering from multiple shoulder surgeries … and have used aider extensively. It has allowed me to continue productivity._ – [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
*   _I am an aider addict. I’m getting so much more work done, but in less time._ – [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
*   _After wasting $100 on tokens trying to find something better, I’m back to Aider. It blows everything else out of the water hands down, there’s no competition whatsoever._ – [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
*   _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ – [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
*   _Hands down, this is the best AI coding assistant tool so far._ – [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
*   _\[Aider\] changed my daily coding workflows. It’s mind-blowing how a single Python application can change your life._ – [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
*   _Best agent for actual dev work in existing codebases._ – [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)

---

