# 开发指南 | Koishi



## [https://koishi.chat/zh-CN/guide/#VPContent](https://koishi.chat/zh-CN/guide/#VPContent)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/develop/setup.html](https://koishi.chat/zh-CN/guide/develop/setup.html)

环境搭建 [​](#环境搭建)
===============

本节将介绍推荐的开发环境搭建流程。如果某些软件已经安装完成，可以跳过对应的步骤。

安装 Node.js [​](#安装-node-js)
---------------------------

Koishi 需要 [Node.js](https://nodejs.org/) (最低 v18，推荐使用 LTS) 运行环境，你需要自己安装它。

### 下载安装包 [​](#下载安装包)

首先我们前往 [Node.js](https://nodejs.org/) 的官方网站：

在这里可以看到两个巨大的按钮，分别对应着 **LTS (长期维护版)** 和 **Current (最新版本)**。我们建议你选择更加稳定的 LTS 版本，点击按钮即可下载安装包。

随后，运行下载好的安装包，根据提示完成整个安装流程即可。

### 安装包管理器 [​](#安装包管理器)

Node.js 自带名为 [npm](https://www.npmjs.com/) 的包管理器，你可以直接使用它。我们同时也推荐功能更强大的 [yarn](https://classic.yarnpkg.com/) 作为包管理器。它的安装非常简单，只需打开命令行输入下面的命令：

sh

    # 安装 yarn
    npm i -g yarn
    
    # 查看版本
    yarn -v

TIP

部分 Windows 用户可能会发现以下错误 ([参考链接](https://learn.microsoft.com/zh-cn/powershell/module/microsoft.powershell.core/about/about_execution_policies))：

text

    yarn：无法加载文件 yarn.ps1，因为在此系统上禁止运行脚本。

此时请以管理员身份重新运行终端，并输入下面的命令：

sh

    Set-ExecutionPolicy RemoteSigned

之后就可以正常使用 yarn 了。

### 配置镜像源 [​](#配置镜像源)

如果你是国内用户，从 npm 或 yarn 上下载依赖可能非常慢。因此，我们推荐你配置一下镜像源，以提升安装速度。

npmyarn

npm

    npm config set registry https://registry.npmmirror.com

### 注册 npm [​](#注册-npm)

如果你打算发布插件，你还需要注册一个 npm 账号。这一步非常简单，只需前往这里的 [注册页面](https://www.npmjs.com/signup)。填写你的用户名、邮箱和密码，勾选同意协议，点击注册即可。

注册完成后，你就可以在命令行中使用 `npm login` 来登录你的账号：

sh

    npm login --registry=https://registry.npmjs.org

版本控制 [​](#版本控制)
---------------

我们强烈推荐使用版本控制系统 (VCS) 来管理你的代码。这一方面允许你在任何时候回退到之前的版本，另一方面也能让你与其他开发者协作。

### 安装 Git [​](#安装-git)

Git 是最普遍使用的版本控制工具。前往 [官网](https://git-scm.com/downloads)，点击右上角的青色按钮下载安装包。

国内的 Windows 用户也可以选择从 [镜像](https://registry.npmmirror.com/binary.html?path=git-for-windows/) 下载。如果不知道下载哪个版本，可以在上面的官网中看到 (比如图中就是 2.39.1)。

获取到安装包后，双击运行。安装过程无需手动配置，一直点击下一步即可完成安装。

安装完成后，可以在命令行中输入 `git --version` 来查看版本号，以确认安装成功：

sh

    git --version           # git version 2.39.1

最后你还需要设置你的姓名和邮箱。它们将会默认作为你创建的插件的作者，也会出现在你的提交记录中：

sh

    git config --global user.name "Your Name"
    git config --global user.email "you@example.com"

### 注册 GitHub [​](#注册-github)

通常来说我还会建议你注册一个 GitHub 账号。[GitHub](https://github.com) 是一个代码托管平台，我们可以在上面创建仓库来存放我们的代码。由于篇幅有限，请在互联网搜索相关的教程，自行完成注册。如果发现无法注册，也不用担心，你仍然可以在本地进行开发。

安装 Koishi [​](#安装-koishi)
-------------------------

打开命令行，并进入你想要创建 Koishi 项目的目录。

TIP

这个目录不宜过长，且路径中请避免出现中文或者空格。我们推荐的目录如下：

*   Windows：`C:\dev` 或者 `D:\dev` (也不要直接在盘根创建项目，最好是建一层目录)
*   其他操作系统：`~/dev`

输入下面的命令以创建 Koishi 项目：

npmyarn

npm

    npm init koishi@latest

跟随提示即可完成全套初始化流程。

如果你顺利完成了上述操作，你的应用此时应该已经是启动状态，并弹出了控制台界面。接下来的几节中我们将学习更多的命令行用法，因此我们可以先关闭 Koishi。在命令行中按下 `Ctrl+C` 组合键即可停止 Koishi 的运行。

---



## [https://koishi.chat/zh-CN/guide/develop/config.html](https://koishi.chat/zh-CN/guide/develop/config.html)

配置文件 [​](#配置文件)
===============

WARNING

配置文件的结构未来可能会发生变化，请留意后续更新。

每个 Koishi 应用都有一个配置文件，它管理了应用及其插件的全部配置。在绝大多数情况下，我们都可以使用控制台修改这些配置，而无需手动编辑配置文件。但作为开发指南的一部分，我们还是需要了解一下配置文件的结构，并介绍一些你可能会用到的进阶用法。

默认情况下配置文件的格式为 [YAML](https://en.wikipedia.org/wiki/YAML)，它是一种易于阅读和编辑的文本格式，你可以用任何文本编辑器打开。

应用目录 [​](#应用目录)
---------------

配置文件所在的目录叫**应用目录**。根据你的安装方式，应用目录的位置可能不同：

*   模板项目：你创建的项目目录，例如 `D:/dev/koishi-app`
*   启动器 (zip)：解压目录下 `data/instances/default`
*   启动器 (msi)：`C:/Users/你的用户名/AppData/Roaming/Koishi/Desktop/data/instances/default`
*   启动器 (pkg)：`~/Library/Application Support/Koishi/Desktop/data/instances/default`

配置文件是应用目录下名为 `koishi.yml` 的文件。当你遇到问题时，开发者可能会要求你提供配置文件的内容。此时去上面的地方找就好了。

理解配置文件 [​](#理解配置文件)
-------------------

尝试打开配置文件，你会发现它的内容大致如下：

yaml

    # 全局设置
    host: localhost
    port: 5140
    
    # 插件列表
    plugins:
      # group 表示这是一个插件组
      group:console:
        # 波浪线前缀表示一个不启用的插件
        ~auth:
        console:
        logger:
        insight:
        market:
          # 以缩进的方式显示插件的配置项
          registry:
            endpoint: https://registry.npmmirror.com
    
      # 这里是一些零散的插件
      github:
      dialogue:

具体而言，配置文件中包含的内容如下。

### 全局设置 [​](#全局设置)

全局设置对应于配置文件中 `plugins:` 一行以上的部分。这里会包含一些最基础的配置项，例如网络设置、指令前缀、默认权限等。修改这里的配置项，会影响整个 Koishi 应用的行为而非某个插件。你可以在 [这个页面](./../../api/core/app.html) 了解全部的全局设置。

### 插件配置 [​](#插件配置)

`plugins` 是一个 YAML 对象，它的每一个键对应于插件的名称，而值则对应于插件的配置。当没有进行配置时，值可以省略 (或者写成 `{}`)。当存在配置时，值需要在插件的基础上缩进并写在接下来的几行中。例如：

yaml

    plugins:
      dialogue:
        # 这里是 koishi-plugin-dialogue 的配置
        context:
          enable: true

### 插件名称 [​](#插件名称)

插件名称通常对应于插件发布时的包名。例如：

*   `market` 对应于官方插件 `@koishijs/plugin-market`
*   `dialogue` 对应于社区插件 `koishi-plugin-dialogue`

除了插件的包名外，插件名称还可以拥有一个可选的前缀 (`~`) 和后缀 (`:xxx`)。插件名称前的波浪线 (`~`) 表示该插件不会被启用。插件名称后的冒号后是插件的别名，当某个插件需要存在多组配置时这会非常有用。

### 插件组 [​](#插件组)

你可以将插件组理解为一个名为 `group` 的特殊插件。它的语法与 `plugins` 一致，都是一个包含了插件名称和插件配置的 YAML 对象。使用插件组不仅能更好地帮助你整理插件，还能批量控制其中插件的行为。插件组也支持嵌套，例如：

yaml

    plugins:
      group:official:
        # 一层嵌套插件组下的 help 插件
        help:
        group:console:
          # 两层嵌套插件组下的 market 插件
          market:

### 元信息 [​](#元信息)

一些以 `$` 开头的属性会记录插件和插件组的元信息。例如：

yaml

    plugins:
      group:console:
        # 在控制台中折叠该插件组
        $collapsed: true
        status:
          # 仅对于 telegram 平台启用该插件
          $filter:
            $eq:
              - $: platform
              - telegram

修改配置文件 [​](#修改配置文件)
-------------------

TIP

如果你不了解 YAML 的语法，请不要随意修改配置文件，否则将可能导致 Koishi 应用无法运行。你可以在 [这篇教程](https://www.runoob.com/w3cnote/yaml-intro.html) 中学习 YAML 的语法。

当你启动 Koishi 应用时，Koishi 会读取上述配置文件并加载所需的插件。反过来，如果你想调整 Koishi 及其插件的行为，你就需要修改这个配置文件。

如果你使用的是模板项目，你需要手动修改它并重新启动 Koishi 应用；如果你使用的是启动器，则你可以直接在「插件配置」中进行调整，Koishi 会自动将这些改动写入配置文件。事实上你会发现，配置文件的结构与「插件配置」页面基本是一致的。

绝大多数的功能都可以通过「插件配置」页面来完成，但目前尚有一些功能没有做好相应的交互界面，这时你仍然需要手动修改配置文件。具体的步骤与模板项目类似：

1.  关闭当前 Koishi 应用
2.  在 [应用目录](#应用目录) 下找到配置文件并进行编辑
3.  保存配置文件后再次启动 Koishi 应用

使用环境变量 [​](#使用环境变量)
-------------------

你可以通过插值语法在配置文件中使用环境变量。例如：

koishi.yml

    plugins:
      adapter-discord:
        token: ${{ env.DISCORD_TOKEN }}

当项目启动时，会将环境变量中的值替换进去。

除了系统提供的环境变量外，Koishi 还原生支持 [dotenv](https://github.com/motdotla/dotenv)。你可以在当前目录创建一个 `.env.local` 文件，并在里面填写你的环境变量。这个文件已经被包含在 `.gitignore` 中，你可以在其中填写隐私信息 (例如账号密码) 而不用担心被上传到远端。例如在上面的例子中你就可以这样写：

.env

    DISCORD_TOKEN = xxx

环境变量的另一个作用是条件判断。例如官方提供的模板项目里：

koishi.yml

    plugins:
      desktop:
        $if: env.KOISHI_AGENT?.includes('Desktop')

这样一来，只有当你使用桌面客户端启动 Koishi 时，这个插件才会被启用。

---



## [https://koishi.chat/zh-CN/guide/develop/script.html](https://koishi.chat/zh-CN/guide/develop/script.html)

启动脚本 [​](#启动脚本)
===============

Koishi 提供了一套命令行工具，用于读取配置文件快速启动应用。

TIP

本节中介绍的命令行都需要在 [应用目录](./config.html#应用目录) 下运行。

基本用法 [​](#基本用法)
---------------

我们通常使用 **启动脚本** 来启动 Koishi 应用。打开应用目录下的 `package.json` 文件：

package.json

    {
      "scripts": {
        "dev": "cross-env NODE_ENV=development koishi start -r esbuild-register -r yml-register",
        "start": "koishi start"
      }
    }

在应用目录运行下面的命令行以启动 Koishi 应用：

npmyarn

npm

    npm run start

在本节的后续部分，我们会介绍上述启动脚本的更多参数。无论你做何改动，你都可以使用上面的命令行来快速启动。这也是启动脚本的意义所在。

### 启动参数 [​](#启动参数)

启动脚本支持 Node.js 的 [命令行参数](https://nodejs.org/api/cli.html)。例如，上面的 `-r` 对应于 `--require`，它将允许你加载 `.ts` 和 `.yml` 后缀的文件。

除了 Node.js 的命令行参数，Koishi 还提供了一些额外的参数。我们将在下面逐一介绍。

### 自动重启 [​](#自动重启)

Koishi 的命令行工具支持自动重启。当运行 Koishi 的进程崩溃时，如果 Koishi 已经启动成功，则监视进程将自动重新启动一个新的进程。

开发模式 [​](#开发模式)
---------------

除了 `start` 以外，模板项目还准备了名为 `dev` 的开发模式启动脚本。在应用目录运行下面的命令行可以以开发模式启动应用：

npmyarn

npm

    npm run dev

如你所见，`dev` 相当于在 `start` 指令的基础上添加了额外的参数和环境变量。这些参数为我们启用了额外的特性，而环境变量则能影响插件的部分行为。

### TypeScript 支持 [​](#typescript-支持)

Koishi 模板项目原生地支持 TypeScript 开发。上述 `-r esbuild-register` 参数允许我们在运行时直接使用工作区插件的 TypeScript 源代码。

你也可以自行扩展更多的后缀名支持。例如，如果你更喜欢 CoffeeScript，你可以这样修改你的开发脚本为：

package.json

    {
      "scripts": {
        "dev": "koishi start -r coffeescript/register"
      },
      "devDependencies": {
        "coffeescript": "^2.7.0"
      }
    }

这样你就可以使用 CoffeeScript 编写你的插件源代码 (当然你还得自行处理构建逻辑)，甚至连配置文件都可以使用 `koishi.coffee` 书写了。

DANGER

我们并不推荐使用高级语言来编写配置文件，因为动态的配置无法支持环境变量、配置热重载和插件市场等特性。大部分情况下我们建议仅将 `-r` 用于开发目的。

### 模块热替换 [​](#hmr)

如果你开发着一个巨大的 Koishi 项目，可能光是加载一遍全部插件就需要好几秒了。在这种时候，像前端框架一样支持模块热替换就成了一个很棒的主意。幸运的是，Koishi 也做到了这一点！内置插件 @koishijs/plugin-hmr 实现了插件级别的热替换。每当你修改你的本地文件时，Koishi 就会尝试重载你的插件，并在命令行中提醒你。

这里的行为也可以在配置文件中进行定制：

koishi.yml

    plugins:
      group:develop:
        $if: env.NODE_ENV === 'development'
        hmr:
          root: '.'
          # 要忽略的文件列表，支持 glob patterns
          ignore:
            - some-file

TIP

由于部分 Linux 系统有着 8192 个文件的监听数量限制，你可能会发现运行 `yarn dev` 后出现了如下的报错：

text

    NOSPC: System limit for number of file watchers reached

此时你可以使用下面的命令来增加监听数量限制：

sh

    echo fs.inotify.max_user_watches=524288 |
    sudo tee -a /etc/sysctl.conf &&
    sudo sysctl -p

另一种方案是只监听部分子路径，例如将 `root` 改为 `external/foo` (其中 `foo` 是你正在开发的插件目录，参见下一节的工作区指南)，这将忽略其他目录下的变化，并依然对你的插件进行热重载。当你同时开发多个插件时，你也可以将 `root` 改成一个数组来使用。

---



## [https://koishi.chat/zh-CN/guide/develop/workspace.html](https://koishi.chat/zh-CN/guide/develop/workspace.html)

工作区开发 [​](#工作区开发)
=================

Koishi 的核心是插件系统，绝大部分 Koishi 功能都可以通过插件实现。本章节将介绍如何使用模板项目开发和构建自己的 Koishi 插件。

TIP

本节中介绍的命令行都需要在 [应用目录](./config.html#应用目录) 下运行。

创建新插件 [​](#setup)
-----------------

在应用目录运行下面的命令以创建一个新的插件工作区：

npmyarn

npm

    npm run setup [name] -- [-c] [-m] [-G]

*   **name:** 插件的包名，缺省时将进行提问
*   **\-c, --console:** 创建一个带控制台扩展的插件
*   **\-m, --monorepo:** 创建 monorepo 的插件
*   **\-G, --no-git:** 跳过 git 初始化

我们假设你创建了一个叫 `example` 的插件。那么，你将看到下面的目录结构：

diff

    root
    ├── external
    │   └── example
    │       ├── src
    │       │   └── index.ts
    │       └── package.json
    ├── koishi.yml
    └── package.json

打开 `index.ts` 文件，并修改其中的代码：

ts

    import { Context } from 'koishi'
    
    export const name = 'example'
    
    export function apply(ctx: Context) {
      // 如果收到“天王盖地虎”，就回应“宝塔镇河妖”
      ctx.on('message', (session) => {
        if (session.content === '天王盖地虎') {
          session.send('宝塔镇河妖')
        }
      })
    }

以 [开发模式](./script.html#开发模式) 重新运行你的项目，点击右上角的「添加插件」按钮，选择你刚才创建的插件名称，你会立即在网页控制台的配置界面中看到 `example` 插件。只需点击启用，你就可以实现与机器人的对话了：

A

Alice

天王盖地虎

Koishi

宝塔镇河妖

### 创建私域插件 [​](#scoped)

如果你发现想要创建的插件名称已经被占用了，除了重新想名字或在后面加上数字之外，你还可以改为创建私域插件。私域插件使用你自己的 [npm 用户名](./setup.html#注册-npm) 作为包名前缀，因此不用担心与其他人的插件冲突。

假设你的 npm 用户名是 `alice`，那么你可以使用下面的命令创建一个私域插件工作区：

npmyarn

npm

    npm run setup @alice/example

此外，你还需要额外修改 `tsconfig.json` 文件。打开这个文件，你将看到下面的内容：

json

    {
      "extends": "./tsconfig.base",
      "compilerOptions": {
        "baseUrl": ".",
        "paths": {
          // "@scope/koishi-plugin-*": ["external/*/src"],
          "@alice/koishi-plugin-*": ["external/*/src"],
        },
      },
    }

找到高亮的一行代码，将其复制一份，并将 `@scope` 替换为你的 npm 用户名，然后将复制的这一行代码前面的注释符号去掉。

构建源代码 [​](#build)
-----------------

上面的插件暂时还只能在开发模式下运行。如果想要在生产模式下使用或发布到插件市场，你需要构建你的源代码。在应用目录运行下面的命令：

npmyarn

npm

    npm run build [...name]

*   **name:** 要构建的插件列表，缺省时表示全部插件

还是以上面的插件 `example` 为例：

*   后端代码将输出到 `external/example/lib` 目录
*   前端代码将输出到 `external/example/dist` 目录 (如果存在)

添加依赖 [​](#add)
--------------

插件创建时，`package.json` 中已经包含了一些必要的依赖。如果你需要添加其他依赖，可以使用下面的命令：

npmyarn

npm

    npm install [...deps] -w koishi-plugin-[name]

*   **name:** 你的插件名称
*   **deps:** 要添加的依赖列表

如果要添加的是 `devDependencies` 或者 `peerDependencies`，你也需要在命令后面加上 `-D` 或 `-P` 参数。关于服务类插件的依赖声明，请参考 [后续章节](./../plugin/service.html#关于-peerdependencies)。

更新依赖版本 [​](#dep)
----------------

尽管 npm 和 yarn 等包管理器都提供了依赖更新功能，但它们对工作区开发的支持都不是很好。因此，我们也提供了一个简单的命令用于批量更新依赖版本。

npmyarn

npm

    npm run dep

这将按照每个 `package.json` 中声明的依赖版本进行更新。举个例子，如果某个依赖的版本是 `^1.1.4`，而这个依赖之后发布了新版本 `1.2.3` 和 `2.3.3`，那么运行该指令后，依赖的版本将会被更新为 `^1.2.3`。

二次开发 [​](#clone)
----------------

TIP

阅读本节前请确保你已经完成 [版本控制](./setup.html#版本控制) 中的全部准备工作。

TIP

如果你想要贡献原始仓库，在开始执行下面的操作之前，请确保你对要开发的仓库有写入权限。如果没有，你应当先创建属于自己的 fork，然后将下面的仓库名称替换为你的 fork 仓库名称。举个例子，假如你的 GitHub 用户名是 `alice`，那么下面你使用的仓库名称应当是 `alice/koishi-plugin-forward` 而不是 `koishijs/koishi-plugin-forward`。

二次开发是指调试或修改其他仓库中的插件。这种情况下，你需要先将对应的仓库克隆到本地，然后在本地进行调试和修改。

### 开发插件 [​](#开发插件)

其他人创建的工作区插件可以直接克隆到你的 `external` 目录下。例如，你可以使用下面的命令将 `koishi-plugin-forward` 插件克隆到本地：

npmyarn

npm

    npm run clone koishijs/koishi-plugin-forward

### 开发 Koishi [​](#开发-koishi)

工作区不仅可以用于插件的二次开发，还可以用于开发 Koishi 本身。只需使用下面的命令将 Koishi 仓库克隆到本地，并完成构建：

npmyarn

npm

    npm run clone koishijs/koishi
    npm run build -w @root/koishi

通常来说，非插件仓库在克隆下来之后还需经过路径配置才可以正常使用。不过不同担心，模板项目支持已经内置了 Koishi 生态中的几个核心仓库 ([koishi](https://github.com/koishijs/koishi), [satori](https://github.com/satorijs/satori), [minato](https://github.com/shigma/minato)) 的路径配置。

完成上述操作后，现在你的 `yarn dev` 已经能直接使用 Koishi 的 TypeScript 源码了！

---



## [https://koishi.chat/zh-CN/guide/develop/publish.html](https://koishi.chat/zh-CN/guide/develop/publish.html)

发布插件 [​](#发布插件)
===============

为了让别人更方便地使用你编写的插件，你需要将其作为一个 npm 包进行发布。只需满足一定的规范，你的插件就能显示在 [插件市场](./../../market/) 中，其他人可以通过控制台来安装它。

TIP

本节中介绍的命令行都需要在 [应用目录](./config.html#应用目录) 下运行。

准备工作 [​](#准备工作)
---------------

首先让我们关注插件目录中的 `package.json` 文件。这个文件非常重要，它包含了要发布插件的一切元信息。

diff

    root
    ├── plugins
    │   └── example
    │       ├── src
    │       │   └── index.ts
    │       └── package.json        # 你应该修改这里
    ├── koishi.yml
    └── package.json                # 而不是这里

TIP

请注意 `package.json` 文件不是唯一的，它在应用目录和每个插件目录都会存在。请确保你修改了正确的文件。

打开上述文件，你会看到它大概长这样：

package.json

    {
      "name": "koishi-plugin-example",
      "version": "1.0.0",
      // ……
    }

其中最重要的属性有两个：`name` 是要发布的包名，`version` 是当前版本号。可以看到，这里的包名相比实际在插件市场中看到的插件名多了一个 `koishi-plugin-` 的前缀，这使得我们很容易区分 Koishi 插件与其他 npm 包，同时也方便了用户安装和配置插件。

TIP

请注意：包名和版本号都是唯一的：包名不能与其他已经发布的包相同，而同一个包的同一个版本号也只能发布一次。如果出现了包名冲突或版本号冲突，则会在之后的发布流程中出现错误提示。你可以自行根据错误提示更改包名或更新插件版本。

补充更多信息 [​](#补充更多信息)
-------------------

除了包名和版本号以外，`package.json` 还包括了插件的依赖、描述、贡献者、许可证、关键词等更多信息。你并不需要一上来就把所有信息都填写完整，因为你可以随后再进行修改。但请别忘了，这些内容也是插件的一部分，修改完成后别忘了 [更新版本](#更新插件版本) 并 [再次发布](#发布插件)。

### 准入条件 [​](#准入条件)

TIP

使用模板项目创建的插件一定是符合要求的，因此你可以跳过这一节。

要想显示在插件市场中，插件的 `package.json` 需要满足以下基本要求：

*   [`name`](https://docs.npmjs.com/cli/v8/configuring-npm/package-json#name) 必须符合以下格式之一：
    *   `koishi-plugin-*`
    *   `@bar/koishi-plugin-*`
    *   `@koishijs/plugin-*` (官方插件)
    *   其中 `*` 是由数字、小写字母和连字符 `-` 组成的字符串
*   [`name`](https://docs.npmjs.com/cli/v10/configuring-npm/package-json#name) 不能与已发布的插件重复或相似
*   [`version`](https://docs.npmjs.com/cli/v10/configuring-npm/package-json#version) 应当符合 [语义化版本](https://semver.org/lang/zh-CN/) (通常从 `1.0.0` 开始)
*   [`peerDependencies`](https://docs.npmjs.com/cli/v10/configuring-npm/package-json#peerdependencies) 必须包含 `koishi`
*   不能声明 [`private`](https://docs.npmjs.com/cli/v10/configuring-npm/package-json#private) 为 `true` (否则你的插件无法发布)
*   最新版本不能被 [弃用](https://docs.npmjs.com/deprecating-and-undeprecating-packages-or-package-versions)

一个符合上述标准的示例：

package.json

    {
      "name": "koishi-plugin-example",
      "version": "1.0.0",
      "peerDependencies": {
        "koishi": "^4.3.2"
      }
    }

### 添加相关信息 [​](#添加相关信息)

除去上面的基本要求外，`package.json` 中还有一些字段能帮助显示插件的相关信息。

package.json

    {
      "name": "koishi-plugin-example",
      "version": "1.0.0",
      "contributors": [                         // 贡献者
        "Alice <alice@gmail.com>",
        "Bob <bob@gmail.com>"
      ],
      "license": "MIT",                         // 许可证
      "homepage": "https://example.com",        // 主页
      "repository": {                           // 源码仓库
        "type": "git",
        "url": "git+https://github.com/alice/koishi-plugin-example.git"
      },
      "keywords": ["example"],                  // 关键词
      "peerDependencies": {
        "koishi": "^4.3.2"
      }
    }

*   **contributors:** 插件维护者，应该是一个数组，其中的元素通常使用 `名字 <邮箱>` 的格式
*   **license:** 插件许可证，你可以在 [这里](https://choosealicense.com/licenses/) 了解各种许可证的详细信息
*   **homepage:** 插件主页，可以是一个网址 (比如你的 GitHub 项目地址)
*   **repository:** 插件源码仓库，应该是一个对象，其中 `type` 字段指定仓库类型，`url` 字段指定仓库地址
*   **keywords:** 插件关键词，应该是一个字符串数组，会用于插件市场中的搜索功能

TIP

`package.json` 中还有一些字段没有在这里提及，如果你对此感兴趣，可以前往 [npmjs.com](https://docs.npmjs.com/files/package.json/) 查看文档。

### `koishi` 字段 [​](#koishi-字段)

除此以外，我们还提供了一个额外的 `koishi` 字段，用于指定与 Koishi 相关的信息。

package.json

    {
      "name": "koishi-plugin-dialogue",
      "version": "1.0.0",
      "peerDependencies": {
        "koishi": "^4.3.2"
      },
      "koishi": {
        "description": {                        // 不同语言的插件描述
          "en": "English Description",
          "zh": "中文描述"
        },
        "service": {
          "required": ["database"],             // 必需的服务
          "optional": ["assets"],               // 可选的服务
          "implements": ["dialogue"],           // 实现的服务
        },
      }
    }

*   **description:** 插件描述，应该是一个对象，其中的键代表语言名，值是对应语言下的描述
*   **service:** 插件的服务相关信息，详情请参见 [服务与依赖](./../plugin/service.html#package-json)
*   **preview:** 配置为 `true` 可以让插件显示为「开发中」状态
*   **hidden:** 配置为 `true` 可以让插件市场中不显示该插件 (通常情况下你不需要这么做)

TIP

此外，还有一些字段与 [Koishi Online](./../../cookbook/practice/online.html) 的部署流程相关 (如 `browser`, `exports` 等)。由于不影响主线开发，你可以稍后再进行了解。

发布插件 [​](#发布插件-1)
-----------------

编辑完上面的清单文件并 [构建源代码](./workspace.html#build) 后，你就可以公开发布你的插件了。

npmyarn

npm

    npm run pub [...name]

*   **name:** 要发布的插件列表，缺省时表示全部 (此处 `name` 不包含 `koishi-plugin-` 前缀，而是你的工作区目录名)

这将发布所有版本号发生变动的插件。

TIP

从插件成功发布到进插件市场需要一定的时间 (通常在 15 分钟内)，请耐心等待。

TIP

如果你配置了国内镜像，你可能会遇到以下的错误提示：

text

    No token found and can't prompt for login when running with --non-interactive.

此时你需要在发布时使用官方镜像，具体操作如下：

npmyarn

npm

    npm run pub [...name] -- --registry https://registry.npmjs.org

对于 Yarn v2 及以上版本，你还可以分别针对发布和安装设置不同的镜像：

yarn

yarn

    # 安装时使用国内镜像
    yarn config set npmRegistryServer https://registry.npmmirror.com
    # 发布时使用官方镜像
    yarn config set npmPublishRegistry https://registry.yarnpkg.com

更新插件版本 [​](#更新插件版本)
-------------------

初始创建的插件版本号为 `1.0.0`。当你修改过插件后，你需要更新版本号才能重新发布。在应用目录运行下面的命令以更新版本号：

npmyarn

npm

    npm run bump [...name] -- [-1|-2|-3|-p|-v <ver>] [-r]

*   **name:** 要更新的插件列表，不能为空
*   **\-1, --major:** 跳到下一个大版本，例如 `3.1.4` -> `4.0.0`
*   **\-2, --minor:** 跳到下一个中版本，例如 `3.1.4` -> `3.2.0`
*   **\-3, --patch:** 跳到下一个小版本，例如 `3.1.4` -> `3.1.5`
*   **\-p, --prerelease:** 跳到下一个预览版本，具体行为如下
    *   如果当前版本是 `alpha.x`，则跳到 `beta.0`
    *   如果当前版本是 `beta.x`，则跳到 `rc.0`
    *   如果当前版本是 `rc.x`，则移除 prerelease 部分
    *   其他情况下，跳到下一个大版本的 `alpha.0`
*   **\-v, --version:** 设置具体的版本号
*   **\-r, --recursive:** 递归更新依赖版本
*   缺省情况：按照当前版本的最后一位递增

当进行此操作时，其他相关插件的依赖版本也会同步更新，确保所有工作区内依赖的插件版本一致。进一步，如果你希望更新了依赖版本的插件也同时更新自身的版本，那么可以附加 `-r, --recursive` 选项。

弃用插件 [​](#deprecate)
--------------------

如果你不再维护某个插件，或者你希望更换一个名字重新发布，那么你可以弃用该插件。在任意目录运行下面的命令以弃用插件：

sh

    npm deprecate <full-name> <message>
    # 例如
    npm deprecate koishi-plugin-example "this plugin is deprecated"

请注意这里要写出的是完整的包名，而不是插件的目录名。

你也可以弃用某个特定版本或版本区间 (默认情况下将弃用所有版本)：

sh

    npm deprecate <full-name>[@<version>] <message>

弃用插件的最新版本后，该插件将不再显示在插件市场中。未来你仍然可以发布新版本，这将使你的插件重新进入插件市场。

---



## [https://koishi.chat/zh-CN/guide/basic/command.html](https://koishi.chat/zh-CN/guide/basic/command.html)

指令开发 [​](#指令开发)
===============

TIP

在学习本节之前，建议先完整阅读 [入门 > 指令系统](./../../manual/usage/command.html)。

正如我们在入门篇中介绍的那样，一个 Koishi 机器人的绝大部分功能都是通过指令提供给用户的。Koishi 的指令系统能够高效地处理大量消息的并发调用，同时还提供了快捷方式、调用前缀、权限管理、速率限制、本地化等大量功能。因此，只需掌握指令开发并编写少量代码就可以轻松应对各类用户需求。

编写下面的代码，你就实现了一个简单的 echo 指令：

ts

    ctx.command('echo <message>')
      .action((_, message) => message)

A

Alice

echo Hello!

Koishi

Hello!

让我们回头看看这段代码是如何工作的：

*   `.command()` 方法定义了名为 echo 的指令，其有一个必选参数为 `message`
*   `.action()` 方法定义了指令触发时的回调函数，第一个参数是一个 `Argv` 对象，第二个参数是输入的 `message`

这种链式的结构能够让我们非常方便地定义和扩展指令。稍后我们将看到这两个函数的更多用法，以及更多指令相关的函数。

定义参数 [​](#定义参数)
---------------

正如你在上面所见的那样，使用 `ctx.command(decl)` 方法可以定义一个指令，其中 `decl` 是一个字符串，包含了 **指令名** 和 **参数列表**。

*   指令名可以包含数字、字母、短横线甚至中文，但不应该包含空白字符、小数点 `.` 或斜杠 `/`；小数点和斜杠的用途参见 [注册子指令](#注册子指令) 章节
*   一个指令可以含有任意个参数，其中 **必选参数** 用尖括号包裹，**可选参数** 用方括号包裹；这些参数将作为 `action` 回调函数除 `Argv` 以外的的后续参数传入

例如，下面的程序定义了一个拥有三个参数的指令，第一个为必选参数，后面两个为可选参数，它们将分别作为 `action` 回调函数的第 2~4 个参数：

ts

    ctx.command('test <arg1> [arg2] [arg3]')
      .action((_, arg1, arg2, arg3) => { /* do something */ })

TIP

除去表达的意义不同，以及参数个数不足时使用必选参数可能产生错误信息外，这两种参数在程序上是没有区别的。与此同时，默认情况下 `action` 回调函数从第二个参数起也总是字符串。如果传入的参数不足，则对应的参数不会被传入，因此你需要自己处理可能的 `undefined`。

### 变长参数 [​](#变长参数)

有时我们需要传入未知数量的参数，这时我们可以使用 **变长参数**，它可以通过在括号中前置 `...` 来实现。在下面的例子中，无论传入了多少个参数，都会被放入 `rest` 数组进行处理：

ts

    ctx.command('test <arg1> [...rest]')
      .action((_, arg1, ...rest) => { /* do something */ })

### 文本参数 [​](#文本参数)

通常来说传入的信息被解析成指令调用后，会被空格分割成若干个参数。但如果你想输入的就是含有空格的内容，可以通过在括号中后置 `:text` 来声明一个 **文本参数**。 在下面的例子中，即使 test 后面的内容中含有空格，也会被整体传入 `message` 中：

ts

    ctx.command('test <message:text>')
      .action((_, message) => { /* do something */ })

TIP

文本参数的解析优先级很高，即使是之后的内容中含有选项也会被一并认为是该参数的一部分。因此，当使用文本参数时，应确保选项写在该参数之前，或 [使用引号](./../../manual/recipe/execution.html#使用引号) 将要输入的文本包裹起来。

### 参数类型 [​](#argument-type)

除去 `text` 以外，Koishi 还支持许多其他的类型。它们的用法与 `text` 无异：

ts

    function showValue(value) {
      return `${typeof value} ${JSON.stringify(value)}`
    }
    
    ctx.command('test [arg:number]')
      .option('foo', '<val:string>')
      .action(({ options }, arg) => `${showValue(arg)} ${showValue(options.foo)}`)

A

Alice

test 100 --foo 200

Koishi

number 100 string "200"

A

Alice

test xyz

Koishi

参数 arg 输入无效，请提供一个数字。

目前 Koishi 支持的内置类型如下：

*   string: `string` 字符串
*   number: `number` 数值
*   bigint: `bigint` [大整数](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/BigInt)
*   text: `string` 贪婪匹配的字符串
*   user: `string` 用户，格式为 `{platform}:{id}` (调用时可以使用 `at` 元素或者 `@{platform}:{id}` 的格式)
*   channel: `string` 频道，格式为 `{platform}:{id}` (调用时可以使用 `sharp` 元素或者 `#{platform}:{id}` 的格式)
*   integer: `number` 整数
*   posint: `number` 正整数
*   natural: `number` 正整数
*   date: `Date` 日期
*   image: `Dict` 图片

定义选项 [​](#定义选项)
---------------

使用 `cmd.option(name, decl)` 方法可以给指令定义参数。这个方法也是支持链式调用的，就像这样：

ts

    ctx.command('test')
      .option('alpha', '-a')          // 定义一个选项
      .option('beta', '-b [beta]')    // 定义一个带参数的可选选项
      .option('gamma', '-c <gamma>')  // 定义一个带参数的必选选项
      .action(({ options }) => JSON.stringify(options))

A

Alice

test -adb text --gamma=1 --foo-bar baz --no-xyz

Koishi

{ "alpha": true, "d": true, "beta": "text", "gamma": 1, "fooBar": "baz", "xyz": false }

从上面的例子中我们不难看出 Koishi 指令系统的许多方便的特性：

*   使用注册的多个别名中的任何一个都会被赋值到 `name` 中
*   选项和参数之间同时支持用空格或等号隔开的语法
*   单个短横线后跟多个字母时，会把之后的参数赋给最后一个字母（如果需要参数的话）
*   多字母中如果有短横线，会被自动进行驼峰式处理
*   类型自动转换：无参数默认为 `true`，如果是数字会转化为数字，其余情况为字符串
*   支持识别未注册选项，同时会根据传入的命令行推测是否需要参数
*   如果一个未注册选项以 `no-` 开头，则会自动去除这个前缀并处理为 `false`

在调用 `cmd.option()` 时，你还可以传入第三个参数，它应该是一个对象，用于配置选项的具体特性。它们将在下面逐一介绍。

### 选项的默认值 [​](#选项的默认值)

使用 `fallback` 配置选项的默认值。配置了默认值的选项，如果没有被使用，则会按照注册的默认值进行赋值。

ts

    ctx.command('test')
      .option('alpha', '-a', { fallback: 100 })
      .option('beta', '-b', { fallback: 100 })
      .action(({ options }) => JSON.stringify(options))

A

Alice

test -b 80

Koishi

{ "alpha": 100, "beta": 80 }

### 选项的重载 [​](#选项的重载)

将同一个选项注册多次，并结合使用 `value` 配置选项的重载值。如果使用了带有重载值的选项，将按照注册的重载值进行赋值。

ts

    ctx.command('test')
      .option('writer', '-w <id>')
      .option('writer', '--anonymous', { value: 0 })
      .action(({ options }) => JSON.stringify(options))

A

Alice

test --anonymous

Koishi

{ "writer": 0 }

### 选项类型 [​](#option-type)

选项也可以像参数一样设置类型：

ts

    ctx.command('text')
      .option('alpha', '-a <value:number>')

除了这种写法外，你还可以传入一个 `type` 属性，作为选项的临时类型声明。它可以是像上面的例子一样的回调函数，也可以是一个 `RegExp` 对象，表示传入的选项应当匹配的正则表达式：

ts

    ctx.command('test')
      .option('beta', '-b <value>', { type: /^ba+r$/ })
      .action(({ options }) => options.beta)

A

Alice

test -f bar

Koishi

bar

A

Alice

test -f baaaz

Koishi

选项 beta 输入无效，请检查语法。

指令别名 [​](#指令别名)
---------------

WARNING

由于指令名可以在用户侧配置，因此**不建议**开发者设置过多别名或以常用词作为别名。如果用户加载的多个插件都注册了同一个指令别名，那么后一个加载的插件将直接加载失败。

你可以为一条指令添加别名：

ts

    ctx.command('echo <message>').alias('say')

这样一来，无论是 `echo` 还是 `say` 都能触发这条指令了。

你还可以为别名添加参数或选项：

ts

    ctx.command('market <area> <item>').alias('市场', { args: ['China'] })

此时调用 `市场` 时将等价于调用 `market China`。如果你传入了更多的参数，那么它们将被添加到 `China` 之后。

编写帮助 [​](#编写帮助)
---------------

TIP

此功能需要安装 [@koishijs/plugin-help](./../../plugins/common/help.html) 插件。

之前已经介绍了 `ctx.command()` 和 `cmd.option()` 这两个方法，它们都能传入一个 `desc` 参数。你可以在这个参数的结尾补上对于指令或参数的说明文字，就像这样：

ts

    ctx.command('echo <message:text> 输出收到的信息')
      .option('timeout', '-t <seconds> 设定延迟发送的时间')

A

Alice

echo -h

Koishi

echo <message>

输出收到的信息

可用的选项有：

\-t, --timeout <seconds> 设定延迟发送的时间

### 添加使用说明 [​](#添加使用说明)

当然，我们还可以加入具体的用法和使用示例，进一步丰富这则使用说明：

ts

    ctx.command('echo <message:text>', '输出收到的信息')
      .option('timeout', '-t <seconds> 设定延迟发送的时间')
      .usage('注意：参数请写在最前面，不然会被当成 message 的一部分！')
      .example('echo -t 300 Hello World  五分钟后发送 Hello World')

这时再调用 `echo -h`，你便会发现使用说明中已经添加了你刚刚的补充文本：

A

Alice

echo -h

Koishi

echo <message>

输出收到的信息

注意：参数请写在最前面，不然会被当成 message 的一部分！

可用的选项有：

\-t, --timeout <seconds> 设定延迟发送的时间

使用示例：

echo -t 300 Hello World 五分钟后发送 Hello World

### 隐藏指令和选项 [​](#隐藏指令和选项)

读到这里，细心的你可能会产生一丝好奇：如果 `echo -h` 能够被解析成查看帮助的话，这个 `-h` 为什么不出现在这个帮助中呢？答案很简单，因为这个内置选项被 Koishi 隐藏起来了。如果你希望隐藏一条指令或一个选项，只需要注册时将配置项 `hidden` 设置为 `true` 即可：

ts

    // 手动导入类型
    import {} from '@koishijs/plugin-help'
    
    ctx.command('bar 一条看不见的指令', { hidden: true })
      .option('foo', '<text> 一个看不见的选项', { hidden: true })
      .action(({ options }) => 'secret: ' + options.foo)

A

Alice

help

Koishi

当前可用的指令有：

help 显示帮助信息

输入“帮助+指令名”查看特定指令的语法和使用示例。

A

Alice

help bar

Koishi

指令：bar

一条看不见的指令

A

Alice

bar --foo 123

Koishi

secret: 123

如果要查看隐藏的指令和选项，可以使用 `help -H`：

A

Alice

help -H

Koishi

当前可用的指令有：

help 显示帮助信息

bar 一条看不见的指令

输入“帮助+指令名”查看特定指令的语法和使用示例。

A

Alice

help bar -H

Koishi

指令：bar

一条看不见的指令

可用的选项有：

\--foo <text> 一个看不见的选项

注册子指令 [​](#注册子指令)
-----------------

在本节的最后，我们介绍一下[子指令](./../../manual/usage/command.html#子指令)的注册方法：

ts

    // 层级式子指令
    ctx.command('foo/bar')
    
    // 派生式子指令
    ctx.command('foo.bar')

是的，除了这里用到了斜杠 `/` 和小数点 `.` 来分别表示层级式和派生式子指令外，其他用法都是完全一致的。

对于已经存在的指令，你也可以使用 `cmd.subcommand()` 方法来注册子指令：

ts

    // 层级式子指令
    ctx.command('foo').subcommand('bar')
    
    // 派生式子指令
    ctx.command('foo').subcommand('.bar')

---



## [https://koishi.chat/zh-CN/guide/basic/events.html](https://koishi.chat/zh-CN/guide/basic/events.html)

事件系统 [​](#事件系统)
===============

在上一节中我们了解了指令开发，现在让我们回到更加基础的事件系统。事件系统在 Koishi 中扮演着底层的角色，它不仅包含由聊天平台触发的会话事件，还包含了监听运行状态的生命周期事件和提供扩展性的自定义事件。

基本用法 [​](#基本用法)
---------------

让我们先从一个基本示例开始：

ts

    ctx.on('message', (session) => {
      if (session.content === '天王盖地虎') {
        session.send('宝塔镇河妖')
      }
    })

上述代码片段实现了一个简单的功能：当任何用户发送「天王盖地虎」时，机器人将发送「宝塔镇河妖」。如你所见，`ctx.on()` 方法监听了一个事件。传入的第一个参数 `message` 是事件的名称，而第二个参数则是事件的回调函数。每一次 `message` 事件被触发 (即收到消息) 时都会调用该函数。

回调函数接受一个参数 `session`，称为**会话对象**。在这个例子中，我们通过它访问事件相关的数据 (使用 `session.content` 获取消息的内容)，并调用其上的 API 作为对此事件的响应 (使用 `session.send()` 在当前频道内发送消息)。

事件与会话构成了最基础的交互模型。这种模型不仅能够处理消息，还能够处理其他类型的事件。我们再给出一个例子：

ts

    // 当有好友请求时，接受请求并发送欢迎消息
    ctx.on('friend-request', async (session) => {
      // session.bot 是当前会话绑定的机器人实例
      await session.bot.handleFriendRequest(session.messageId, true)
      await session.bot.sendPrivateMessage(session.userId, '很高兴认识你！')
    })

像这样由聊天平台推送的事件，我们称之为 **会话事件**。除此以外，Koishi 还有着其他类型的事件，例如由 Koishi 自身生成的 **生命周期事件**，又或者是由插件提供的 **自定义事件** 等等。这些事件的监听方式与会话事件基本一致，只不过它们的回调函数接受的参数不同。例如下面的代码实现了当 Bot 上线时自动给自己发送一条消息的功能：

ts

    // bot-status-updated 不是会话事件
    // 所以回调函数接受的参数不是 session 而是 bot
    ctx.on('bot-status-updated', (bot) => {
      if (bot.status === Status.ONLINE) {
        // 这里的 userId 换成你的账号
        bot.sendPrivateMessage(userId, '我上线了~')
      }
    })

在后续的章节中，我们也将介绍更多的事件和会话的使用方法。

监听事件 [​](#监听事件)
---------------

在上面的例子中，我们已经了解到事件系统的基本用法：使用 `ctx.on()` 注册监听器。它的写法与 Node.js 自带的 [EventEmitter](https://nodejs.org/api/events.html#events_class_eventemitter) 类似：第一个参数表示要监听的事件名称，第二个参数表示事件的回调函数。同时，我们也提供了类似的函数 `ctx.once()`，用于注册一个只触发一次的监听器；以及 `ctx.off()`，用于取消一个已注册的监听器。

这套事件系统与 EventEmitter 的一个不同点在于，无论是 `ctx.on()` 还是 `ctx.once()` 都会返回一个 dispose 函数，调用这个函数即可取消注册监听器。因此你其实不必使用 `ctx.once()` 和 `ctx.off()`。下面给一个只触发一次的监听器的例子：

ts

    declare module 'koishi' {
      interface Events {
        foo(...args: any[]): void
      }
    }
    // ---cut---
    // 回调函数只会被触发一次
    const dispose = ctx.on('foo', (...args) => {
      dispose()
      // do something
    })

### 事件的命名 [​](#事件的命名)

无论是会话事件，生命周期事件还是插件自定义的事件，Koishi 的事件名都遵循着一些既定的规范。遵守规范能够让开发者获得一致的体验，提高开发和调试的效率。它们包括：

*   总是使用 param-case 作为事件名
*   通过命名空间进行管理，使用 `/` 作为分隔符
*   配对使用 xxx 和 before-xxx 命名具有时序关系的事件

举个例子，koishi-plugin-dialogue 扩展了多达 20 个自定义事件。为了防止命名冲突，所有的事件都以 `dialogue/` 开头，并且在特定操作前触发的事件都包含了 `before-` 前缀，例如：

*   dialogue/before-search: 获取搜索结果前触发
*   dialogue/search: 获取完搜索结果后触发

### 前置事件 [​](#前置事件)

前面介绍了，Koishi 有不少监听器满足 before-xxx 的形式。对于这类监听器的注册，我们也提供了一个语法糖，那就是 `ctx.before('xxx', callback)`。这种写法也支持命名空间的情况：

ts

    // @errors: 2304
    ctx.before('dialogue/search', callback)
    // 相当于
    ctx.on('dialogue/before-search', callback, true)

默认情况下，事件的多个回调函数的执行顺序取决于它们添加的顺序。先注册的回调函数会先被执行。如果你希望提高某个回调函数的优先级，可以给 `ctx.on()` 传入第三个参数 `prepend`，设置为 true 即表示添加到事件执行队列的开头而非结尾，相当于 [`emitter.prependListener()`](https://nodejs.org/api/events.html#emitterprependlistenereventname-listener)。

对于 `ctx.before()`，情况则正好相反。默认的行为的先注册的回调函数后执行，同时 `ctx.before()` 的第三个参数 `append` 则表示添加到事件执行队列的末尾而非开头。

触发事件 [​](#触发事件)
---------------

如果你开发的插件希望允许其他插件扩展，那么触发事件就是最简单的方式。

触发事件的基本用法也都与 EventEmitter 类似，第一个参数是事件名称，之后的参数对应回调函数的参数。下面是一个例子：

ts

    declare module 'koishi' {
      interface Events {
        'custom-event'(...args: any[]): void
      }
    }
    
    // ---cut---
    // @errors: 2304
    ctx.emit('custom-event', arg1, arg2, ...rest)
    // 对应于
    ctx.on('custom-event', (arg1, arg2, ...rest) => {})

### 触发方式 [​](#触发方式)

Koishi 的事件系统与 EventEmitter 的另一个区别在于，触发一个事件可以有着多种形式，目前支持 4 个不同的方法，足以适应绝大多数需求。

*   emit: 同时触发所有 event 事件的回调函数
*   parallel: 上述方法对应的异步版本
*   bail: 依次触发所有 event 事件的回调函数；当返回一个 `false`, `null`, `undefined` 以外的值时将这个值作为结果返回
*   serial: 上述方法对应的异步版本

此外，你还将在下一节学习 [中间件](./middleware.html)，它提供了一种更加强大的消息事件处理流程。

### 过滤触发上下文 [​](#过滤触发上下文)

如果你的自定义事件与某个特定会话相关 (并不需要是会话事件)，你可以在触发事件的时候传入一个额外的一参数 `session`，以实现对触发上下文的过滤：

ts

    declare module 'koishi' {
      interface Events {
        'custom-event'(...args: any[]): void
      }
    }
    
    // ---cut---
    // @errors: 2304
    // 无法匹配该会话的上下文中注册的回调函数不会被执行 (可能有点绕)
    ctx.emit(session, 'custom-event', arg1, arg2, ...rest)

过滤触发上下文的效果将在 [过滤器](./../plugin/filter.html) 一节中详细介绍。

更一般地，即使是不使用会话的事件也能主动选择触发的上下文，其语法完全一致：

ts

    const thisArg = { [Context.filter]: callback }
    ctx.emit(thisArg, 'custom-event', arg1, arg2, ...rest)

触发事件时传入的一参数如果是对象，则会作为事件回调函数的 `this`。并且如果这个对象有 `Context.filter` 属性，那么这个属性将被用于过滤触发上下文。对应的值是一个函数，传入一个上下文对象，返回一个 boolean 表示是否应该在该上下文上触发该事件。而上面介绍的会话事件只是一种特殊情况而已。

自定义事件 [​](#自定义事件)
-----------------

在本节的最后，我们来聊聊插件扩展的事件系统。

如果你是插件的开发者，想要自定义一些事件，那么只需要在你的插件中添加下面的代码：

ts

    declare module 'koishi' {
      interface Events {
        // 方法名称对应自定义事件的名称
        // 方法签名对应事件的回调函数签名
        'kook/message-btn-click'(...args: any[]): void
      }
    }

如果你监听的事件由其他插件扩展而来，那么你同样需要通过一行额外的代码来导入相应的类型：

ts

    // 从 @koishijs/plugin-adapter-kook 导入事件类型
    // 这里的 import {} from 会在编译时被删除，不会影响运行时的行为
    // 请不要写成 import '@koishijs/plugin-adapter-kook'
    import {} from '@koishijs/plugin-adapter-kook'
    
    // 如果没有上面的类型导入，下面的代码会报错
    ctx.on('kook/message-btn-click', callback)

---



## [https://koishi.chat/zh-CN/guide/basic/middleware.html](https://koishi.chat/zh-CN/guide/basic/middleware.html)

中间件 [​](#中间件)
=============

有了接收事件和发送消息的能力，似乎你就能完成一切工作了——很多机器人框架也的确是这么想的。但是从 Koishi 的角度，这还远远不够。因为当我们面临更复杂的需求时，新的问题也会随之产生：如何限制消息能触发的应答次数？如何进行权限管理？如何提高机器人的性能？这些问题的答案将我们引向另一套更高级的系统——这也就是中间件的由来。

中间件是对消息事件处理流程的再封装。你注册的所有中间件将会由一个事件监听器进行统一管理，数据流向下游，控制权流回上游——这可以有效确保了任意消息都只被处理一次。被认定为无需继续处理的消息不会进入下游的中间件——这让我们能够轻易地实现权限管理。与此同时，Koishi 的中间件也支持异步调用，这使得你可以在中间件函数中实现任何逻辑。事实上，相比更加底层地调用事件监听器，**使用中间件处理消息才是 Koishi 更加推荐的做法**。

TIP

与事件系统的通用性不同，中间件专注于消息事件。你不能使用中间件处理其他类型的事件。

基本用法 [​](#基本用法)
---------------

还记得上一节介绍的 [基本示例](./events.html#基本用法) 吗？让我们把它改成中间件的形式：

ts

    // 如果收到“天王盖地虎”，就回应“宝塔镇河妖”
    ctx.middleware((session, next) => {
      if (session.content === '天王盖地虎') {
        return '宝塔镇河妖'
      } else {
        // 如果去掉这一行，那么不满足上述条件的消息就不会进入下一个中间件了
        return next()
      }
    })

中间件与事件的写法非常相似，但有三点区别：

*   事件使用 `ctx.on()` 注册，而中间件使用 `ctx.middleware()` 注册
*   中间件的回调函数接受额外的第二个参数 `next`，只有调用了它才会进入接下来的流程
*   中间件支持直接返回要发送的内容，而事件需要手动调用 `session.send()`

同事件类似，注册中间件时也会返回一个新的函数，调用这个函数就可以取消该中间件：

ts

    declare const callback: import('koishi').Middleware
    // ---cut---
    const dispose = ctx.middleware(callback)
    dispose() // 取消中间件

异步中间件 [​](#异步中间件)
-----------------

中间件也可以是异步的。下面给出一个示例：

ts

    ctx.middleware(async (session, next) => {
      // 获取数据库中的用户信息
      // 这里只是示例，事实上 Koishi 会自动获取数据库中的信息并存放在 session.user 中
      const user = await session.getUser(session.userId)
      if (user.authority === 0) {
        return '抱歉，你没有权限访问机器人。'
      } else {
        return next()
      }
    })

注意

异步中间件代码中，`next` 函数被调用时前面必须加上 await (或者 return)。如果删去将可能会导致时序错误，这在 Koishi 中将会抛出一个运行时警告。

前置中间件 [​](#前置中间件)
-----------------

从上面的两个例子中不难看出，中间件是一种消息过滤的利器。但是反过来，当你需要的恰恰是捕获全部消息时，中间件反而不会是最佳选择——因为更早注册的中间件可能会将消息过滤掉，导致你注册的回调函数根本不被执行。因此在这种情况下，我们更推荐使用事件监听器。然而，还存在着这样一种情况：你既需要捕获全部的消息，又要对其中的一些加以回复，这又该怎么处理呢？

听起来这种需求有些奇怪，让我们举个具体点例子吧：假如你写的是一个复读插件，它需要在每次连续接收到 3 条相同消息时进行复读。我们不难使用事件监听器实现这种逻辑：

ts

    let times = 0 // 复读次数
    let message = '' // 当前消息
    
    ctx.on('message', (session) => {
      // 这里其实有个小问题，因为来自不同群的消息都会触发这个回调函数
      // 因此理想的做法应该是分别记录每个群的当前消息和复读次数
      // 但这里我们假设机器人只处理一个群，简化示例的逻辑
      if (session.content === message) {
        times += 1
        if (times === 3) session.send(message)
      } else {
        times = 0
        message = session.content
      }
    })

但是这样写出的机器人就存在所有用事件监听器写出的机器人的通病——如果这条消息本身可以触发其他回应，机器人就会多次回应。更糟糕的是，你无法预测哪一次回应先发生，因此这样写出的机器人就会产生延迟复读的迷惑行为。为了避免这种情况发生，Koishi 对这种情况也有对应的解决方案，那就是 **前置中间件**。

与前置事件类似，向 `ctx.middleware()` 传入额外的第二个参数 `true` 以注册前置中间件。所有消息会优先经过前置中间件，像事件监听器一样，并且你获得了决定这条消息是否继续触发其他中间件的能力，这是事件监听器所不具有的。

ts

    let times = 0 // 复读次数
    let message = '' // 当前消息
    
    ctx.middleware((session, next) => {
      if (session.content === message) {
        times += 1
        if (times === 3) return message
      } else {
        times = 0
        message = session.content
        return next()
      }
    }, true /* true 表示这是前置中间件 */)

临时中间件 [​](#临时中间件)
-----------------

有的时候，你也可能需要实现这样一种逻辑：你的中间件产生了一个响应，但你认为这个响应优先级较低，希望等后续中间件执行完毕后，如果信号仍然未被截取，就执行之前的响应。这当然可以通过注册新的中间件并取消的方法来实现，但是由于这个新注册的中间件可能不被执行，你需要手动处理许多的边界情况。

为了应对这种问题 Koishi 提供了更加方便的写法：你只需要在调用 `next` 时再次传入一个回调函数即可！这个回调函数只接受一个 `next` 参数，且只会加入当前的中间件执行队列；无论这个回调函数执行与否，在本次中间件解析完成后，它都会被清除。下面是一个例子：

ts

    ctx.middleware((session, next) => {
      if (session.content === 'hlep') {
        // 如果该 session 没有被截获，则这里的回调函数将会被执行
        return next('你想说的是 help 吗？')
      } else {
        return next()
      }
    })

除此以外，临时中间件还有下面的用途。让我们先回到上面介绍的前置中间件。它虽然能够成功解决问题，但是如果有两个插件都注册了类似的前置中间件，就仍然可能发生一个前置中间件截获了消息，导致另一个前置中间件获取不到消息的情况发生。但是，借助临时中间件，我们便有了更好的解决方案：

ts

    let times = 0 // 复读次数
    let message = '' // 当前消息
    
    ctx.middleware((session, next) => {
      if (session.content === message) {
        times += 1
        if (times === 3) return next(message)
      } else {
        times = 0
        message = session.content
        return next()
      }
    }, true)

搭配使用上面几种中间件，你的机器人便拥有了无限可能。在 koishi-plugin-repeater 库中，就有着一个官方实现的复读功能，它远比上面的示例所显示的更加强大。如果想深入了解中间件机制，可以去研究一下这个功能的 [源代码](https://github.com/koishijs/koishi-plugin-repeater/blob/main/src/index.ts)。

---



## [https://koishi.chat/zh-CN/guide/basic/element.html](https://koishi.chat/zh-CN/guide/basic/element.html)

消息元素 [​](#消息元素)
===============

当然，一个聊天平台所能发送或接收的内容往往不只有纯文本。为此，我们引入了 **消息元素 (Element)** 的概念。

消息元素类似于 HTML 元素，它是组成消息的基本单位。一个元素可以表示具有特定语义的内容，如文本、表情、图片、引用、元信息等。Koishi 会将这些元素转换为平台所支持的格式，以便在不同平台之间发送和接收消息。

基本用法 [​](#基本用法)
---------------

一个典型的元素包含名称、属性和内容。在 Koishi 中，我们通常使用 JSX 或 API 的方式创建元素。下面是一些例子：

JSXAPI

JSX

    // 欢迎 @用户名 入群！
    session.send(<>欢迎 <at id={userId}/> 入群！</>)
    
    // 发送一张 Koishi 图标
    session.send(<img src="https://koishi.chat/logo.png"/>)

这两种写法各有优劣，不同人可能会有不同的偏好。但无论哪一种写法都表达了同样的意思。

### 使用 JSX [​](#使用-jsx)

学习 JSX 的写法需要你有一定的 HTML 基础 (如果有 React 基础将更好，尽管这不是必需的)。如果你不熟悉 HTML，可以参考 [这篇文档](https://developer.mozilla.org/zh-CN/docs/Glossary/Element)。

如果你已经学习过 HTML 的相关知识，你唯一额外需要了解的事情就是我们使用单花括号 `{}` 进行插值。你可以在单花括号中使用任何 JavaScript 表达式，它们会在运算完成后成为元素的一部分。此外，我们还为消息元素编写了完整的 [语法规范](./../../api/message/syntax.html)，供你参考。

### 使用 API [​](#使用-api)

对于更喜欢原生 JavaScript 的人，我们也提供了 API 的方式来创建元素。Koishi 提供一个 `h` 函数，它有着灵活的使用方式：

ts

    // 第一个参数是元素名称 (必选)
    h('message')
    
    // 你可以传入一个由属性构成的对象作为第二个参数
    h('quote', { id })
    
    // 后续参数是元素的内容，可以是字符串或其他元素
    h('p', {}, 'hello')
    
    // 没有属性时二参数可以忽略不写
    h('p', 'hello', h('img', { src }))

### 混用两种写法 [​](#混用两种写法)

虽然大部分情况下你可能并不想这么做 (看起来很怪不是吗)，但事实上这两种写法也是可以混用的。例如，你可以在 JSX 中使用 `h` 函数：

tsx

    // 欢迎 @用户名 入群！
    <>欢迎 {h('at', { id: userId })} 入群！</>

也可以反过来，将由 JSX 创建出的元素传入 `h` 函数的参数中：

tsx

    // 创建一个仅包含图片的消息
    h('message', <img src="https://koishi.chat/logo.png"/>)

标准元素 [​](#标准元素)
---------------

Koishi 提供了一系列标准元素，它们覆盖了绝大部分常见的需求。例如：

*   `at`：提及用户
*   `quote`：引用回复
*   `img`：嵌入图片
*   `message`：发送消息

尽管一个平台不太可能支持所有的行为，但适配器对每一个标准元素都进行了最大程度的适配。例如，对于不支持斜体的平台，我们会将斜体元素转换为普通文本；对于无法同时发送多张图片的平台，我们会将多张图片转换为多条消息分别发送等等。这样一来，开发者便可以在不同平台上使用同一套代码，而不用担心平台差异。

我们先对比较常用的一些元素进行介绍，你可以稍后在 [这个页面](./../../api/message/elements.html) 查看所有的标准元素。

### 提及用户和消息 [​](#提及用户和消息)

使用 `at` 元素提及用户：

html

    欢迎 <at id={userId}/> 入群！

Koishi

欢迎 @用户名 入群！

使用 `quote` 元素引用回复：

html

    <quote id={messageId}/> 你说得对

Koishi

> 原消息文本

你说得对

### 嵌入图片和其他资源 [​](#嵌入图片和其他资源)

使用 `img`, `audio`, `video` 和 `file` 元素嵌入图片、音频、视频和文件，它们的用法是类似的。这里以图片为例：

html

    <img src="https://koishi.chat/logo.png"/>

Koishi

上面是对于网络图片的用法，如果你想发送本地图片，可以使用 `file:` URL：

tsx

    import { pathToFileURL } from 'url'
    import { resolve } from 'path'
    
    // 发送相对路径下的 logo.png
    h.image(pathToFileURL(resolve(__dirname, 'logo.png')).href)
    
    // 等价于下面的写法
    <img src={pathToFileURL(resolve(__dirname, 'logo.png')).href}/>

如果图片以二进制数据的形式存在于内存中，你也可以直接通过 `h.image()` 构造 `data:` URL：

tsx

    // 这里的二参数是图片的 MIME 类型
    h.image(buffer, 'image/png')
    
    // 等价于下面的写法
    <img src={'data:image/png;base64,' + buffer.toString('base64')}/>

消息组件 实验性 [​](#消息组件)
-------------------

**消息组件 (Component)** 是一种对消息元素的扩展和封装。它允许你创建可重用的定制元素，并在渲染时引入自定义逻辑。例如，`<execute>` 组件会将其中的内容作为指令执行，并将执行结果替换该元素：

html

    这是执行结果：<execute>echo hello</execute>

Koishi

这是执行结果：hello

如你所见，你可以像使用普通的消息元素一样使用消息组件。唯一的区别是消息组件不由适配器实现，而是由 Koishi 直接处理。与之相对的，某些消息组件只有在特定的会话环境下才能使用 (例如在 `ctx.broadcast()` 中传入 `<execute>` 是无意义的，也会抛出错误)。

Koishi 已经内置了一系列消息组件，包括：

*   `<execute>`：执行指令
*   `<prompt>`：等待输入
*   `<i18n>`：国际化
*   `<random>`：随机选择

你可以在 [这个页面](./../../api/message/components.html) 了解每个组件的详细用法和适用范围。

### 定义消息组件 [​](#定义消息组件)

一个消息组件本质上是一个函数，它接受三个参数：

*   **attrs:** 元素的属性
*   **children:** 子元素列表
*   **session:** 当前会话

例如，下面的代码就定义了一个简单的消息组件：

ts

    // 请注意函数名必须以大写字母开头
    function Custom(attrs, children, session) {
      return '自定义内容'
    }

你可以直接在渲染时使用这个组件：

JSXAPI

JSX

    // 请注意这里的大写字母
    session.send(<Custom/>)

### 注册全局组件 [​](#注册全局组件)

上面的写法只能在当前文件中使用，并且必须以大写字母开头。如果想要更自然的写法，并将组件提供给其他插件使用，只需使用 `ctx.component()` 将它注册为一个全局组件：

ts

    ctx.component('custom', (attrs, children, session) => {
      return '自定义内容'
    })
    
    // 现在你可以在任何地方使用小写的 <custom/> 了
    session.send(<custom/>)

转义与解析 [​](#转义与解析)
-----------------

DANGER

直接发送未经转义的用户输入是非常危险的，因为它很容易导致 [XSS 攻击](https://zh.wikipedia.org/wiki/%E8%B7%A8%E7%B6%B2%E7%AB%99%E6%8C%87%E4%BB%A4%E7%A2%BC)。在使用诸如 `h.unescape()` 之类的 API 时，请务必确保输入的安全性。

在默认情况下，Koishi 会对指令参数进行转义以确保安全性。但在某些情况下，你可能希望手动处理消息元素的转义和解析。为此，我们提供了一系列实用方法：

*   [`h.escape()`](./../../api/message/api.html#h-escape): 转义字符串
*   [`h.unescape()`](./../../api/message/api.html#h-unescape): 反转义字符串
*   [`h.parse()`](./../../api/message/api.html#h-parse): 将字符串解析为消息元素
*   [`h.select()`](./../../api/message/api.html#h-select): 从消息元素中选择指定类型的元素
*   [`h.transform()`](./../../api/message/api.html#h-transform): 在消息元素中查找并替换指定类型的元素
*   [`h.transformAsync()`](./../../api/message/api.html#h-transformasync): 上述方法的异步版本

---



## [https://koishi.chat/zh-CN/guide/basic/advanced.html](https://koishi.chat/zh-CN/guide/basic/advanced.html)

进阶用法 [​](#进阶用法)
===============

在前面的几节中，我们已经了解了基础的交互概念。以他们为基础，Koishi 提供了一些进阶的用法，用于处理真实应用场景中的交互需求。

机器人对象 [​](#机器人对象)
-----------------

我们通常将机器人做出的交互行为分为两种：主动交互和被动交互。**主动交互**是指机器人主动进行某些操作，而**被动交互**则是指机器人接收到特定事件后做出的响应。一个机器人的大部分交互都应该是被动的，而主动交互则可用于一些特殊情况，比如定时任务、通知推送等。

Koishi 提供的交互性 API 可能存在于 `ctx`，`session` 和 `bot` 三种对象中。其中，上下文对象 `ctx` 可以在插件参数中取得，会话对象 `session` 可以在被动交互中取得，而机器人对象 `bot` 则可以从上述两个对象中访问到：

ts

    // 从 session 中访问 bot
    session.bot
    
    // 从 ctx 中访问 bot，其中 platform 和 selfId 分别是平台名称和机器人 ID
    ctx.bots[`${platform}:${selfId}`]

在之后的章节中，我们将进一步了解这三种对象的用法。

广播消息 [​](#广播消息)
---------------

主动交互中的一种常见需求是同时向多个频道发送消息。Koishi 提供了两套方法来实现消息的广播。最基础的写法是直接使用 `bot.broadcast()`：

ts

    // 一参数填写你要发送到的频道 ID 列表
    await bot.broadcast(['123456', '456789'], '全体目光向我看齐')

但这样写需要知道每一个频道对应哪个机器人。对于启用了多个机器人的场景下，这么写就有点不方便了。幸运的是，Koishi 还有另一个方法：`ctx.broadcast()`。在启用了数据库的情况下，此方法会自动获取每个频道的 [受理人](./../../manual/usage/customize.html#受理人机制)，并以对应的账号发送消息：

ts

    await ctx.broadcast(['telegram:123456', 'discord:456789'], '全体目光向我看齐')

等待输入 [​](#等待输入)
---------------

当你需要进行一些交互式操作时，可以使用 `session.prompt()`：

ts

    await session.send('请输入用户名：')
    
    const name = await session.prompt()
    if (!name) return '输入超时。'
    
    // 执行后续操作
    return `${name}，请多指教！`

你可以给这个方法传入一个 `timeout` 参数，或使用 `delay.prompt` 配置项，来作为等待的时间。

延时发送 [​](#延时发送)
---------------

如果你需要连续发送多条消息，那么在各条消息之间留下一定的时间间隔是很重要的：一方面它可以防止消息刷屏和消息错位 (后发的条消息呈现在先发的消息前面)，提高了阅读体验；另一方面它能够有效降低机器人发送消息的频率，防止被平台误封。这个时候，`session.sendQueued()` 可以解决你的问题。

ts

    // 发送两条消息，中间间隔一段时间，这个时间由系统计算决定
    await session.sendQueued('message1')
    await session.sendQueued('message2')
    
    // 清空等待队列
    await session.cancelQueued()

你也可以在发送时手动定义等待的时长：

ts

    import { Time } from 'koishi'
    
    // 如果消息队列非空，在前一条消息发送完成后 1s 发送本消息
    await session.sendQueued('message3', Time.second)
    
    // 清空等待队列，并设定下一条消息发送距离现在至少 0.5s
    await session.cancelQueued(0.5 * Time.second)

事实上，对于不同的消息长度，系统等待的时间也是不一样的，你可以通过配置项修改这个行为：

yaml

    delay:
      # 消息里每有一个字符就等待 0.02s
      character: 20
      # 每条消息至少等待 0.5s
      message: 500

这样一来，一段长度为 60 个字符的消息发送后，下一条消息发送前就需要等待 1.2 秒了。

执行指令 [​](#执行指令)
---------------

我们还可以实用 `session.execute()` 来让用户执行某条指令：

ts

    // 当用户输入“查看帮助”时，执行 help 指令
    ctx.middleware((session, next) => {
      if (session.content === '查看帮助') {
        return session.execute('help', next)
      } else {
        return next()
      }
    })

---



## [https://koishi.chat/zh-CN/guide/plugin/](https://koishi.chat/zh-CN/guide/plugin/)

认识插件 [​](#认识插件)
===============

TIP

在学习本章之前，建议先完整阅读 [入门 > 安装和配置插件](./../../manual/usage/market.html)。

模块化是 Koishi 的核心特性。借助插件系统，Koishi 得以将各种功能解耦出来，并以模块的形式分发。在「开发上手」中我们已经体验了基础的插件开发范例。本章将介绍更多的模块化编写方式，并介绍一些场景下的最佳实践。

插件的基本形式 [​](#插件的基本形式)
---------------------

一个插件需要是以下三种基本形式之一：

1.  一个接受两个参数的函数，第一个参数是所在的上下文，第二个参数是传入的配置项
2.  一个接受两个参数的类，第一个参数是所在的上下文，第二个参数是传入的配置项
3.  一个对象，其中的 `apply` 方法是第一种形式中所说的函数

而一个插件在被加载时，则相当于进行了上述函数的调用。因此，下面的四种写法是基本等价的：

ts

    declare const callback: Middleware
    /// ---cut---
    ctx.middleware(callback)
    
    ctx.plugin(ctx => ctx.middleware(callback))
    
    ctx.plugin({
      apply: ctx => ctx.middleware(callback),
    })
    
    ctx.plugin(class {
      constructor(ctx) {
        ctx.middleware(callback)
      }
    })

看起来插件似乎只是将函数调用换了一种写法，但这种写法能够帮助我们将多个逻辑组合在一起并模块化，同时可以在插件内部对所需的选项进行初始化，这些都能极大地提高了代码的可维护性。

模块化的插件 [​](#模块化的插件)
-------------------

插件化最大的好处就是可以把不同的功能写在不同的模块中。此时插件将作为模块的导出，它可以是 [默认导出](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/import#%E5%AF%BC%E5%85%A5%E9%BB%98%E8%AE%A4%E5%80%BC) 或 [导出整体](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/import#%E5%AF%BC%E5%85%A5%E6%95%B4%E4%B8%AA%E6%A8%A1%E5%9D%97%E7%9A%84%E5%86%85%E5%AE%B9)。

对于对象形式的插件，你还可以额外提供一个 `name` 属性作为插件的名称。对于函数和类形式的插件来说，插件名称便是函数名或类名。具名插件有助于更好地描述插件的功能，并被用于插件关系可视化中，实际上不会影响任何运行时的行为。

foo.ts

    // 整体导出对象形式的插件
    export interface Config {}
    
    export const name = 'Foo'
    
    export function apply(ctx: Context, config: Config) {}

bar.ts

    // 默认导出类形式的插件
    class Bar {
      constructor(ctx: Context, config: Bar.Config) {}
    }
    
    namespace Bar {
      export interface Config {}
    }
    
    export default Bar

嵌套的插件 [​](#嵌套的插件)
-----------------

Koishi 的插件也是可以嵌套的。你可以将你编写的插件解耦成多个独立的子模块，再将调用这些子模块的一个新插件作为入口模块，就像这样：

index.ts

    // 入口文件，从上述模块分别加载插件
    import Foo from './foo'
    import * as Bar from './bar'
    
    export function apply(ctx: Context) {
      ctx.plugin(Foo)
      ctx.plugin(Bar)
    }

这样当你加载上述模块时，就相当于同时加载了 foo 和 bar 两个模块。这样的做法不仅能够减轻心智负担，解耦出的模块还享受独立的热重载，你可以在不影响一个模块运行的情况下修改另一个的代码！

当你在开发较为复杂的功能时，可以将插件分解成多个独立的子插件，并在入口文件中依次加载这些子插件。许多大型插件都采用了这种写法。

在配置文件中加载 [​](#在配置文件中加载)
-----------------------

一个模块可以作为插件被 Koishi 的配置文件加载，其需要满足以下两条中的一条：

*   此模块的**默认导出**是一个插件
*   此模块的**导出整体**是一个插件

这两种写法并无优劣之分，你完全可以按照自己的需求调整导出的形式。按照惯例，如果你的插件是一个函数，我们通常直接导出 apply 方法，并将导出整体作为一个插件；如果你的插件是一个类，那么我们通常使用默认导出的形式。

TIP

这里默认导出的优先级更高。因此，只要模块提供了默认导出，Koishi 就会尝试加载这个默认导出，而不是导出整体。在开发中请务必注意这一点。

配置文件中的 `plugins` 字段记录了插件的信息：

koishi.yml

    plugins:
      console:
      dialogue:
        prefix: '#'

这里的键对应插件的路径，值则为插件的配置。这个路径的解析逻辑如下：

*   对于 foo，我们将尝试读取 @koishijs/plugin-foo 和 koishi-plugin-foo
*   对于 @foo/bar，我们将尝试读取 @foo/koishi-plugin-bar

换言之，上述配置文件相当于下面的代码：

ts

    app.plugin(require('@koishijs/plugin-console').default)
    app.plugin(require('koishi-plugin-dialogue'), { prefix: '#' })

在这个例子中，console 是官方插件，并且使用了默认导出；dialogue 是社区插件，并且使用了导出整体。配置文件使你得以无视这些区别，每个插件的加载方式都会由 CLI 自动检测。

---



## [https://koishi.chat/zh-CN/guide/plugin/schema.html](https://koishi.chat/zh-CN/guide/plugin/schema.html)

配置构型 [​](#配置构型)
===============

在上一节中，我们已经了解了插件的本质是一个接受了上下文和配置项的函数。但仅仅是接受任意格式的输入是不够的，我们还需要对配置项进行一些约束，以确保插件能够正常运行。为此，我们开发了 [schemastery](https://github.com/shigma/schemastery) 这个工具，并将它集成到了 Koishi 中。这个工具可以帮助你：

*   验证某个配置项是否合法
*   为可缺省的配置项提供默认值
*   在控制台中通过表单让用户进行在线配置

让我们来看看它是如何工作的。

基本示例 [​](#基本示例)
---------------

让我们看一个简单的示例。下面的插件将注册一个指令，输出当前插件的配置项。

ts

    import { Context, Schema } from 'koishi'
    
    export const name = 'example'
    
    export interface Config {
      foo: string
      bar?: number
    }
    
    export const Config: Schema<Config> = Schema.object({
      foo: Schema.string().required(),
      bar: Schema.number().default(1),
    })
    
    export function apply(ctx: Context, config: Config) {
      ctx.command('config').action(() => {
        // 输出当前的配置
        return `foo: ${config.foo}\nbar: ${config.bar}`
      })
    }

在这个示例中，我们的插件导出了一个 `Config` 类型和一个同名的 `Schema` 对象。前者为我们的插件提供了类型，而后者则生成了对配置项的约束。我们可以看到，这个插件的配置项有两个属性，`foo` 是必需的，而 `bar` 则是可选的。如果你不填写 `foo`，那么插件在启动时就会报错；而如果你不填写 `bar`，那么它将会被赋予默认值 `1`。

描述类型信息 [​](#描述类型信息)
-------------------

除了 `string`, `number`, `boolean` 等类型外，Koishi 同样支持 `array`, `dict`, `object` 等复合类型。你可以组合使用它们来构造出更复杂的配置项。

ts

    Schema.object({
      foo: Schema.array(Schema.string()),
      bar: Schema.dict(Schema.number()),
      baz: Schema.object({
        quz: Schema.boolean(),
      }),
    })

你可以通过 `Schema` 对象的静态方法来创建这些类型；而对于已经创建的类型，你还可以通过链式调用的方式添加更多信息：

ts

    Schema.number()
      // 限制取值范围
      .min(0).max(100).step(1)
      // 设置默认值
      .default(50)
      // 以滑动条的形式显示
      .role('slider')
      // 设置描述信息
      .description('这是一个介于 0 和 100 之间的整数。')

我们能做的还远不止于此。一些高级类型如 `intersect` 可用于将类型的分组显示；而 `union` 则可以创造联合类型。通过恰当地组合它们，你甚至可以构造出上下关联的配置项！

为了帮助你更好地理解这些类型，我们专门编写了在线的 [配置演练场](./../../schema/)。所有类型的详细信息和用法示例都可以在这里找到。

插件的元属性 [​](#插件的元属性)
-------------------

需要注意的是，`Config` 应当是导出的插件的一个属性。因此，如果你使用默认导出，推荐你使用 `namespace` 来声明插件的配置：

ts

    class Example {
      constructor(ctx: Context, config: Example.Config) {
        // 这里是插件实现
      }
    }
    
    namespace Example {
      export interface Config {}
    
      export const Config: Schema<Config> = Schema.object({
        // 这里是配置声明
      })
    }
    
    export default Example

形如 `name` 和 `Config` 这样的属性，我们称之为插件的元属性。它们需要与插件的入口函数同级导出。例如，你还可以通过导出 `usage` 属性来为插件提供使用方法。这样一来，一个完整的插件就可以写成这样：

ts

    export const name = 'example'
    export const usage = '这是一个示例插件。'
    export interface Config {}
    export const Config: Schema<Config> = Schema.object({})
    export function apply(ctx: Context, config: Config) {}

类似的属性还有 `reusable`, `using`, `filter` 等等，我们将在接下来的几节中介绍它们的用法。

---



## [https://koishi.chat/zh-CN/guide/plugin/lifecycle.html](https://koishi.chat/zh-CN/guide/plugin/lifecycle.html)

生命周期 [​](#生命周期)
===============

在 [事件系统](./../basic/events.html) 中，我们已经了解了由聊天平台推送的会话事件。除此以外，Koishi 也提供了一些生命周期事件。这些事件会在某些 Koishi 的运行阶段被触发，你可以通过监听它们来实现各种各样的功能。本节主要介绍与插件开发相关的一些核心事件。

要了解 Koishi 所提供的全部事件，可以参考 [事件列表](./../../api/core/events.html)。

异步加载与 `ready` 事件 [​](#异步加载与-ready-事件)
-------------------------------------

`ready` 事件在应用启动时触发。如果一个插件在加载时，应用已经处于启动状态，则会立即触发。在下面的场景建议将逻辑放入 `ready` 事件：

*   含有异步操作 (比如文件操作，网络请求等)
*   希望等待其他插件加载完成后才执行的操作

副作用与 `dispose` 事件 [​](#副作用与-dispose-事件)
---------------------------------------

### 停用插件 [​](#停用插件)

之前我们已经了解了插件的启用，而 Koishi 同样支持在运行时停用一个插件。`ctx.plugin()` 返回一个 `Fork` 对象。调用 `fork.dispose()` 可以停用一个插件。

ts

    import { Context } from 'koishi'
    
    function callback(ctx: Context) {
      // 编写你的插件逻辑
      ctx.on('message', callback1)
      ctx.command('foo').action(callback2)
      ctx.middleware(callback3)
      ctx.plugin(require('another-plugin'))
    }
    
    // 加载插件
    const fork = ctx.plugin(callback)
    
    // 停用这个插件，取消上述全部副作用
    fork.dispose()

对于可重用的插件，`fork.dispose()` 也只会停用 `fork` 对应的那一次。如果你想取消全部的副作用，可以使用 `ctx.registry.delete()`：

ts

    // 移除可重用插件的全部副作用
    ctx.registry.delete(plugin)

### 清除副作用 [​](#清除副作用)

Koishi 的插件系统支持热重载，即任何一个插件可能在运行时被多次加载和卸载。要实现这一点，我们就必须在插件被卸载时清除它的所有副作用。

绝大部分 `ctx` 方法都会在在插件被停用自动回收副作用；然而，如果你使用了 `ctx` 之外的方法，你的代码还可能通过其他方式引入副作用，这时就需要通过 `dispose` 事件来手动清除它们。下面是一个例子：

ts

    // 一个示例的服务器插件
    import { Context } from 'koishi'
    import { createServer } from 'http'
    
    export function apply(ctx: Context, config) {
      const server = createServer()
    
      ctx.on('ready', () => {
        // 在插件启动时监听端口
        server.listen(1234)
      })
    
      ctx.on('dispose', () => {
        // 在插件停用时关闭端口
        server.close()
      })
    }

可重用性与 `fork` 事件 [​](#可重用性与-fork-事件)
-----------------------------------

### 可重用插件 [​](#可重用插件)

到此为止，我们所介绍的插件开发都限定在插件只能同时启用一份的情况。如果你想要在同一个应用中同时启用多份插件，会发生什么呢？

ts

    function callback() {
      console.log('called')
    }
    
    ctx.plugin(callback)
    ctx.plugin(callback)

执行上面的代码，你会发现 `called` 只会被打印一次。这是因为 `ctx.plugin()` 会检测插件是否已经被加载：如果是，则会直接返回之前的 `Fork` 对象，而不会再次执行插件的逻辑。

采用这种设计的主要原因是，插件往往会占用某些资源，因此重复启用会导致预期之外的问题。例如，一个插件注册了某个指令，如果重复启用，那么这个指令也会被重复注册。而当用户调用这个指令时，究竟要执行哪个指令的逻辑呢？这显然是不合理的。

不过也不能因此就认为所有插件都不应该被重用。如果你真的有这样的需求，Koishi 也提供了方法——只需声明插件的 `reusable` 属性为 `true` 即可。参考下面的例子：

reply.ts

    export const name = 'reply'
    export const reusable = true    // 声明此插件可重用
    
    export interface Config {
      input: string
      output: string
    }
    
    export function apply(ctx: Context, config: Config) {
      ctx.middleware((session, next) => {
        // 当用户发送 input 时，回复 output
        if (session.content === config.input) {
          return config.output
        }
        return next()
      })
    }

然后我们可以多次调用此插件了：

ts

    import * as reply from './reply'
    
    ctx.plugin(reply, { input: '天王盖地虎', output: '宝塔镇河妖' })
    ctx.plugin(reply, { input: '宫廷玉液酒', output: '一百八一杯' })

如果你在开发类形式的插件，那么可以在类的静态属性中声明 `reusable`，效果是一样的：

bar.ts

    export default class Bar {
      static reusable = true
      constructor(ctx: Context) {}
    }

### 维护共享状态 [​](#维护共享状态)

一种更复杂的情况是，我们既需要插件可重用，又需要维护一些共享状态。例如，我们能否编写一个指令，使得它总是返回插件被调用的次数呢？这时候 `fork` 事件就派上用场了：

count.ts

    export const name = 'count'
    
    export function apply(ctx: Context) {
      let count = 0         // 这里保存了共享状态
    
      ctx.command('count').action(() => {
        return `此插件已被调用 ${count} 次。`
      })
    
      ctx.on('fork', (ctx) => {
        count += 1
        ctx.on('dispose', () => {
          count -= 1
        })
      })
    }

我们可以看到，上面的插件并没有声明 `reusable` 属性，取而代之的是监听了 `fork` 事件。`fork` 是一个生命周期事件，当插件每次被调用时都会触发。因此，我们可以在 `fork` 事件中对共享状态进行更新。我们每创建一个新的 `Fork` 对象，就会增加一次 `count`；而每当 `Fork` 对象被停用，就会减少一次 `count`；当用户调用指令时，我们只需要返回 `count` 的值即可。

`fork` 事件实际上将插件分割成了两个不同的作用域。外侧的代码仍然只会被执行一次，对应着不可重用的部分；而内侧的代码则会被执行多次，对应着可重用的部分。在上面的例子中，只需将指令的注册放在外侧作用域中，这样就不用担心重复注册的问题了。

最后，`fork` 事件的回调函数与插件本身类似，也接受 `ctx` 和 `config` 两个参数，分别对应于该次调用时传入插件的参数。外侧和内侧的 `ctx` 含义不同，请格外注意。

### 嵌套插件的可重用性 [​](#嵌套插件的可重用性)

让我们重新梳理一下可重用插件的概念：

1.  根据插件的 `reusable` 属性，可以将插件分为可重用插件和不可重用插件：不可重用插件被调用多次时，只会执行一次插件逻辑；而可重用插件被调用多次时，会执行多次插件逻辑；
2.  这两种类型本质上都可以使用 `fork` 事件来表达：不可重用插件的逻辑写在 `fork` 事件的外侧，而可重用插件的逻辑写在 `fork` 事件的内侧。

当我们嵌套使用可重用插件和不可重用插件时，又会发生什么呢？让我们来看一些例子吧。

#### 情况一：不可重用插件嵌套可重用插件 [​](#情况一-不可重用插件嵌套可重用插件)

实际上我们会发现，`reusable` 属性只是 `fork` 事件的语法糖。下面两种写法是等价的：

ts

    ctx.plugin({
      reusable: true,
      apply: (ctx) => {
        ctx.middleware(callback)
      },
    })

ts

    ctx.plugin((ctx) => {
      ctx.on('fork', (ctx) => {
        ctx.middleware(callback)
      })
    })

然而，如果你直接将可重用插件嵌套在不可重用插件中，由于外层的插件只会执行一次，所以内层的插件也并不会被重复执行。这显然不是我们想要的结果。这就是为什么我们需要 `fork` 事件。当你需要在不可重用的插件中重用某段代码，你就应该使用 `fork` 事件，就像上面的例子一样。

#### 情况二：可重用插件嵌套不可重用插件 [​](#情况二-可重用插件嵌套不可重用插件)

反过来的情况则更加自然：如果你在可重用插件内调用了一个不可重用的插件，那么可重用插件将被多次执行，而不可重用则会确保只被执行一次。这种写法常常用于注册指令或其他服务：

ts

    export function apply(ctx: Context) {
      // 注册指令
      ctx.command('foo').action(callback)
    
      // 扩展控制台
      ctx.console.addEntry('/client')
    }

ts

    import * as internal from './internal'
    
    export const reusable = true
    
    export function apply(ctx: Context, config: Config) {
      // 不可重用的部分被嵌套在独立的插件中
      ctx.plugin(internal)
    
      // 中间件是可以重复注册的
      ctx.middleware(callback)
    }

重新认识上下文 [​](#重新认识上下文)
---------------------

从学习 Koishi 开发的一开始，我们就已经接触到了 **上下文 (Context)** 这个概念。我们所熟悉的 `ctx.on()`, `ctx.middleware()` 以及 `ctx.command()` 等等 API 都是上下文类所提供的方法。而在本节中，我们进一步看到，上下文在插件开发中扮演着非常重要的角色。

上下文描述了机器人的一种可能的运行环境，而插件则是在这个环境中运行的。每个插件的上下文互不相同，这才保证了插件的副作用可以被有效地回收。

对于完整的运行环境有许多的刻画方式，而副作用的回收正是其中的一种。基于副作用的上下文也可以称为插件上下文。在接下来的章节中，我们还将看到运行环境的其他刻画维度，包括基于依赖的服务上下文和基于过滤器的会话上下文。

---



## [https://koishi.chat/zh-CN/guide/plugin/service.html](https://koishi.chat/zh-CN/guide/plugin/service.html)

服务与依赖 [​](#服务与依赖)
=================

在之前的章节中，你或许已经意识到了 Koishi 的大部分特性都是围绕上下文进行设计的——即使不同的上下文可以隶属于不同的插件、配置不同的过滤器，但许多功能在不同的上下文中访问的效果是一致的。换言之，应用其实可以被理解成一个容器，搭载了各种各样的功能 (如数据库和适配器等)，而上下文则单纯提供了一个接口来访问它们。这种组织形式被称为 **服务 (Service)**。

对于已经有 IoC / DI 概念的同学来说，服务就是一种类似于 IoC 的实现 (但并非通过 DI 实现)。Service API 通过 TypeScript 特有的 **声明合并 (Declaration Merging)** 机制提供了容器内服务的快速访问。

服务的类型 [​](#服务的类型)
-----------------

Koishi 中的服务可以分为大致三种类型。对于每一种我都给出了一些例子。

第一种是由 **Koishi 自带的服务**。只要有上下文对象，你就可以随时访问这些服务。

*   ctx.model：提供数据模型
*   ctx.i18n：提供国际化能力

第二种是由 **Koishi 所定义但并未实现的服务**。你可以选择适当的插件来实现它们。在你安装相应的插件之前，相关的功能是无法访问的。

*   ctx.assets：转存资源文件
*   ctx.database：封装数据库操作

实现特定服务的插件名通常以服务名作为前缀，例如 assets-local, database-mysql 等等。这并非强制的要求，但我们建议插件开发者也都遵循这个规范，这有助于让使用者对你插件的功能建立一个更明确的认识。

最后一种则是 **由插件定义和实现的服务**。通常情况下你需要声明这些服务作为依赖。关于插件与服务的依赖关系，会在下面具体介绍。

*   ctx.console：网页控制台
*   ctx.puppeteer：浏览器截图

服务的依赖关系 [​](#服务的依赖关系)
---------------------

前面从服务提供者的角度提供了解决方案，现在让我们把视角转换到服务的使用者上。假设你正在开发名为 dialogue 的问答系统，并且这个插件依赖多个服务：

*   `database`：你使用数据库存储教学内容，离开数据库你的插件将无法运行
*   `assets`：你需要使用资源存储服务来做图片转存，离开此服务将可能导致部分图片无法正常显示，但短时间内不会对插件的运行造成影响
*   `console`：你为你的插件编写了控制台扩展，当控制台存在时你可以在网页中进行操作，但它并非教学系统的主要功能

那么你应该怎么写呢？先让我们来看一段标准错误答案：

ts

    // 标准错误答案！别抄这个！
    export const name = 'dialogue'
    
    export function apply(ctx: Context) {
      // 检查数据库服务是否存在
      if (!ctx.database) return
    
      ctx.command('dialogue').action((_, content) => {
        // 检查资源存储服务是否存在
        if (ctx.assets) ctx.assets.transform(content)
      })
    
      // 检查控制台服务是否存在
      if (ctx.console) {
        ctx.console.addEntry('/path/to/dialogue/extension')
      }
    }

你很快会发现这样写完全无法运行。首先，数据库服务需要等到应用启动完成后才可以访问，换言之即使安装了数据库插件，你也无法立即判断数据库服务是否存在。此外，一旦上述服务所在插件在运行时被重载，由于上面的代码属于 dialogue 插件，因此 if 中代码的副作用将无法被有效清理；而当相应的服务重新被注册时，这部分的代码也不会被重新运行，从而导致一系列难以检测的问题。

### inject 属性 [​](#inject)

为了解决这种问题，Koishi 为插件声明提供了一个独特的 `inject` 属性：

ts

    export const name = 'dialogue'
    export const inject = ['database']
    
    export function apply(ctx: Context) {
      // 你可以立即访问数据库服务
      ctx.database.get('dialogue', {})
    }

`inject` 可以是一个数组或者对象。这里使用了数组，表示此插件依赖的服务列表。怎么理解这里的依赖关系呢？如果你声明了某个服务作为插件的依赖：

*   直到此服务的值变为 truthy 为止，该插件的函数体不会被加载
*   一旦此服务的值发生变化，该插件将立即回滚 (并非插件停用)
*   如果变化后的值依旧为 truthy，该插件会在回滚完成后被重新加载

对于部分功能依赖某个服务的插件，有两种方式可以实现。第一种情况下，你可以把这部分功能独立为一个子插件。此时，Koishi 提供了一个语法糖 `ctx.inject()`：

ts

    ctx.inject(['console'], (ctx) => {
      ctx.console.addEntry('/path/to/dialogue/extension')
    })
    
    // 等价于
    ctx.plugin({
      using: ['console'],
      apply: (ctx) => {
        ctx.console.addEntry('/path/to/dialogue/extension')
      },
    })

TIP

请注意：这里出现了两个 `ctx` 对象，它们属于不同的插件。在子插件的回调函数内，请务必使用作为参数的 `ctx` 而不是外层的 `ctx`，不然在服务被热重载时可能会引发内存泄漏。

另一种情况是，插件依赖的服务仅仅在运行时判断并使用，并不提供任何副作用。此时可以将 `inject` 声明为一个对象，其含有 `required` 和 `optional` 两个可选的属性，分别表示必需依赖和可选依赖。这样声明的可选依赖同样可以在插件体中直接使用，但插件的生命周期并不会实际依赖该服务。换句话说，插件不会等待该服务加载，也不会因为服务的变化而回滚。

ts

    export const inject = {
      optional: ['assets'],
    }
    
    export function apply(ctx: Context) {
      ctx.command('dialogue').action((_, content) => {
        // 检查资源存储服务是否存在
        if (ctx.assets) ctx.assets.transform(content)
      })
    }

### 最佳实践 [​](#最佳实践)

在上面的讨论中，我们已经分别介绍了 dialogue 插件所用到的三个服务的声明方式。现在让我们把它们结合起来，看看最佳实践应该是怎样的。请注意不同服务的处理方式之间的区别。

ts

    // 正确答案！抄这个！
    export const name = 'dialogue'
    
    // 对于整体依赖的服务，使用 inject 属性声明依赖关系
    export const inject = {
      required: ['database'],
      optional: ['assets'],
    }
    
    export function apply(ctx: Context) {
      ctx.command('dialogue').action((_, content) => {
        // 对于可选的依赖服务，在运行时检测即可
        if (ctx.assets) ctx.assets.transform(content)
      })
    
      // 对于部分功能依赖的服务，使用 ctx.inject() 注册为子插件
      ctx.inject(['console'], (ctx) => {
        ctx.console.addEntry('/path/to/dialogue/extension')
      })
    }

自定义服务 [​](#自定义服务)
-----------------

如果你希望自己插件提供一些接口供其他插件使用，那么最好的办法便是提供自定义服务，就像这样：

ts

    export default class Console extends Service {
      constructor(ctx: Context) {
        super(ctx, 'console')
      }
    }

这样定义的好处在于，`Console` 本身也是一个合法的插件，其他插件可以直接通过 `ctx.plugin(Console)` 来加载它。

对于 TypeScript 用户，在定义服务时，你还需要进行声明合并，以便能够在上下文对象中获得类型提示：

ts

    declare module 'koishi' {
      interface Context {
        console: Console
      }
    }

而使用服务的插件则需要声明依赖并导入类型：

ts

    import {} from 'koishi-plugin-console'
    
    export const inject = ['console']
    
    export function apply(ctx: Context) {
      ctx.console.addEntry('/path/to/dialogue/extension')
    }

### 服务的生命周期 [​](#服务的生命周期)

`Service` 抽象类的构造函数支持三个参数：

*   `ctx`：服务所在的上下文对象
*   `name`：服务的名称 (即其在所有上下文中的属性名)
*   `immediate`：是否立即注册到所有上下文中 (可选，默认为 `false`)

以及三个可选的抽象方法：

*   `start()`：在 `ready` 事件触发时调用
*   `stop()`：在 `dispose` 事件触发时调用
*   `fork()`：在 `fork` 事件触发时调用

默认情况下，一个自定义服务会先等待 ready 事件触发，然后调用可能存在的 `start()` 方法，最后才会被注册到全体上下文中。这种设计确保了服务在能够被访问的时候就已经是可用的。但如果你的服务不需要等待 ready 事件，那么只需传入第三个参数 `true` 就可以立即将服务注册到所有上下文中。

此外，当注册了服务的插件被卸载时，其注册的服务也会被移除，通过 `inject` 声明依赖的插件也会被停止运行，直到服务再次被实现。这意味着开发者不需要担心服务的生命周期，只需要专注于提供或使用服务的功能即可。

### 支持热重载 [​](#支持热重载)

既然服务的作用是提供接口供其他插件调用，就自然会涉及一个热重载的问题。如果某个插件先调用了服务上的方法，然后被卸载，那么我们就需要处理调用所带来的副作用。让我们来看一段 console 插件的源码：

ts

    interface Console {
      entries: Set<string>
      triggerReload(): void
    }
    // ---cut---
    class Console extends Service {
      // 这个方法的作用是添加入口文件
      addEntry(filename: string) {
        this.entries.add(filename)
        this.triggerReload()
    
        // 注意这个地方，ctx 属性会指向访问此方法的上下文 (而不是构造函数中的上下文)
        // 只需要在这个上下文上监听 dispose 事件，就可以顺利处理副作用了
        this.ctx.on('dispose', () => {
          this.entries.delete(filename)
          this.triggerReload()
        })
      }
    }

在 `package.json` 中声明依赖 [​](#package-json)
-----------------------------------------

如果你打算将插件发布到插件市场，我们建议在插件的 `package.json` 中对其所提供和使用的服务进行声明。这些字段将显示在控制台中插件的详情页中，帮助使用者更好地理解插件的功能。

package.json

    {
      "koishi": {
        "service": {
          "required": ["database"],
          "optional": ["assets", "console"],
          "implements": ["dialogue"]
        }
      }
    }

在这里，`required` 对应于必需依赖，`optional` 对应于可选依赖，`implements` 对应于提供的服务。如果你的插件没有使用或提供服务，那么对应的字段可以省略。

### 对比 `inject` 声明 [​](#inject-vs-dep)

对于任何依赖服务的插件，其必须声明 `inject` 才能正常工作，但缺失 `package.json` 中的声明并不会影响插件的运行。尽管如此，我们依然建议你在 `package.json` 中声明依赖，因为这样做能够在安装时提供更多信息，使用者可以一次性地安装插件所需的所有依赖，而不是等到插件运行时才发现缺少了某个服务。

### 关于 `peerDependencies` [​](#peer-vs-dep)

一个很容易混淆的概念是 `package.json` 自带的 `peerDependencies` 字段。这个字段用于声明一个 npm 包的依赖，但声明的依赖需要由用户安装 (或由包管理器自动安装到依赖树顶层)。是不是跟服务的概念非常像？它们之间的区别如下：

1.  `peerDependencies` 描述的是 npm 包的运行时行为。如果对应的依赖不存在，那么程序预期无法正常运行 (除非在 `peerDependenciesMeta` 中指明可选性)。而对于 Koishi 插件来说，由于有了 `inject` 机制，即使依赖的服务不存在，程序也不会崩溃。
    
2.  `peerDependencies` 是一对一的关系，即依赖的只能是另一个确定的包。而 Koishi 中的服务则是一对多的关系，即依赖的服务可以被多个插件所提供。
    

基于以上两点，关于是否要在插件的 `package.json` 中为服务声明 `peerDependencies`，我们可以根据插件从依赖中导入的内容来判断：

#### 情况一：插件仅导入了类型声明 [​](#情况一-插件仅导入了类型声明)

这是绝大部分的情况。在这种情况下，我们无需声明 `peerDependencies`，但建议把依赖加入 `devDependencies` 中。下面将以 puppeteer 插件提供的服务为例介绍：

ts

    // import {} 的意思是，我们只需要类型声明，而不需要导入任何内容
    // 在编译后，这个语句会被移除，不会引入任何副作用
    import {} from 'koishi-plugin-puppeteer'
    
    // 通过 inject 属性声明依赖，并通过 ctx 来访问服务
    export const inject = ['puppeteer']
    export function apply(ctx: Context) {
      ctx.puppeteer.render()
    }

此时插件的 `package.json` 可以这样写：

package.json

    {
      "service": {
        "required": ["puppeteer"]
      },
      "devDependencies": {
        "koishi-plugin-puppeteer": "^2.0.0"
      }
    }

#### 情况二：插件导入了类型声明以外的内容 [​](#情况二-插件导入了类型声明以外的内容)

一个典型的例子是 console 服务。一些控制台扩展需要从 `@koishijs/plugin-console` 中导入 `DataService` 基类。此时你的代码应该是这样的：

ts

    import { DataService } from '@koishijs/plugin-console'
    
    export class ExamplePlugin extends DataService {
      // ...
    }

此时你需要同时声明 `peerDependencies` 和 `devDependencies`：

json

    {
      "service": {
        "required": ["console"]
      },
      "peerDependencies": {
        "@koishijs/plugin-console": "^5.13.0"
      },
      "devDependencies": {
        "@koishijs/plugin-console": "^5.13.0"
      }
    }

---



## [https://koishi.chat/zh-CN/guide/plugin/filter.html](https://koishi.chat/zh-CN/guide/plugin/filter.html)

过滤器 [​](#过滤器)
=============

TIP

在学习本节之前，建议先完整阅读 [入门 > 过滤器](./../../manual/usage/customize.html#filters)。

默认情况下，一个会话事件、中间件或者指令都对所有的会话生效。但如果我们希望这些功能只对部分群聊或者用户生效，我们就需要用到 **过滤器**。

属性过滤器 [​](#属性过滤器)
-----------------

WARNING

请不要滥用这项功能：在源码中直接书写账号或群号会导致隐私泄露，并且其他用户无法使用你的插件。推荐 [在配置文件中使用过滤器](#配置文件中的过滤器)。

让我们先从最简单的会话过滤器开始。**属性过滤器**可以用来快速创建满足特定条件的子上下文：

ts

    ctx.user('112233')                  // 选择来自用户 112233 的会话
    ctx.self('112233')                  // 选择发送给机器人 112233 的会话
    ctx.guild('445566')                 // 选择来自群组 445566 的会话
    ctx.channel('778899')               // 选择来自频道 778899 的会话
    ctx.platform('discord')             // 选择来自平台 discord 的会话

这种写法也支持链式的调用：

ts

    // 选择来自平台 discord 中用户 112233 的会话
    ctx.platform('discord').user('112233')

利用上下文，你可以非常方便地对每个环境进行分别配置：

ts

    declare const callback: Middleware
    declare const listener: (session: Session) => void
    /// ---cut---
    // 在所有环境注册中间件
    ctx.middleware(callback)
    
    // 注册指令 my-command，仅对机器人 112233 有效
    ctx.self('112233').command('my-command')
    
    // 当有人申请加群 445566 时触发 listener
    ctx.guild('445566').on('guild-request', listener)
    
    // 安装插件 ./my-plugin，仅限 Telegram 平台使用
    ctx.platform('telegram').plugin(require('./my-plugin'))

是不是非常方便呢？

条件过滤器 [​](#条件过滤器)
-----------------

如果简单的会话过滤器无法满足你的需求，你也可以给一个上下文添加**条件过滤器**：它传入一个会话对象，并返回一个布尔类型。条件过滤器有三种添加方式：

ts

    // 满足当前上下文条件，且消息内容为“啦啦啦”
    ctx.intersect(session => session.content === '啦啦啦')
    
    // 满足当前上下文条件，或消息内容为“啦啦啦”
    ctx.union(session => session.content === '啦啦啦')
    
    // 满足当前上下文条件，且消息内容不为“啦啦啦”
    ctx.exclude(session => session.content === '啦啦啦')

上述方法也可以传入一个上下文作为参数，分别表示两个上下文的交集、并集和差集：

ts

    // 选择来自群组 1122233 和用户 445566 的会话
    ctx.guild('112233').intersect(ctx.user('445566'))
    
    // 选择来自群组 1122233 或用户 445566 的会话
    ctx.guild('112233').union(ctx.user('445566'))
    
    // 选择来自群组 1122233 的会话，但来自用户 445566 的会话除外
    ctx.guild('112233').exclude(ctx.user('445566'))

与选择器方法类似，过滤器方法也会返回一个新的上下文，你可以在其上自由的添加监听器、中间件、指令和插件。

配置文件中的过滤器 [​](#配置文件中的过滤器)
-------------------------

如果你遵循了模块化的开发理念，你的插件应该具有较为独立的功能。那么此时，你的插件内部其实并不需要使用过滤器，而是在插件加载时指定一次即可。在这种情况下，Koishi 提供了直接在配置文件中指定过滤器的方法：

koishi.yml

    plugins:
      repeater:
        $filter:
          # 仅在 telegram 平台下 2 个特定频道内注册插件
          $and:
            - $eq:
                - $: platform
                - telegram
            - $in:
                - $: channel
                - - '123456'
                  - '456789'
        onRepeat:
          minTimes: 3
          probability: 0.5

这相当于

ts

    ctx
      .intersect(app.platform('telegram'))
      .intersect(app.channel('123456', '456789'))
      .plugin(require('koishi-plugin-repeater'), {
        onRepeat: {
          minTimes: 3,
          probability: 0.5,
        },
      })

我必须承认这种写法并不是很简便，但事实上它设计出来也不是让你手写的。在控制台的「插件配置」界面我们提供了图形化的过滤器配置，你可以在那里轻松地配置每个插件的会话过滤器。这个图形化界面对插件组也同样有效。

隐藏过滤器设置 [​](#隐藏过滤器设置)
---------------------

特别地，如果你的插件不涉及任何会话，不需要设置会话过滤器，你也可以在插件中手动声明 `filter` 属性为 `false` (声明方式参考 [插件的元属性](./schema.html#插件的元属性))：

ts

    // 作为导出整体的函数插件
    export const name = 'Foo'
    export const filter = false
    export function apply(ctx: Context) {}

ts

    // 作为默认导出的类插件
    export default class Bar {
      static filter = false
      constructor(ctx: Context) {}
    }

定义条件属性 [​](#定义条件属性)
-------------------

过滤器除了可以控制插件生效的范围，还能控制具体配置项的取值。使用 `Schema.computed()` 创建一个条件属性，它可以在会话满足不同过滤器时取不同的值：

ts

    export interface Config {
      foo: Computed<number>
    }
    
    export const Config: Schema<Config> = Schema.object({
      foo: Schema.computed(Number),
    })
    
    export function apply(ctx: Context, config: Config) {
      ctx.command('foo').action(({ session }) => {
        // 在会话满足不同过滤器时取不同的值
        const value = session.resolve(config.foo)
      })
    }

---



## [https://koishi.chat/zh-CN/guide/database/](https://koishi.chat/zh-CN/guide/database/)

基本用法 [​](#基本用法)
===============

TIP

`ctx.database` 并非内置服务，因此如果你的插件需要使用数据库功能，需要[声明依赖](./../plugin/service.html#inject-属性)。

对于几乎所有大型机器人项目，数据库的使用都是不可或缺的。但如果每个插件都独立处理与数据库的交互，这将导致插件之间的兼容性非常差——用户要么选择同时安装多个数据库，要么只能放弃一些功能。为此，Koishi 设计了一整套对象关系映射 (ORM) 接口，它易于扩展并广泛地运用于各种插件中，足以应对绝大部分使用场景。

本页中涉及的完整 API：

*   [数据库操作](./../../api/database/database.html)
*   [查询表达式](./../../api/database/query.html)
*   [求值表达式](./../../api/database/evaluation.html)

`get`：查询数据 [​](#get)
--------------------

使用 `database.get()` 方法以获取特定表中的数据。下面是一个最基本的形式：

ts

    // 获取 schedule 表中 id 为 1234 的数据行，返回一个数组
    await ctx.database.get('schedule', 1234)
    
    // 获取 schedule 表中 id 为 1234 或 5678 的数据行，返回一个数组
    await ctx.database.get('schedule', [1234, 5678])

对于复杂的数据表，如果你只需要获取少数字段，你可以通过第三个参数手动指定要获取的字段：

ts

    // 返回的数组中每个元素只会包含 command, time 属性
    await ctx.database.get('schedule', [1234], ['command', 'time'])

你还可以向第二个参数传入一个对象，用来查询非主键上的数据或者同时指定多列的值：

ts

    // 获取名为 schedule 的表中 assignee 为 123456 或 456789 的数据行
    await ctx.database.get('schedule', {
      assignee: ['123456', '456789'],
    })

对于需要进行复杂的数据库搜索的，你可以使用查询表达式：

ts

    // 获取名为 schedule 的表中 id 大于 2 但是小于等于 5 的数据行
    await ctx.database.get('schedule', {
      id: { $gt: 2, $lte: 5 },
    })

为了处理更加复杂的需求，我们还引入了求值表达式。它表现为一个接受 `row` 参数的回调函数，并通过一系列 `$` 上的运算返回一个 `Boolean` 类型的值。这种写法的表达能力更强，例如你可以让多个字段共同参与运算：

ts

    import { $ } from 'koishi'
    
    // 上述两个搜索条件的或运算
    await ctx.database.get('schedule', (row) =>
      $.or(
        $.in(row.assignee, [
          '123456',
          '456789',
        ]),
        $.and(
          $.gt(row.id, 2),
          $.lte(row.id, 5),
        ),
      ),
    )

TIP

虽然求值表达式在形式上是一个回调函数，但是 Koishi 并不会将数据全部拉取到内存中，而是会将这个函数的行为编译成相对应的查询语句，提交给数据库运行。因此你可以放心地使用这种写法，它并不会带来额外的性能问题 (如果你遇到查询性能瓶颈，这更有可能是数据模型本身导致的，例如缺少必要的索引)。

`create`：插入数据 [​](#create)
--------------------------

使用 `database.create()` 方法以插入数据。

ts

    // 向 schedule 表中添加一行数据，data 是要添加的数据行
    // 返回值是添加的行的完整数据 (包括自动填充的 id 和默认属性等)
    await ctx.database.create('schedule', data)

如果你想要批量插入数据，可以使用下面介绍的 [`database.upsert()`](#upsert) 方法。

`set`：修改数据 [​](#set)
--------------------

`database.set()` 方法需要传入三个参数：表名、查询条件和要修改的数据。

ts

    // 第二个参数也可以使用上面介绍的查询表达式
    await ctx.database.set('schedule', 1234, {
      assignee: 'telegram:123456',
      time: new Date(),
    })

如果要修改的数据与已有数据相关，可以使用求值表达式：

ts

    // 让所有日期为今天的数据行的 count 字段在原有基础上增加 1
    await ctx.database.set('foo', { date: new Date() }, (row) => ({
      count: $.add(row.count, 1),
    }))

`upsert`：修改或插入数据 [​](#upsert)
-----------------------------

`database.upsert()` 的逻辑稍微有些不同，需要你传入一个数组：

ts

    // 用一个数组来对数据进行更新，你需要确保每一个元素都拥有这个数据表的主键
    // 修改时只会用每一行中出现的键进行覆盖，不会影响未定义的字段
    await ctx.database.upsert('foo', (row) => [
      { id: 1, foo: 'hello' },
      { id: 2, foo: 'world' },
      // 如果此列存在，则会按照 $.concat() 的行为进行修改
      // 如果此列不存在，row.bar 则会使用默认值
      { id: 3, bar: $.concat(row.bar, ['koishi']) },
    ])

如果初始的数据库是这样的：

id

foo

bar

(默认值)

null

bar

1

foo

baz

那么进行上述操作后的数据库将是这样的：

id

foo

bar

说明

1

hello

baz

该行已经存在，只更新了 foo 字段

2

world

bar

插入了新行，其中 foo 字段取自传入的数据，bar 字段取自默认值

3

null

barkoishi

插入了新行，其中 bar 字段取自传入的数据，foo 字段取自默认值

如果想以非主键来索引要修改的数据，可以使用第三个参数：

ts

    // 以非主键为基准对数据表进行更新，你需要确保每一个元素都拥有 telegram 属性
    await ctx.database.upsert('user', rows, 'telegram')
    
    // 以复合键为基准对数据表进行更新，你需要确保每一个元素都拥有 platform 和 id 属性
    await ctx.database.upsert('channel', rows, ['platform', 'id'])

`remove`：删除数据 [​](#remove)
--------------------------

使用 `database.remove()` 方法以删除特定表中的数据。

ts

    // 从 schedule 表中删除特定 id 的数据行
    // 第二个参数也可以使用上面介绍的查询表达式
    await ctx.database.remove('schedule', [id])

获取改动行数 [​](#write-result)
-------------------------

`set`, `upsert` 和 `remove` 操作都会返回一个 `WriteResult` 对象，它包含了这次操作的结果。你可以通过 `matched` 属性来获取匹配的数据行数 (注意不是修改的函数)，通过 `inserted` 属性来获取插入的数据行数 (仅限 `upsert` 操作)。

ts

    // 对某个用户的余额进行扣除
    const result = await ctx.database.set(
      'user',
      { id, money: { $gte: 100 } },
      (row) => ({ money: $.sub(row.money, 100) }),
    )
    // 如果用户不存在或余额不足，此时 result.matched 为 0
    if (!result.matched) {
      throw new Error('用户不存在或余额不足！')
    }

对比 set 和 upsert [​](#set-upsert)
--------------------------------

`set` 与 `upsert` 方法都可以用于修改已经存在的数据，它们的区别如下表所示：

set

upsert

作用范围

支持复杂的查询表达式

只能限定特定字段的值

插入行为

如果数据不存在则不会进行任何操作

如果数据不存在则会插入新行

对比 create 和 upsert [​](#create-upsert)
--------------------------------------

`create` 与 `upsert` 方法都可以用于插入新的数据，它们的区别如下表所示：

create

upsert

插入数量

只能插入一条数据

可以批量插入多条数据

返回值

返回经过填充后的数据

没有返回值

冲突行为

如果数据已存在则会报错

如果数据已存在则会执行修改

---



## [https://koishi.chat/zh-CN/guide/database/model.html](https://koishi.chat/zh-CN/guide/database/model.html)

数据模型 [​](#数据模型)
===============

Koishi 的架构允许任何插件对数据库的结构进行扩展。你就可以在不修改 Koishi 或其他插件源码的情况下，为数据库添加新的字段或者表。这些功能都是通过 `ctx.model` 提供的。

TIP

请注意：数据模型的扩展一定要在使用前完成，不然后续数据库操作可能会失败。

扩展表和字段 [​](#扩展表和字段)
-------------------

可以使用 `model.extend()` 方法扩展一个新的数据表，其中的第一个参数是表名，第二个参数包含了各字段的类型声明。下面的代码向数据库中扩展了一个名为 `schedule` 的表：

ts

    declare module 'koishi' {
      interface Tables {
        schedule: Schedule
      }
    }
    
    // 这里是新增表的接口类型
    export interface Schedule {
      id: number
      assignee: string
      time: Date
      interval: number
      command: string
      session: Session.Payload
    }
    
    ctx.model.extend('schedule', {
      // 各字段的类型声明
      id: 'unsigned',
      assignee: 'string',
      time: 'timestamp',
      interval: 'integer',
      command: 'text',
      session: 'json',
    })

`model.extend()` 同样也可以向已经存在的表中注入新的字段，使用方法与上面完全一致。例如，下面的代码向内置的 `User` 表中注入了 `foo` 字段：

ts

    declare module 'koishi' {
      interface User {
        foo: string
      }
    }
    
    ctx.model.extend('user', {
      // 向用户表中注入字符串字段 foo
      foo: 'string',
    })

数据类型 [​](#数据类型)
---------------

上面的数据类型均直接使用字符串来定义。对于更复杂的需求，你也可以选择传入一个对象：

ts

    ctx.model.extend('user', {
      foo: {
        type: 'string',
        // 占据的字节长度
        length: 65535,
        // 该字段的默认值
        initial: 'bar',
        // 是否允许为空
        nullable: false,
      },
    })

当你直接使用 `string` 作为类型时，其默认字节长度为 255，默认初始值为 `''`。不同字段的默认值也有所区别，你可以在 [这里](./../../api/database/model.html) 查看完整的数据类型列表。

字段迁移 [​](#字段迁移)
---------------

如果你想要修改一个已有的字段 (只修改名称，不修改逻辑)，你并不能单纯地将源码中的字段名改成新名称。如果这样做，数据仍然会停留在旧的字段中，它们实质上已经丢失了，却仍然占据的数据库的空间。此时你需要将旧的字段一并声明到表中：

ts

    ctx.model.extend('user', {
      foo: {
        type: 'string',
        legacy: ['bar', 'baz'],
      },
    })

这样一来，Koishi 就知道 `foo`, `bar`, `baz` 这三个字段实际上对应是同一列数据，并在启动时自动将旧字段中的数据迁移到 `foo` 字段中。

嵌套字段 实验性 [​](#嵌套字段)
-------------------

数据模型中的字段也可以是一个对象。有两种方式可以实现这一点：

1.  使用 `json` 类型，适用于对象内部属性不固定的情况
2.  为每个属性单独声明嵌套类型，这种做法在查询时更加高效

下面是第二种方式的声明示例：

ts

    declare module 'koishi' {
      interface User {
        foo: {
          bar: string
          baz: number
        }
      }
    }
    
    // 声明嵌套类型时，对象的多级属性被拼接为一个字符串
    ctx.model.extend('user', {
      'foo.bar': 'string',
      'foo.baz': 'integer',
    })

无论是哪一种情况，在查询时 `foo` 都会被视为一个独立的字段。

我们甚至还可以把上述两种方式相结合起来，例如指定 `foo.bar` 的类型为 `json`。

声明索引 实验性 [​](#声明索引)
-------------------

`model.extend()` 还接受一个可选的三参数，在这里你可以对表的索引进行设置：

ts

    // 注意这里配置的是第三个参数，也就是之前 autoInc 所在的参数
    ctx.model.extend('foo', {}, {
      // 主键，默认为 'id'
      // 主键将会被用于 Query 的简写形式，如果传入的是原始类型或数组则会自行理解成主键的值
      primary: 'name',
      // 自增主键值
      autoInc: true,
      // 唯一键，这应该是一个列表
      // 这个列表中的字段对应的值在创建和修改的时候都不允许与其他行重复
      unique: ['bar', 'baz'],
      // 外键，这应该是一个键值对
      foreign: {
        // 相当于约束了 foo.uid 必须是某一个 user.id
        uid: ['user', 'id'],
      },
    })

整表迁移 实验性 [​](#整表迁移)
-------------------

WARNING

整表迁移的性能较差，建议谨慎设计数据库结构而不是依赖迁移。

前面介绍的 [字段迁移](#字段迁移) 仅仅适用于修改字段名称的情况。如果你的插件需要重构表的数据结构，这种方法就不适用了。此时你可以使用 `model.migrate()` 方法来进行整表迁移：

ts

    ctx.model.extend('qux', {
      id: 'unsigned',
      text: 'string',
    })
    
    ctx.model.extend('qux2', {
      id: 'unsigned',
      flag: 'boolean',
    })
    
    // 如果 qux 中存在 flag 列，则对这部分数据进行迁移
    ctx.model.migrate('qux', {
      flag: 'boolean',
    }, async (database) => {
      const data = await database.get('qux', {}, ['id', 'flag'])
      await database.upsert('qux2', data)
    })

上面的例子展示了如何将 `qux` 表中的 `flag` 数据迁移到 `qux2` 表中。迁移完成后，`qux` 表中的 `flag` 列将会被删除，而其他列则会保留。如果你希望删除旧表，可以在回调函数的最后加上一句 `database.drop('qux')`。

---



## [https://koishi.chat/zh-CN/guide/database/selection.html](https://koishi.chat/zh-CN/guide/database/selection.html)

进阶查询技巧 [​](#进阶查询技巧)
===================

`database.get()` 已经能实现一些简单的查询了。然而在实际的开发中，我们通常会遇到排序、分组乃至聚合等更复杂的查询需求。此时就轮到更加强大的 `database.select()` 方法登场了。

基本用法 [​](#基本用法)
---------------

`database.select()` 会创建一个 `Selection` 对象。它提供了一系列的链式方法，你可以将其理解成一个查询语句的构造器。构造完成后，你可以调用 `.execute()` 方法来执行最终的查询。下面是一个简单的例子：

ts

    ctx.database.get('foo', { id: { $gt: 5 } })
    // 等价于
    ctx.database
      .select('foo')
      .where(row => $.gt(row.id, 5))
      .execute()

排序与分页 [​](#排序与分页)
-----------------

使用 `.orderBy()` 方法来对查询结果排序，使用 `.limit()` 和 `.offset()` 方法来分页：

ts

    // 按 id 降序排列，从第 100 条开始取 10 条数据
    ctx.database
      .select('foo')
      .orderBy('id', 'desc')
      .limit(10)
      .offset(100)
      .execute()

求值表达式 [​](#求值表达式)
-----------------

`.orderBy()` 和 `.where()` 等方法都支持传入一个函数，这个函数会接受一个 `row` 参数，表示当前正在处理的数据行。你可以在这个函数中返回一个值，这个值会被用于排序或筛选。

ts

    // 返回 id 大于 5 的数据行，并按 id 升序排列
    ctx.database
      .select('foo')
      .where(row => $.gt(row.id, 5))
      .orderBy(row => row.id)
      .execute()

字段映射 [​](#字段映射)
---------------

`.project()` 方法可以用于映射查询结果。它接受一个对象，对象的键表示要映射的字段名，值表示映射的表达式。下面是一个例子：

ts

    // 返回的数组元素将只含有 a, b 属性
    ctx.database
      .select('foo')
      .project({
        a: row => $.add(row.id, 1),         // a = id + 1
        b: row => $.multiply(row.id, 2),    // b = id * 2
      })
      .execute()

聚合查询 [​](#聚合查询)
---------------

`.execute()` 也可以传入一个带有聚合运算的求值函数。如果你这样做，此时返回的结果将不再是一个数组，而是该表达式计算出的值。

ts

    // 返回 id 大于 5 的数据行的数量
    ctx.database
      .select('foo')
      .where(row => $.gt(row.id, 5))
      .execute(row => $.count(row.id))

除了 `.count()` 外还有其他的一些聚合运算，例如 `$.sum()`，`$.max()` 等。聚合运算与其他求值函数的区别在于，聚合运算的外部不能再包含 `row` 的引用。

此外，只有特定方法中才能使用聚合运算，例如 `.execute()` 和 `.having()` 等。

分组查询 [​](#分组查询)
---------------

`.groupBy()` 和 `.having()` 方法可以用于分组查询。`.groupBy()` 方法接受一个字段名或求值函数，`.having()` 方法接受一个含有聚合运算并返回布尔值的表达式。下面是一个例子：

ts

    // 按照 value 字段分组，返回结果数大于 5 的分组
    ctx.database
      .select('foo')
      .groupBy('value')
      .having(row => $.gt($.count(row.id), 5))
      .execute()

`.groupBy()` 可以接受一个数组，表示同时对数组中的字段进行分组。甚至也可以是一个对象，与 `.project()` 中的用法类似。

ts

    // 返回的数据将按照 id - value 的值分组
    ctx.database
      .select('foo')
      .groupBy({
        key: row => $.subtract(row.id, row.value),
      })
      .execute()

`.having()` 中可以使用的 `row` 属性仅限于 `.groupBy()` 中的字段。

### 添加字段 [​](#添加字段)

`.groupBy()` 还额外接受一个二参数，用于在查询结果中添加聚合字段。这个参数是一个对象，同样与 `.project()` 中的用法类似。下面是一个例子：

ts

    // 返回的数据包含 value, sum, count 三个属性
    ctx.database
      .select('foo')
      .groupBy('value', {
        sum: row => $.sum(row.id),
        count: row => $.count(row.id),
      })
      .execute()

### 多级分组 [​](#多级分组)

可以通过链式调用 `.groupBy()` 方法来实现多级分组。下面是一个例子：

ts

    ctx.database
      .select('foo')
      .groupBy(['uid', 'pid'], {
        submit: row => $.sum(1),
        accept: row => $.sum(row.value),
      })
      .groupBy(['uid'], {
        submit: row => $.sum(row.submit),
        accept: row => $.sum($.if($.gt(row.accept, 0), 1, 0)),
      })
      .orderBy('uid')
      .execute()

连接查询 实验性 [​](#连接查询)
-------------------

最后介绍一下连接查询的用法。使用 `.join()` 可以将多个表连接起来，返回一个新的 `Selection`，其属性分别对应多个表的名称。下面是一个例子：

ts

    // 返回的数据包含 foo, bar 两个属性
    ctx.database
      .join(['foo', 'bar'], (foo, bar) => $.eq(foo.id, bar.id))
      .orderBy('foo.id') // orderBy 可以使用 'a.b' 的形式
      .execute()

如果你的表名比较复杂，你也可以为参与连接的各个表指定别名。将用于指定表名的数组改为传入一个对象，并修改传入函数的参数即可。下面是一个例子：

ts

    // 返回的数据包含 t1, t2 两个属性
    ctx.database
      .join({ t1: 'foo', t2: 'bar' }, row => $.eq(row.t1.id, row.t2.id))
      .orderBy('t1.id') // orderBy 可以使用 'a.b' 的形式
      .execute()

---



## [https://koishi.chat/zh-CN/guide/database/builtin.html](https://koishi.chat/zh-CN/guide/database/builtin.html)

内置数据结构 [​](#内置数据结构)
===================

通常来说，中间件、插件的设计可以让机器人的开发变得更加模块化，但是缺乏统一的数据流管理也带来了额外的问题。如果每个中间件分别从数据库中读取和更新自己所需的字段，那会造成大量重复的请求，导致严重的资源浪费；将所有可能请求的数据都在中间件的一开始就请求完成，也并不会解决问题，因为一条信息的解读可能只需要少数几个字段，而大部分都是不需要的；更严重的是，后一种做法将导致资源单次请求，多次更新，从而产生种种数据安全性问题。

针对这些问题，Koishi 提供了一套完善的数据流管理机制，它能够在保证数据安全的同时，最大化地减少数据库访问次数。在这一节中，我们将会介绍这套机制的使用方法。

观察者对象 [​](#观察者对象)
-----------------

假设我们正在开发一个抽奖插件，每调用一次 lottery 指令，用户会获得一件物品，并存入用户表的 `inventory` 属性中。下面是这个插件的实现：

ts

    declare function getLottery(): string
    
    // ---cut---
    // 定义一个 inventory 字段，用于存放物品列表
    declare module 'koishi' {
      interface User {
        inventory: string[]
      }
    }
    
    ctx.model.extend('user', {
      inventory: 'list',
    })
    
    ctx.command('lottery')
      // 声明所需字段
      .userFields(['inventory'])
      .action(({ session }) => {
        // 这里假设 inventory 是一个字符串，表示抽到的物品
        const item = getLottery()
        // 将抽到的物品存放到 user.items 中
        session.user.inventory.push(item)
        return `恭喜您获得了 ${item}！`
      })

我们都知道，写入数据库是一个异步的操作，而上面的代码看起来完全没有异步操作。然而如果你运行这段代码，你会发现用户数据被成功地更新了。这就归功于观察者机制。

`session.user` 是一个 **观察者 (Observer)** 对象，它会检测在其上面做的一切更改并缓存下来。当中间件执行完毕后，Koishi 又会自动将变化的部分进行更新，同时将缓冲区清空。我们因此得以直接在 `session.user` 上进行赋值，而不必手动调用 `ctx.database` 上的方法。

### 声明所需字段 [​](#声明所需字段)

`cmd.userFields()` 方法用于声明所需的用户字段。未声明的字段将不会被加载，也无法直接被修改。这样做的好处是，无论用户表有多少字段，我们都可以只加载所需的字段，从而提高性能。同理我们也有 `cmd.channelFields()` 方法，功能类似。

这两个方法不仅可以接受一个可迭代对象，还可以接受一个回调函数。第一个参数是当前的 `Argv` 对象，第二个参数是 `Set<keyof User>`，可以通过 add / delete 方法来添加或删除字段。因此上面的代码等价于：

ts

    cmd.userFields((argv, fields) => {
      fields.add('inventory')
    })

### 阻塞式更新 [​](#阻塞式更新)

观察者机制不仅可以将多次更新合并成一次以提高程序性能，更能解决数据竞争的问题。如果两条消息在临近的时间点被接收到，如果单纯地使用 get / set 进行处理，可能会发生后一次 get 在前一次 set 之前完成，导致本应获得 2 件物品，但实际只获得了 1 件的问题。而观察者会随时同步同源数据，数据安全得以保证。

当然，如果你确实需要阻塞式地等待数据写入，我们也提供了 `user.$update()` 方法。顺便一提，一旦成功执行了观察者的 `$update()` 方法，之前的缓冲区将会被清空，因此之后不会重复更新数据；对于缓冲区为空的观察者，`$update()` 方法也会直接返回，不会产生任何的数据库访问。这些都是我们优化的几个细节。

你可以在 [这里](./../../api/utils/observer.html) 看到完整的观察者 API。

进阶用法 [​](#进阶用法)
---------------

### attach 事件 [​](#attach-事件)

Koishi 内置了四个与观察者相关的事件，分别是：

*   `before-attach-channel`：在频道观察者被绑定到会话上之前触发
*   `attach-channel`：在频道观察者被绑定到会话上之后触发
*   `before-attach-user`：在用户观察者被绑定到会话上之前触发
*   `attach-user`：在用户观察者被绑定到会话上之后触发

下面是一个例子，我们在用户对象上实现了一个 `msgCount` 字段，用于存放收到的信息数量：

ts

    // 定义一个 msgCount 字段，用于存放收到的信息数量
    declare module 'koishi' {
      interface User {
        msgCount: number
      }
    }
    
    ctx.model.extend('user', {
      msgCount: 'integer',
    })
    
    ctx.before('attach-user', (session, fields) => {
      fields.add('msgCount')
    })
    
    ctx.middleware((session: Session<'msgCount'>, next) => {
      // 这里更新了 msgCount 数据
      session.user.msgCount++
      return next()
    })

### 手动绑定 [​](#手动绑定)

如果要绑定的字段无法提前判断，我们也提供了动态补充观察者字段的方法：

ts

    declare const fields: any[]
    
    // ---cut---
    // 绑定一个用户观察者，确保 fields 中的字段都被加载
    session.observeUser(fields)
    
    // 绑定一个频道观察者，确保 fields 中的字段都被加载
    session.observeChannel(fields)

---



## [https://koishi.chat/zh-CN/guide/database/permission.html](https://koishi.chat/zh-CN/guide/database/permission.html)

权限管理 实验性 [​](#权限管理)
===================

WARNING

权限管理目前属于实验性功能，API 可能随时会发生变化。

权限是什么？ [​](#权限是什么)
------------------

权限其实就是执行某些操作的能力。权限具有唯一的标识符，通常由小写英文字母、数字、短横线和点构成。下面是一些你可能会见到的权限名称：

*   `user:514`：ID 为 514 的用户的权限
*   `group:114`：ID 为 114 的用户组的权限
*   `authority:3`：权限等级 3 的权限
*   `command:foo`：指令 foo 的权限
*   `command:foo:option:bar`：指令 foo 选项 bar 的权限
*   `telegram:admin`：telegram 平台下群管理员的权限
*   `bot:channel.mute`：能够禁言频道的机器人的权限
*   `config:write`：能够写入配置文件的权限

权限之间存在两种关系：继承和依赖。Koishi 不区分权限与权限组的概念，权限组只是继承了其他权限的权限。你可以将用户和用户组也都视为一种权限组。

权限的继承 [​](#权限的继承)
-----------------

权限可以继承其他权限。它的基本写法如下：

ts

    ctx.permissions.inherit(A, B)

如果权限 A 继承了权限 B，那么拥有权限 A 的主体将被视为同时拥有权限 B。

例：ID 为 514 的用户拥有权限等级 3，指令 foo 所需要的权限等级是 2。这种情况下该用户显然应该可以调用该指令。那么这种调用关系具体是如何体现的呢？

text

    user:514 > authority:3 > authority:2 > command:foo

这里出现了三个继承关系：

*   `user:114 > authority:3`，因为 ID 为 514 的用户拥有权限等级 3
*   `authority:3 > authority:2`，因为权限等级 3 天生比权限等级 2 大（内置逻辑）
*   `authority:2 > command:foo`，因为指令 foo 被权限等级 2 继承

由此，权限的继承关系能够顺利表达已有的权限等级机制，并且具备更强的表达能力。

### 权限的多继承 [​](#权限的多继承)

权限继承除了不能循环外，几乎没有任何限制。因此，任何一个权限既可以被多个权限继承，也可以继承多个权限。下面分别展示一些使用例。

例：ID 为 514 的用户同时继承了权限等级 1，而指令 foo 所需权限等级 2，此时该用户并不能调用 foo 指令。但如果现在我们让该用户直接继承 foo 指令的调用权限，会发生什么呢？

text

    user:514 > authority:1
             > command:foo

在这张图中，`user:514` 并不能经由 `authority:1` 到达 `command:foo`，但是添加第二条边后又可以直接到达 `command:foo` 了。因此该用户此时就又可以调用 foo 指令了。

可以看到，权限的继承为我们提供了一种能力，可以允许特定低等级用户去调用高级权限的指令，这种能力是过去的权限等级所不具有的。

例：我们希望某个管理型指令 foo 既可以被权限等级 2 的用户调用，又可以被 QQ 群的管理员调用。此时我们可以对 foo 指令进行以下配置：

text

    authority:2  >
    telegram:admin > command:foo

这样一来，一个用户只需满足上述两个条件之一就可以调用此指令了。

可以看到，判断指令是否可以被用户调用，本质上是判断用户自身的权限是否可以顺着权限继承的关系到达指令的权限。同时，权限的继承允许我们给指令的调用设置多个不同条件。

权限的依赖 [​](#权限的依赖)
-----------------

Koishi 中的权限不仅存在继承关系，还存在依赖关系。它的基本写法如下：

ts

    ctx.permissions.depend(A, B)

如果权限 A 依赖了权限 B，那么要执行权限 A 的操作时必须同时检查权限 B。

例：foo 指令的代码中调用了 bar 指令，因此 foo 指令依赖 bar 指令。

text

    command:foo -> command:bar

如果用户只拥有 foo 的权限，没有调用 bar 的权限，他依然无法调用 foo 指令。

例：foo 指令的代码中使用了 `bot.muteChannel()`。

text

    command:foo -> bot:channel.mute

如果机器人没有实现此 API，用户就无法在该机器人上调用 foo 指令。

由此可见，权限的依赖与继承不同。继承更多的是一种管理上的考虑，而依赖则关乎具体的功能实现。

权限访问器 [​](#权限访问器)
-----------------

在上面的介绍中，如果要定义新的权限，就必须手动分配给用户或用户组后才能使用。有没有方法自动为一个会话分配权限呢？这就是权限访问器的功能。

ts

    ctx.permissions.provide('telegram:admin', async (name, session) => {
      return session.telegram?.sender?.role === 'admin'
    })

上面的代码的作用是：当某个会话处于 telegram 平台，并且发送者是群内管理员时，自动附加一个 `telegram:admin` 权限。利用这种技术，我们就可以为特定平台提供权限能力了。

每个权限可以定义多个访问器函数。在运行时必须通过每一个访问器函数的检查才能视为拥有权限。

一个权限要么是普通权限，要么是访问器权限。下面是一些区别：

普通权限

访问器权限

手动分配给用户 (组)

自动分配给会话

可以被其他权限继承

不能被其他权限继承

权限国际化 [​](#权限国际化)
-----------------

普通权限要被用于指令和控制台中显示，因此需要做国际化。具体的做法也很简单：

*   通过 API 定义：使用 `permission.{name}` 提供翻译文本
*   通过指令定义：定义时提供文本 (自动视为当前用户语言)，或通过 `--locale` 指定特定语言的文本
*   通过控制台定义：可以在控制台「用户管理」界面中配置用户组文本

访问器权限由于其不能被其他权限继承，因此不需要做国际化。

---



## [https://koishi.chat/zh-CN/guide/adapter/index.html](https://koishi.chat/zh-CN/guide/adapter/index.html)

基础知识 [​](#基础知识)
===============

Koishi 通过适配器插件来实现对不同聊天平台的支持。

一方面，适配器插件需要接收来自聊天平台的消息，并将其转换为 Koishi 的标准格式并触发会话事件；另一方面，对于来自 Koishi 内部的请求，适配器也需要将其转换为聊天平台的格式并发送出去。我们可以简单地将这两个过程概括成「接收」和「发送」。

在 Koishi 中，尽管适配器要处理的逻辑随着平台的不同而变化，但本质上所有适配器的结构都是类似的：通过实现 `Bot` 类完成发送的功能，而通过实现 `Adapter` 类完成接收的功能。我们先介绍一些与跨平台相关的核心概念，随后将给出一个最简单的适配器插件示例。

核心概念 [​](#核心概念)
---------------

在我们开始之前，先来了解一些与跨平台相关的核心概念。

**平台 (Platform)** 是指聊天平台，比如 Discord、Telegram 等。同一平台内的用户间具有相互发送消息的能力，而不同平台的用户间则没有。对于 Rocket Chat 这一类可自建的聊天平台而言，每个独立的自建服务器都视为不同的平台。

**机器人 (Bot)** 是指由 Koishi 操控的平台用户。这里的用户可以是真实用户，也可以是部分平台专门提供的机器人用户。其他用户通过与机器人进行交互来体验 Koishi 的各项功能。

**适配器 (Adapter)** 是指实现了平台协议，能够让机器人接入平台的插件。通常来说一个适配器实例对应了一个机器人用户，同时启用多个适配器就实现了多个机器人的同时接入。

**消息 (Message)** 是字面意义上的消息。通常是文本或富文本格式的，有时也会包含图片、语音等媒体资源。在 Koishi 中，消息通过消息元素进行统一编码。

**频道 (Channel)** 是消息的集合。一个频道包含了具备时间、逻辑顺序的一系列消息。频道又分为私聊频道和群聊频道，其中私聊频道有且仅有两人参与，而群聊频道可以有任意多人参与。

**群组 (Guild)** 是平台用户的集合。一个群组通常会同时包含一组用户和频道，并通过权限机制让其中的部分用户进行管理。在部分平台中，群组和群聊频道的概念恰好是重合的 (例如 QQ)：一个群组内有且仅有一个群聊频道。私聊频道不属于任何群组。

REPL 适配器 [​](#repl-适配器)
-----------------------

下面展示的插件是 REPL 适配器，它可以接收来自命令行的消息，并把 Koishi 的回复同样输出到命令行中。你可以在 [这个仓库](https://github.com/koishijs/koishi-plugin-adapter-repl) 查看它的源码。

> REPL 的意思是 Read-Eval-Print-Loop (读取-求值-输出-循环)，是一种交互式环境。

REPL 适配器有三个文件。首先来看入口文件 `index.ts`，它什么事都没做：

index.ts

    import ReplBot from './bot'
    export default ReplBot

接下来是 `bot.ts`。我们可以看到它实现了 `sendMessage` 方法，用来发送消息：

bot.ts

    import { Bot, Context, h, Schema } from 'koishi'
    import { EOL } from 'os'
    import ReplAdapter from './adapter'
    
    export interface Config {}
    export const Config: Schema<Config> = Schema.object({})
    
    export default class ReplBot extends Bot {
      constructor(ctx: Context, config: Config) {
        super(ctx, config)
        this.platform = 'repl'
        this.selfId = 'koishi'
        ctx.plugin(ReplAdapter, this)
      }
    
      async createMessage(channelId: string, content: h.Fragment) {
        process.stdout.write(h('', content).toString(true))
        process.stdout.write(EOL)
        return []
      }
    }

最后是 `adapter.ts`，它创建了一个 [readline](https://nodejs.org/dist/latest-v20.x/docs/api/readline.html) 接口，用于接收消息并生成会话：

adapter.ts

    import { Adapter, Context } from 'koishi'
    import { createInterface } from 'readline'
    import ReplBot from './bot'
    
    export default class ReplAdapter extends Adapter<ReplBot> {
      rl = createInterface({
        input: process.stdin,
      })
    
      async start(bot: ReplBot) {
        bot.online()
        this.rl.on('line', (line) => {
          const session = bot.session()
          session.type = 'message'
          session.userId = 'repl'
          session.channelId = 'repl'
          session.isDirect = true
          session.content = line
          bot.dispatch(session)
        })
      }
    
      async stop(bot: ReplBot) {
        this.rl.close()
      }
    }

真实的聊天平台当然会比命令行交互复杂得多，但你仍然可以使用相同的结构来实现它们。在接下来的几节中，我们会进一步介绍适配器插件的更多设计细节。

TIP

等下，上面的代码的确实现了一个适配器，但它是一个插件吗？

答案是肯定的。这个插件的入口文件默认导出了 `ReplBot`。而 `ReplBot` 的构造函数接受两个参数 `ctx` 和 `config`，这与插件的 [类形式](./../plugin/) 是一致的。这意味着，一个 `ReplBot` 类本身就是一个可以安装的插件！

与此同时，`Bot` 基类中也声明了它是一个 [可重用](./../plugin/lifecycle.html#可重用插件) 的插件，因此多次加载此插件将会创建多个独立的 `ReplBot` 实例。适配器插件是最常见的可重用插件。

---



## [https://koishi.chat/zh-CN/guide/adapter/bot.html](https://koishi.chat/zh-CN/guide/adapter/bot.html)

实现机器人 [​](#实现机器人)
=================

`Bot` 对应着由 Koishi 操纵的聊天平台机器人账号。其上封装了一系列方法，用于发送消息、获取频道信息等操作。要实现一个聊天平台的 `Bot` 类，只需要实现这些方法即可。

通用接口 [​](#universal)
--------------------

让我们先回忆一下上一节介绍的 `ReplBot`：

ts

    class ReplBot<C extends Context> extends Bot<C> {
      constructor(ctx: C, config: Config) {
        super(ctx, config)
        this.platform = 'repl'
        this.selfId = 'koishi'
        ctx.plugin(ReplAdapter, this)
      }
    
      async createMessage(channelId: string, content: h.Fragment) {
        process.stdout.write(h('', content).toString(true))
        process.stdout.write(EOL)
        return []
      }
    }

这里仅仅实现了 `createMessage` 一个方法，而真正的聊天平台往往具备更多通用能力，例如获取群组、频道、用户信息，添加表态，管理群组成员以及处理邀请等等。

Koishi 提供了一套通用的 [机器人接口](./../../api/core/bot.html)。适配器应当尽可能地实现这些标准方法，但这并不是必需的。对于平台没有提供能力的 API，可以直接略去实现。

访问内部接口 [​](#internal-access)
----------------------------

尽管上面的通用接口足以应对大多数插件的需求，但这并不能将平台的能力发挥到极致。为此，Koishi 也允许 `Bot` 提供一套内部接口，用于直接调用平台的原生能力。

TIP

**为什么不能直接在 `Bot` 类上添加方法？**

首先，插件并不能确定所拿到的 `Bot` 对象来自哪一个适配器，就算想要用上原生能力也必须强行做类型转换 (你稍后就能看到内部接口是如何解决类型问题的)；其次，原生接口可能与通用接口有相同的名称，随着 Koishi 未来进一步扩展通用接口，会有很大可能性引发接口冲突。

### 在插件中访问 [​](#access-from-plugin)

在插件中访问内部接口有两种方法。我们以 Discord 平台为例展示。

第一种是直接通过 `bot.internal` 属性访问。这个属性在 `Bot` 基类中的类型是 `any`，因此你可以直接使用其上的方法，也可以通过类型断言来获取更好的类型提示：

ts

    // 这一行写在文件头
    import type { DiscordBot } from '@koishijs/plugin-adapter-discord'
    
    (bot as DiscordBot).internal.getGuild(guildId)

另一种方法是在有 `Session` 对象的环境中，直接通过 `session[platform]` 就可以访问到对应适配器的内部接口。这种方式不仅无需类型断言，并且能够直接访问到会话的原始数据。你可以用这种方式对特定平台提供定制化的支持：

ts

    // 这一行写在文件头
    import {} from '@koishijs/plugin-adapter-discord'
    
    if (session.discord) {
      session.discord.getGuild(guildId)     // 内部接口
      session.discord.t                     // 原始事件名称
      session.discord.d                     // 原始事件数据
    } else {
      // 其他平台的处理
    }

TIP

在上面的例子中，我们仅仅从 @koishijs/plugin-adapter-discord 中导入了类型。这种情况下插件并不实际依赖 Discord 适配器，因此你只需要将该依赖写入 `devDependencies` 即可。对于尚未接入 Discord 平台的用户，也不需要为运行你的插件多装一个适配器，仍然确保了安装体积的精简。关于这部分的讨论，可以参考 [服务与依赖](./../plugin/service.html#peer-vs-dep) 一节。

### 在适配器中访问 [​](#access-from-adapter)

内部接口不仅能为插件提供更全面的平台能力，对适配器本身的实现也有很大的帮助。让我们截取 Discord 适配器的一段代码作为示例：

ts

    class Internal {
      // 这里的实现先略去
    }
    
    // 将 Discord 的数据结构转换为通用数据结构
    const decodeGuild = (data: Discord.Guild): Universal.Guild => ({
      guildId: data.id,
      guildName: data.name,
    })
    
    class DiscordBot<C extends Context> extends Bot<C> {
      constructor(ctx: C, config: Config) {
        super(ctx, config)
        this.internal = new Internal()
        ctx.plugin(DiscordAdapter, this)
      }
    
      // 获取群组数据
      async getGuild(guildId: string) {
        const data = await this.internal.getGuild(guildId)
        return decodeGuild(data)
      }
    
      // 获取群组列表
      async getGuildList() {
        const data = await this.internal.getCurrentUserGuilds()
        return { data: data.map(decodeGuild) }
      }
    }

在上面这段代码中，Discord 平台与 Koishi 都定义了一个 `Guild` 接口。前者包含了更多信息，但由于它们的关键字段不完全相同，因此并不能直接把请求的结果作为通用方法的返回值。

为此，我们实现了一个 `decodeGuild` 函数，将 Discord 的数据结构转换为 Koishi 的通用数据结构。与此同时，我们把网络请求的部分放在 `Internal` 类中实现，并在 `Bot` 类中直接调用内部方法。可以看到，这样编写出来的代码结构相比直接把请求放在 `Bot` 类中要清晰得多。

实现内部接口 [​](#internal-impl)
--------------------------

不同的平台由于其 API 的差异性，`Internal` 类的实现方式也会有所不同。对于简单的平台，你完全可以手动实现每一个内部接口 (甚至可以不实现 `Internal` 类，就像 REPL 适配器那样)；但如果平台本身就有上百个 API，手写每一个内部接口显然既费时又啰嗦。因此，Koishi 提供了一些技巧以简化你的适配工作。我们这里仍然以 Discord 为例。

### 使用 HTTP 服务 [​](#http-service)

让我们进一步完成上面的代码。Discord 的 API 是 Restful 的，并且需要 `Authorization` 请求头。我们通过在 `Internal` 类中传入一个 `http` 对象简化网络请求的写法：

ts

    class Internal {
      constructor(private http: HTTP) {}
    
      getGuild(guildId: string) {
        return this.http.get(`/guilds/${guildId}`)
      }
    
      getCurrentUserGuilds() {
        return this.http.get('/users/@me/guilds')
      }
    }
    
    class DiscordBot<C extends Context> extends Bot<C> {
      constructor(ctx: C, config: Config) {
        super(ctx, config)
        const http = ctx.http.extend({
          endpoint: 'https://discord.com/api/v10',
          headers: {
            Authorization: `Bot ${config.token}`,
          },
        })
        this.internal = new Internal(http)
      }
    }

[`ctx.http`](./../../api/service/http.html) 是 Koishi 的基础服务，其上封装了一套基于 [fetch](https://developer.mozilla.org/zh-CN/docs/Web/API/Fetch_API) 的网络请求 API。这里，我们使用 `ctx.http.extend()` 方法创建了一个新的 `HTTP` 实例，其上的请求会继承传入的配置。这样我们就无需每次请求都写一遍请求头了。

### 反射网络请求 [​](#reflect)

在 `HTTP` 的帮助下，我们甚至可以直接对网络请求进行反射，从而自动生成内部接口。

ts

    class Internal {
      constructor(private http: HTTP) {}
    
      static define(path: string, methods: Partial<Record<HTTP.Method, string | string[]>>) {
        for (const key in methods) {
          const method = key as HTTP.Method
          for (const name of makeArray(methods[method])) {
            this.prototype[name] = async function (this: Internal, ...args: any[]) {
              // 将参数填入路径中
              const url = path.replace(/\{([^}]+)\}/g, () => {
                if (!args.length) throw new TypeError('missing arguments')
                return args.shift()
              })
              return this.http(method, url)
            }
          }
        }
      }
    }

有了这个 `Internal.define()` 方法，我们就可以批量定义内部接口了：

ts

    Internal.define('/guilds/{guild.id}', {
      GET: 'getGuild',
      PATCH: 'modifyGuild',
      DELETE: 'deleteGuild',
    })
    
    Internal.define('/users/@me/guilds', {
      GET: 'getCurrentUserGuilds',
    })

最后别忘了通过类型合并的方式，将这些方法添加到 `Internal` 类型上：

ts

    interface Internal {
      getGuild(guildId: string): Promise<Discord.Guild>
      modifyGuild(guildId: string, data: Discord.PartialGuild): Promise<Discord.Guild>
      deleteGuild(guildId: string): Promise<void>
      getCurrentUserGuilds(): Promise<Discord.Guild[]>
    }

上面的代码还没有考虑请求体和异常处理等问题，如果想要深入了解，可以阅读 Discord 适配器的 [源码](https://github.com/satorijs/satori/blob/master/adapters/discord/src/types/internal.ts)。事实上，Discord 的接口已经是比较复杂的了。相信有了这些技巧的加持，其他平台的适配器你一定也能手到擒来。

### 注入会话属性 [​](#session-injection)

在本节的最后，我们还有一点伏笔没有回收。我们还需要在 `Session` 对象中注入 `discord` 属性，以便插件能够访问到内部接口：

ts

    declare module 'koishi' {
      interface Session {
        discord?: Internal & Payload
      }
    }

这里的 `Internal` 对应着内部接口，而 `Payload` 则对应着原始事件数据。当构造会话对象时 (将在下一节具体介绍)，我们需要将这些数据注入到 `Session` 对象中：

ts

    session.setInternal('discord', payload)

---



## [https://koishi.chat/zh-CN/guide/adapter/adapter.html](https://koishi.chat/zh-CN/guide/adapter/adapter.html)

实现适配器 [​](#实现适配器)
=================

我们已经知道，单独一个 `Bot` 类已经构成一个合法的插件了。不过，这样的插件只具备调用平台 API 的能力，还无法接收消息。这个时候就需要 `Adapter` 类出场了。

适配器的类型 [​](#types)
------------------

适配器需要建立并维护机器人与聊天平台之间的连接。通常来说，根据协议的不同，适配器与机器人可能是一对一的，也可能是一对多的。让我们再看一眼之前介绍过的 `ReplBot` 实例：

ts

    class ReplBot<C extends Context> extends Bot<C> {
      constructor(ctx: C, config: Config) {
        super(ctx, config)
        this.platform = 'repl'
        this.selfId = 'koishi'
        ctx.plugin(ReplAdapter, this)
      }
    }

如果我们多次加载上述插件，由于 `Bot` 基类的可重用性，每一次加载都会构造出新的 `ReplBot` 实例。另一方面，`ReplAdapter` 类继承了 `Adapter`，并且没有声明 `reusable` 属性，因此是一个不可重用插件。在多次加载的过程中，多个 `ReplBot` 实例会对应于同一个 `ReplAdapter` 实例。这便是典型的一对多适配器逻辑。

相比之下，Discord 平台使用 WebSocket 向机器人推送事件。每一个机器人都需要维护一个独立的 WebSocket 连接，因此需要多个 `Adapter` 实例。在这种情况下，我们无需改动上面机器人的代码，只需要将 `DiscordAdapter` 继承的基类变为 `Adapter.WsClient`。这个基类声明了可重用性，它将实现一个一对一的适配器逻辑。

简单来说就是，在实现适配器时，首先需要协议的类型确定适配器与机器人的对应关系。如果是一对一的，就需要声明 `reusable` 属性，否则不需要声明。此外，对于部分典型场景，我们又进一步派生出了 `Adapter.WsClient` 等子类，方便你快速实现适配器。

典型实现 [​](#typical-impls)
------------------------

下面让我们看几种典型的适配器实现。

### WebSocket [​](#websocket)

一种常见的通信方式是 WebSocket，许多平台 (Discord、KOOK、钉钉等) 都会使用这项技术。它的工作原理是，机器人首先向聊天平台的 WebSocket 网关发起连接请求，随后平台会将事件推送到机器人的 WebSocket 连接上。这里我们还是以 Discord 平台为例：

ts

    export class DiscordAdapter<C extends Context> extends Adapter.WsClient<C, DiscordBot<C>> {
      async prepare() {
        const { url } = await this.bot.internal.getGatewayBot()
        return this.bot.http.ws(url + '/?v=10&encoding=json')
      }
    
      accept() {
        this.socket.addEventListener('message', async ({ data }) => {
          const parsed = JSON.parse(data.toString())
          if (parsed.t === 'READY') {
            const user = decodeUser(parsed.d.user)
            Object.assign(this.bot, user)
            return this.bot.online()
          } else {
            const session = createSession(this.bot, parsed)
            if (session) this.dispatch(session)
          }
        })
      }
    }

一个 `WsClient` 类需要实现 `prepare()` 和 `accept()` 两个方法。`prepare()` 方法应当返回一个 `WebSocket` 对象，用于与聊天平台建立连接。在上面的例子中，我们首先通过内部 API 获取了 WebSocket 网关地址，然后使用 `bot.http.ws()` 方法创建了一个 `WebSocket` 对象：

ts

    const { url } = await this.bot.internal.getGatewayBot()
    return this.bot.http.ws(url + '/?v=10&encoding=json')

`accept()` 方法用于处理已经成功连接的 `WebSocket` 对象。具体而言应当包含三件事：

1.  在初始化机器人各项属性后，调用 `bot.online()` 方法，将机器人标记为在线状态
2.  接收来自聊天平台的事件，构造 `Session` 对象并初始化各项属性，随后调用 `dispatch()` 方法将其触发为会话事件
3.  根据聊天平台的协议要求，处理心跳、重连、错误等情况 (如果平台没有专门设置与重连相关的信令，可以不用实现，`WsClient` 基类已经内置了简单的重连逻辑)

在上面的例子中，`READY` 事件表示机器人已经成功连接，此时我们对机器人进行初始化：

ts

    const user = decodeUser(parsed.d.user)
    Object.assign(this.bot, user)
    return this.bot.online()

在我们调用 `bot.online()` 之前，应当尽量保证 `Bot` 实例有 `selfId`, `username` 和 `avatar` 属性。前者本身就是必须属性，而后两个属性则会显示在控制台的机器人状态栏中。

对于其他事件，我们都尝试创建一个 `Session` 对象，并将它触发为会话事件：

ts

    const session = createSession(this.bot, parsed)
    if (session) this.dispatch(session)

`createSession()` 会根据事件的类型，创建不同的 `Session` 实例。如果无法对应到标准的会话事件，那么 `createSession()` 方法会返回空值，表示我们不需要调用 `dispatch()` 方法。

### Webhook [​](#webhook)

另一种常见的通信方式是 Webhook，使用这种通信方式的平台有飞书、企业微信、Line 等。它的工作原理是，机器人搭建者首先在聊天平台的开发者后台配置一个 HTTP 服务器地址，随后平台会将事件推送到该地址上。这里我们以 Line 平台为例：

ts

    export class HttpServer<C extends Context> extends Adapter<C, LineBot<C>> {
      static inject = ['server']
    
      constructor(public ctx: C) {
        super()
    
        ctx.server.post('/line', async (ctx) => {
          const { destination, events } = ctx.request.body
          const bot = this.bots.find(bot => bot.selfId === destination)
          if (!bot) return ctx.status = 403
    
          for (const event of events) {
            const session = createSession(bot, event)
            if (session) bot.dispatch(session)
          }
          ctx.status = 200
          ctx.body = 'ok'
        })
      }
    
      async start(bot: LineBot) {
        await this.getLogin()
        await bot.internal.setWebhookEndpoint({
          endpoint: this.ctx.server.config.selfUrl + '/line',
        })
      }
    }

任何一个适配器都需要通过 `start()` 和 `stop()` 方法来控制机器人的启动和停止 (你在前一个例子中没有看到这两个方法，只是因为 `WsClient` 已经内置了实现)。在这个例子中，我们通过内部接口对机器人数据做了初始化，并设置了 Webhook 回调地址：

ts

    await this.getLogin()
    await bot.internal.setWebhookEndpoint({
      endpoint: this.ctx.server.config.selfUrl + '/line',
    })

对于 HTTP 服务器来说，我们不仅需要维护机器人的状态，还需要创建一个 HTTP 服务器，用于接收来自聊天平台的事件。因此，我们在构造函数中使用 `ctx.server` 监听了 Webhook 回调地址。对于每一个接收到的请求，我们首先验证其是否对应于已经配置的机器人：

ts

    const sign = ctx.headers['x-line-signature']?.toString()
    const parsed = ctx.request.body as WebhookRequestBody
    const bot = this.bots.find(bot => bot.selfId === parsed.destination)
    if (!bot) return ctx.status = 403

验证完成后，对于请求中的每一个事件，我们创建 `Session` 对象，并将它触发为会话事件：

ts

    for (const event of parsed.events) {
      const session = createSession(bot, event)
      if (session) bot.dispatch(session)
    }

### 其他通信方式 [​](#others)

除了 WebSocket 和 Webhook 以外，还有一些其他可能出现的通信方式：

*   WS 服务器：机器人建立 WebSocket 服务器，持续接收来自聊天平台的事件
*   HTTP 轮询：机器人定时向聊天平台发起 HTTP 请求，获取新增的事件列表

当然，对于那些不太像聊天平台的聊天平台，你也可以不必拘泥于传统的通信方式。直接继承 `Adapter` 基类，实现自己的逻辑即可。无论是我们在本章开始介绍的命令行环境，又或者是邮件、短信，甚至是社交媒体的评论区、私信，只要是能打字的地方，都可以通过适配器的方式接入到 Koishi 中！

进阶技巧 [​](#advanced)
-------------------

接下来我们将介绍一些复杂适配器的实现技巧。

### 多协议支持 [​](#multi-protocol)

部分平台同时支持了多种通信方式，例如 Telegram 就同时支持了 Webhook 和 HTTP 轮询。对于此类平台，我们可以提供一个配置项，让用户根据需要自行选择通信方式。

首先调整目录结构，在 `server.ts` 和 `polling.ts` 中分别完成两种通信方式的适配器开发：

text

    adapter-telegram
    ├── src
    │   ├── bot.ts
    │   ├── index.ts
    │   ├── adapter.ts
    │   ├── polling.ts
    │   └── server.ts
    └── package.json

每一种适配器可能都有自己的配置项，我们按照类插件的开发方式分别进行声明：

server.ts

    class ServerAdapter<C extends Context> extends Adapter<C, TelegramBot<C>> {}
    
    namespace ServerAdapter {
      export interface Options {
        protocol: 'server'
        path?: string
      }
    
      export const Options: Schema<Options> = Schema.object({
        protocol: Schema.const('server').required(),
        path: Schema.string().default('/telegram'),
      })
    }

polling.ts

    class PollingAdapter<C extends Context> extends Adapter<C, TelegramBot<C>> {
      // polling 适配器是可重用的
      static reusable = true
    }
    
    namespace PollingAdapter {
      export interface Options {
        protocol: 'polling'
        timeout?: string
      }
    
      export const Options: Schema<Options> = Schema.object({
        protocol: Schema.const('server').required(),
        timeout: Schema.number().default(Time.second * 25),
      })
    }

最后编写作为入口的 `TelegramBot` 类，它将根据配置项的 `protocol` 属性，自动选择相关联的适配器 (最后配置项的定义使用了 [配置联动](./../../schema/advanced/union-tagged-2.html) 技巧)：

ts

    class TelegramBot<C extends Context> extends Bot<C, TelegramBot.Config> {
      constructor(ctx: C, config: TelegramBot.Config) {
        super(ctx, config)
        if (config.protocol === 'server') {
          ctx.plugin(HttpServer, this)
        } else if (config.protocol === 'polling') {
          ctx.plugin(HttpPolling, this)
        }
      }
    }
    
    namespace TelegramBot {
      export type Config = ServerAdapter.Options | PollingAdapter.Options
    
      export const Config: Schema<Config> = Schema.intersect([
        Schema.object({
          protocol: Schema.union(['server', 'polling']).required(),
        }),
        Schema.union([
          HttpServer.Options,
          HttpPolling.Options,
        ]),
      ])
    }

### 动态创建机器人 [​](#dynamic)

到此为止，我们的适配器开发中都存在一个隐含限制：用户的一次插件加载只能对应于一个 `Bot` 实例。如果用户需要创建多个机器人，那么就需要多次加载插件。这是因为在绝大多数适配器的使用场景下，用户都能很明确地知道自己需要创建多少个机器人。然而总有一些例外情况：

*   WhatsApp 平台的一个应用可以填入多个手机号，也就对应了多个 `Bot` 实例。
*   Satori 协议并不预先知道机器人的数量，而是在连接中根据机器人相关事件动态创建的。

WARNING

无限制的 `Bot` 连接可能会导致你的 Koishi 被恶意调用。因此，如果将适配器作为可任意连接的服务端，请确保在可信任的网络环境下运行，或者引入其他验证机制。

在上述的情况下，我们需要对插件的写法做一些调整。`Bot` 类不再能作为插件的入口了，但我们可以直接使用 `Adapter` 类作为入口。这里以 WhatsApp 平台为例：

index.ts

    import WhatsAppAdapter from './adapter'
    export default WhatsAppAdapter

同时，适配器也直接继承 `Adapter` 基类，并声明 `schema` 和 `reusable`：

adapter.ts

    class WhatsAppAdapter<C extends Context> extends Adapter<C, WhatsAppBot<C>> {
      // 由适配器直接向外暴露配置项
      static schema = true
      // 这个适配器仍然是可重用的
      static reusable = true
    
      constructor(ctx: C, config: WhatsAppAdapter.Config) {
        super()
    
        // 初始化内部接口
        const http = ctx.http.extend({
          headers: { Authorization: `Bearer ${config.token}` },
        })
        const internal = new Internal(http)
    
        // 启动时创建机器人
        ctx.on('ready', async () => {
          const data = await internal.getPhoneNumbers()
          for (const item of data) {
            const bot = new WhatsAppBot(ctx, {
              phoneNumber: item.id,
            })
            bot.adapter = this
            bot.internal = internal
            this.bots.push(bot)
          }
        })
      }
    }

---



## [https://koishi.chat/zh-CN/guide/adapter/message.html](https://koishi.chat/zh-CN/guide/adapter/message.html)

消息编码 [​](#消息编码)
===============

在 [实现机器人](./bot.html#在适配器中访问) 一节中，我们其实已经涉及了格式转换的概念：

ts

    // 将 Discord 的数据结构转换为通用数据结构
    const decodeGuild = (data: Discord.Guild): Universal.Guild => ({
      guildId: data.id,
      guildName: data.name,
    })
    
    // 将通用数据结构转换为 Discord 的数据结构
    const encodeGuild = (data: Universal.Guild): Discord.Guild => ({
      id: data.guildId,
      name: data.guildName,
    })

不同平台对于同一个概念的接口会存在或多或少的差异。为了抹平这些差异，Koishi 引入了一套通用接口，用来描述这些跨平台的概念。在实现机器人和适配器时，通常都需要编写如上的函数，来对具体平台的数据进行转化。而这其中最复杂的则是对消息的处理。

Koishi 使用 [消息元素](./../basic/element.html) 表达任何聊天平台的消息。这是一种类似于 HTML 的格式。消息元素作为组成消息的基本单位，可以表示具有特定语义的内容，如文本、表情、图片、引用、元信息等。本节将介绍如何在消息元素与平台消息之间互相转换。

接收消息 [​](#receive)
------------------

在会话对象上存在两个属性与消息的内容有关：`content` 和 `elements`，它们分别对应着字符串形式和消息元素形式的消息内容。它们之间会自动转换，因此下面的两种写法是等价的：

ts

    session.content = '欢迎 <at id="1234567"/>'

ts

    session.elements = [
      h('text', { content: '欢迎 ' }),
      h('at', { id: '1234567' }),
    ]

在接收消息时，只需根据平台的格式对消息进行解码，将结果赋值到上述两个属性之一即可。下面是一个最简单的例子，假设平台的消息均以文本形式接收，并且使用 `@id` 的语法表达提及用户，那么你可以这么写：

ts

    session.content = input.replace(/@(\d+)/g, '<at id="$1"/>')

发送消息 [​](#send)
---------------

### 兼容性原则 [​](#compatibility)

在具体介绍消息发送之前，不知道你是否有这样的疑问：Koishi 提供了一整套标准的消息元素，但并非所有平台都支持这些元素。对于那些不支持的元素，应该如何处理呢？

Koishi 的建议是**尽量兼容实现**。对于平台不支持的元素，可以根据元素的类型和用户的配置进行转化与回退。大致可以分为两种情况：

*   修饰型的元素可以选择只渲染内部的元素，或以适当的方式进行文本修饰。  
    例如：在不支持粗体的平台上渲染 `<b>` 时，可以改为只渲染粗体的内容。  
    例如：在不支持列表的平台上渲染 `<ul>` 时，可以在每个列表项前面渲染一个 `-`。
    
*   占位型的元素尽量转换为可渲染的元素；如果实在无法渲染则抛出错误。  
    例如：如果平台不支持发送网络图片，可以先将图片下载到本地再发送。  
    例如：如果平台不支持发送语音，可以改为发送文件，或抛出错误。
    

对于更加复杂的元素，适配器也可以发挥自主性，设计最适合的交互形式。例如，如果用户的需求是「从若干个选项中选择一个」，那么平台 A 可以渲染出多个按钮供用户点击；平台 B 则可以发送一条带有表态的消息，点击表态对应选择选项；实在不行，平台 C 也可以直接发送选项列表和文本提示语，并将用户的下一次输入作为选项。

### 消息编码器 [​](#encoder)

之前介绍过的 REPL 适配器为了简化写法，并未包含消息的编码过程。对于一般的适配器，我们建议通过继承 `MessageEncoder` 类来实现消息的发送逻辑。

这里我们以 Telegram 平台为例，首先在源码目录下创建 `message.ts`：

text

    adapter-example
    ├── src
    │   ├── adapter.ts
    │   ├── bot.ts
    │   ├── index.ts
    │   └── message.ts
    └── package.json

在这个文件中我们定义 `TelegramMessageEncoder`：

message.ts

    class TelegramMessageEncoder<C extends Context> extends MessageEncoder<C, TelegramBot<C>> {
      // 使用 payload 存储待发送的消息
      private payload: Dict
    
      // 在 prepare 中初始化 payload
      async prepare() {
        this.payload = { chat_id: this.channelId, parse_mode: 'html', text: '' }
      }
    
      // 将发送好的消息添加到 results 中
      async addResult(data: Telegram.Message) {
        const message = decodeMessage(data)
        this.results.push(message)
        const session = this.bot.session()
        session.event.message = message
        session.app.emit(session, 'send', session)
      }
    
      // 发送缓冲区内的消息
      async flush() {
        let message: Telegram.Message
        if (this.payload.text) {
          message = await this.bot.internal.sendMessage(this.payload)
        }
        await this.addResult(message)
        this.payload.text = ''
      }
    
      // 遍历消息元素
      async visit(element: h) {
        const { type, attrs, children } = element
        if (type === 'text') {
          this.payload.text += h.escape(attrs.content)
        } else {
          await this.render(children)
        }
      }
    }

一个 `MessageEncoder` 类需要提供 `flush` 和 `visit` 两个方法。前者用于发送缓冲区内的消息，后者用于遍历消息元素。消息发送完成后，还需要触发 `send` 事件并将结果存储于 `results` 数组中。

与此同时，我们还需要修改 `TelegramBot` 类，为其添加静态属性。实现了 `MessageEncoder` 静态属性后，就无需手动实现 `bot.sendMessage()` 和 `bot.sendPrivateMessage()` 方法了：

bot.ts

    export class TelegramBot<C extends Context> extends Bot<C, TelegramBot.Config> {
      static MessageEncoder = TelegramMessageEncoder
    }

### 行内元素 [​](#inline)

上面的例子仅仅包含了消息编码器的基本结构，并未实现除了文本外的任何消息元素。对于任何非文本元素，上面的代码都会回退到其内部的文本。要添加更多消息元素的支持，只需在 `visit` 方法中添加更多的判断分支，就像这样：

ts

    if (type === 'text') {
      this.payload.text += h.escape(attrs.content)
    } else if (['b', 'strong', 'i', 'em', 'u', 'ins', 's', 'del'].includes(type)) {
      // 这些元素都是 Telegram 已经支持的，直接渲染成 HTML 即可
      this.payload.text += `<${type}>`
      await this.render(children)
      this.payload.text += `</${type}>`
    } else if (type === 'at') {
      // 将 at 渲染为用户链接
      this.payload.text += `<a href="tg://user?id=${attrs.id}">@${attrs.name || attrs.id}</a>`
    } else {
      await this.render(children)
    }

### 消息分片 [​](#fragment)

在 Koishi 中，一次消息发送可能在目标平台产生多条独立的消息，称为消息分片。这也是为什么上面的 `results` 是一个数组。消息分片产生的原因是多样的：

*   某些元素的语义就是发送独立的消息 (例如 `<message>`)
*   部分平台不支持某些消息元素的组合 (例如图文混合发送)，此时必须对消息进行拆分
*   待发送的消息长度超出平台限制，此时必须对消息进行拆分

在需要对消息进行分片的场合，我们可以手动调用 `flush()` 方法。下面的代码展示了如何实现 `<message>` 元素：

ts

    // 忽略前面的部分
    } else if (type === 'message') {
      // 在解析内部元素之前先清空缓冲区
      await this.flush()
      await this.render(children)
      await this.flush()
    } else ...

### 资源元素 [​](#asset)

由于不同平台对于媒体资源的支持类型、发送方式、渲染形式有所不同，因此资源元素的情况会更加复杂。可以大致将各种平台规定的发送方式分为以下几类：

1.  通过不同的 API 发送不同类型的资源 (例如 Telegram)
2.  使用统一的 API，但通过不同的字段区分资源类型 (例如 Discord)
3.  先上传资源获得链接或资源 ID，再调用发送 API (例如 Lark)

这里我们还是以 Telegram 平台为例。首先照例修改 `visit` 方法。由于 Telegram 仅支持资源 + 文本的组合 (文本显示在资源下方)，因此我们需要进行消息分片：

ts

    // 忽略前面的部分
    } else if (['image', 'audio', 'video', 'file'].includes(type)) {
      await this.flush()
      this.asset = element
    } else ...

接着，我们需要在 `flush` 方法中处理资源元素。Telegram 的资源上传接口是 `sendPhoto`、`sendAudio` 等，与文本所用的 `sendMessage` 不同，因此我们需要根据资源类型进行判断：

ts

    class TelegramMessageEncoder<C extends Context> extends MessageEncoder<C, TelegramBot<C>> {
      async flush() {
        let message: Telegram.Message
        if (this.asset) {
          const form = new FormData()
          for (const key in this.payload) {
            form.append(key, this.payload[key].toString())
          }
          const { type, attrs } = this.asset
          const { filename, data } = await this.bot.ctx.http.file(attrs.src, attrs)
          if (type === 'img') {
            form.append('photo', data, filename)
            message = await this.bot.internal.sendPhoto(form)
          } else if (type === 'audio') {
            form.append('audio', data, filename)
            message = await this.bot.internal.sendAudio(form)
          } else if (type === 'video') {
            form.append('video', data, filename)
            message = await this.bot.internal.sendVideo(form)
          } else if (type === 'file') {
            form.append('document', data, filename)
            message = await this.bot.internal.sendDocument(form)
          }
          this.asset = null
        } else if (this.payload.text) {
          message = await this.bot.internal.sendMessage(this.payload)
        }
        await this.addResult(message)
        this.payload.text = ''
      }
    }

差不多这样就实现了资源元素的发送。值得一提的是，这里的代码使用了 `http.file()` 方法。它可以自动为我们处理 `http:`、`file:`、`data:` 等各种协议的资源链接，并将它们统一转换为 `ArrayBuffer`。这可以省去适配器解析资源链接的步骤，对于适配器开发是非常方便的。

进阶知识 [​](#advanced)
-------------------

下面的知识并非适用于所有适配器。但对于一些特殊的平台，你可能会用到它们。

### 发送被动消息 [​](#passive)

我们通常将机器人做出的交互行为分为两种：主动交互和被动交互。

*   主动交互是指机器人主动进行某些操作，例如定时任务、通知推送。
*   被动交互是指机器人接收到特定事件后做出的响应，例如消息回复、入群欢迎。

遗憾的是，部分平台会限制机器人的主动交互能力。例如，在 QQ (官方机器人) 中，机器人每天只能发送极少量的主动消息；而对于被动消息，则必须在用户发送消息后的短时间内回复。这种平台被称为**被动型平台**。

被动型平台要求适配器在发送消息时尽可能带有回复目标。当然 Koishi 也提供了解决方案：

ts

    class QQGuildMessageEncoder {
      async flush() {
        await this.bot.internal.sendMessages(this.channelId, {
          content: this.content,
          msgId: this.options?.session?.messageId,
        })
      }
    }

在这一段代码中使用了 `this.options`，它存储了一些额外的发送选项。其中 `session` 正好对应着接收到消息的会话对象。当我们调用 `session.send()` 时，Koishi 会把当前的会话对象传递给 `MessageEncoder`。这样一来，我们就可以在发送消息时带上回复目标了。

### 资源反向代理 [​](#reverse-proxy)

一些平台会使用 ID 标识资源文件 (例如 Lark)。当你接收到来自平台的消息时，拿到的是资源 ID 而非资源链接。此时你需要将资源 ID 转换为资源链接，才能构造合法的资源元素。

TIP

Telegram 是另一种特殊情况。尽管其提供的资源链接是可用的，但这个链接中会明文包含机器人令牌，并非可以公开使用的链接。因此 Telegram 和其他类似平台也适用于这一节的内容。

对于这种情况，一种**不推荐**的做法是直接下载资源，并转存为 `data:` 链接放入消息中。之所以不推荐，是因为这种做法有两大致命缺点：

1.  这些图片本来可以按需加载，但现在却被强制下载到本地，造成额外的带宽消耗。
2.  编码为 `data:` 会导致消息体积大幅增加，极大影响消息处理的性能。

那么，有没有更好的解决方案呢？答案便是资源反向代理。我们要做的，是在本地提供一个路由，将资源 ID 映射到资源链接。这样一来，上面提到的两个问题也就都解决了。

下面是 Lark 适配器的一部分代码，用于实现资源反向代理 (位于 `adapter.ts`)：

ts

    class LarkAdapter {
      static inject = ['server']
    
      constructor(ctx: Context) {
        ctx.server.get('/lark/assets/:message_id/:key', async (ctx) => {
          const key = ctx.params.key
          const messageId = ctx.params.message_id
          const selfId = ctx.request.query.self_id
          const bot = this.bots.find((bot) => bot.selfId === selfId)
          if (!bot) return ctx.status = 404
          const response = await bot.http(`/im/v1/messages/${messageId}/resources/${key}`, {
            method: 'GET',
            params: { type: 'image' },
            responseType: 'stream',
          })
          ctx.status = 200
          ctx.response.headers['content-type'] = response.headers.get('content-type')
          ctx.response.body = response.data
        })
      }
    }

然后在接收消息的逻辑中，我们只需要将资源 ID 转换为资源链接即可：

ts

    h.image(`http://${host}/image/${message_id}/${image_key}?self_id=${selfId}`)

TIP

反向代理同时也带来了一个新的问题，那就是当这个链接被原样发送时，外网可能无法访问到这个链接。但无需担心，上面提到的 `http.file()` 方法恰好可以解决这个问题。因此，即使经过了反向代理，Koishi 也可以确保消息的跨平台转发插件能够正常工作。

### 扩展消息元素 [​](#extension)

平台可以提供扩展消息元素，但需要加上平台通用名称作为前缀。下面是一个例子：

html

    <kook:card size="lg">
      <kook:countdown end-time="1608819168000"/>
    </kook:card>

标准元素的平台扩展属性也可以通过加上平台通用名称作为前缀的方式声明。下面是一个例子：

html

    <!-- src 是 audio 元素的标准属性。 -->
    <!-- 但 cover 并未标准化，所以需要加前缀。 -->
    <audio src="url1" kook:cover="url2"/>

TIP

平台扩展消息元素的属性是否需要前缀由 SDK 实现自行决定。如果某个消息元素希望在未来标准化，那么加上前缀可以降低迁移成本。如果没有标准化需要，那么去掉前缀在书写上更方便。

---



## [https://koishi.chat/zh-CN/guide/adapter/integration.html](https://koishi.chat/zh-CN/guide/adapter/integration.html)

平台集成 [​](#平台集成)
===============

至此，Koishi 的适配器开发已经接近尾声。经过前面的几节内容，我们的适配器已经封装了平台接口，与服务器稳定地进行连接，并能够顺利地接受和发送消息。但除此以外，部分平台还提供了一些额外的能力，允许机器人做得更好。Koishi 当然也要把这些能力集成到机器人中。

斜线指令 [​](#slash-command)
------------------------

TIP

相关章节：[指令开发](./../basic/command.html)

部分平台为机器人提供了斜线指令功能，用于在聊天框中快速输入指令。在 Discord 中差不多是这个效果：

适配器可以通过 `bot.updateCommands()` 方法，将 Koishi 的指令注册为平台的斜线指令：

ts

    class DiscordBot {
      async updateCommands(commands: Universal.Command[]) {
        // 这里忽略了部分细节，仅供参考
        const updates = commands.map(Discord.encodeCommand)
        await this.internal.bulkOverwriteGlobalApplicationCommands(this.selfId, updates)
      }
    }

用户语言偏好 [​](#user-locale)
------------------------

TIP

相关章节：[多语言支持](./../i18n/)

部分平台本身支持多种语言。在这样的平台中，用户可以自行设置自己的语言偏好。当用户向机器人发送消息时，Koishi 就可以根据用户的语言偏好，做出相应语言的回复。

而适配器所需要做的，就只有设置 `session.locales` 属性 (以 Telegram 平台为例)：

ts

    if (from.language_code) {
      // 这里为了简化逻辑，只取语言码的前两位
      session.locales = [from.language_code.slice(0, 2)]
    }

---



## [https://koishi.chat/zh-CN/guide/console/index.html](https://koishi.chat/zh-CN/guide/console/index.html)

扩展控制台 [​](#扩展控制台)
=================

TIP

在学习本章之前，建议先完整阅读 [入门 > 认识控制台](./../../manual/usage/market.html#认识控制台)。

创建扩展 [​](#创建扩展)
---------------

在插件目录中新建这几个文件：

diff

    └── example
    +   ├── client
    +   │   ├── index.ts
    +   │   ├── page.vue
    +   │   └── tsconfig.json
        ├── src
        │   └── index.ts
        ├── package.json
        └── tsconfig.json

client/index.ts

    import { Context } from '@koishijs/client'
    import Page from './page.vue'
    
    export default (ctx: Context) => {
      // 此 Context 非彼 Context
      // 我们只是在前端同样实现了一套插件逻辑
      ctx.page({
        name: '页面标题',
        path: '/custom-page',
        component: Page,
      })
    }

client/page.vue

    <template>
      <k-layout>
        <k-card>扩展内容</k-card>
      </k-layout>
    </template>

client/tsconfig.json

    {
      "compilerOptions": {
        "rootDir": ".",
        "module": "esnext",
        "moduleResolution": "node",
        "types": [
          // 这一行的作用是导入相关全局类型
          // 以便于在编辑器中显示更好的代码提示
          "@koishijs/client/global",
        ],
      },
      "include": ["."],
    }

然后修改插件的 `package.json`，添加以下依赖：

package.json

    {
      "peerDependencies": {
        "@koishijs/plugin-console": "^5.11.0"
      },
      "devDependencies": {
        "@koishijs/client": "^5.11.0"
      }
    }

接着修改你的入口文件：

src/index.ts

    import { Context } from 'koishi'
    // 此处需要导入 @koishijs/plugin-console 以获取类型
    import {} from '@koishijs/plugin-console'
    import { resolve } from 'path'
    
    export const name = 'my-plugin'
    
    export function apply(ctx: Context) {
      // 在已有插件逻辑的基础上，添加下面这段
      ctx.inject(['console'], (ctx) => {
        ctx.console.addEntry({
          dev: resolve(__dirname, '../client/index.ts'),
          prod: resolve(__dirname, '../dist'),
        })
      })
    }

启动应用，并在控制台中配置你的插件。现在你已经可以在网页中看到并调试自己刚刚创建的页面了。

---



## [https://koishi.chat/zh-CN/guide/console/data.html](https://koishi.chat/zh-CN/guide/console/data.html)

数据交互 [​](#数据交互)
===============

Koishi 控制台前后端的数据交互基本是通过 WebSocket 实现的。为了适应不同的场景，我们提供了多种数据交互的形式。

被动推送 [​](#被动推送)
---------------

后端代码：

src/index.ts

    import { Context } from 'koishi'
    import { resolve } from 'path'
    import { DataService } from '@koishijs/plugin-console'
    
    declare module '@koishijs/plugin-console' {
      namespace Console {
        interface Services {
          custom: CustomProvider
        }
      }
    }
    
    class CustomProvider extends DataService<string[]> {
      constructor(ctx: Context) {
        super(ctx, 'custom')
      }
    
      async get() {
        return ['Hello', 'World']
      }
    }
    
    export const name = 'my-plugin'
    export const inject = ['console']
    
    export function apply(ctx: Context) {
      ctx.plugin(CustomProvider)
    
      ctx.console.addEntry({
        dev: resolve(__dirname, 'client/index.ts'),
        prod: resolve(__dirname, 'dist'),
      })
    }

前端代码：

client/index.ts

    import { Context } from '@koishijs/client'
    import Page from './page.vue'
    
    export default (ctx: Context) => {
      ctx.page({
        name: '页面标题',
        path: '/custom-page',
        // 只有当获得了 custom 数据，才可以访问页面
        fields: ['custom'],
        component: Page,
      })
    }

vue

    <template>
      <!-- 这里应该有类型支持，并且支持数据响应式变化 -->
      <k-card>{{ store.custom }}</k-card>
    </template>
    
    <script>
    import { store } from '@koishijs/client'
    </script>

主动获取 [​](#主动获取)
---------------

后端代码：

src/index.ts

    import { Context } from 'koishi'
    import { resolve } from 'path'
    import { DataService } from '@koishijs/plugin-console'
    
    declare module '@koishijs/plugin-console' {
      interface Events {
        'get-greeting'(): string[]
      }
    }
    
    export const name = 'my-plugin'
    export const inject = ['console']
    
    export function apply(ctx: Context) {
      ctx.console.addListener('get-greeting', () => {
        return ['Hello', 'World']
      })
    
      ctx.console.addEntry({
        dev: resolve(__dirname, 'client/index.ts'),
        prod: resolve(__dirname, 'dist'),
      })
    }

client/page.vue

    <template>
      <k-card>{{ greeting }}</k-card>
    </template>
    
    <script>
    import { send } from '@koishijs/client'
    import { ref } from 'vue'
    
    const greeting = ref<string[]>()
    
    send('get-greeting').then(data => {
      greeting.value = data
    })
    </script>

权限管理 [​](#权限管理)
---------------

当你引入了 @koishijs/plugin-auth 插件之后，你可以为你的页面访问和数据交互引入鉴权机制：

ts

    // 只有已登录并且权限等级不低于 3 的用户才能访问此接口
    ctx.console.addListener('get-greeting', () => {
      return ['Hello', 'World']
    }, { authority: 3 })

client/index.ts

    ctx.page({
      name: '页面标题',
      path: '/custom-page',
      // 只有已登录并且权限等级不低于 3 的用户才能访问此界面
      authority: 3,
      component: Page,
    })

---



## [https://koishi.chat/zh-CN/guide/console/client.html](https://koishi.chat/zh-CN/guide/console/client.html)

客户端开发 [​](#客户端开发)
=================

布局组件 [​](#布局组件)
---------------

为了方便控制台开发，Koishi 也提供了一些组件。其中的一部分你已经在前面的两节中见过了。

[`<k-layout>`](./../../api/console/component.html#k-layout) 创建了一个新的页面布局。你扩展任何页面都需要用到它。这个组件有一些插槽：

*   `header`：标题栏的内容
*   `left`：左侧栏的内容
*   `default`：页面主体的内容

除了添加新页面外，窗口底部的状态栏也可以扩展：

ts

    import Status from './status.vue'
    
    ctx.slot({
      type: 'status-left',
      component: Status,
    })

vue

    <template>
      <k-status>
        这段文字将会显示在状态栏中。
      </k-status>
    </template>

在上面的例子中，[`<k-status>`](./../../api/console/component.html#k-status) 创建了一个状态栏元素。

你甚至还可以直接添加页面元素，例如 [live2d](https://github.com/koishijs/koishi-plugin-live2d) 插件就为控制台添加了一个 live2d 的看板娘：

ts

    import Live2D from './live2d.vue'
    
    ctx.slot({
      type: 'global',
      component: Live2D,
    })

使用插槽 [​](#使用插槽)
---------------

你应该已经注意到了，在上面的两个例子中，我们都使用了 [`ctx.slot()`](./../../api/console/context.html#ctx-slot) 来扩展某些元素。这个方法的作用是向控制台的某个区域中注入 Vue 组件。而上面的 `status-left` 和 `global` 则是两个插槽的名称，分别对应了状态栏左侧区域和整个页面区域。

这种注入方式不仅可以作用于控制台本身，也可以作用于其他控制台扩展。例如，当你开发了一个控制台页面，并希望其他插件可以在你的页面中注入一些内容时，你可以这样做：

vue

    <template>
      <k-layout>
        <p>这里是一些文字</p>
        <k-slot name="custom" />
        <p>这里是一些文字</p>
      </k-layout>
    </template>

这样一来，其他控制台插件就可以通过 `ctx.slot()` 来向你的页面中注入内容了。

一个插槽可以同时被注入多次。你可以为每次插槽注入指定优先级和显示条件：

ts

    ctx.slot({
      type: 'custom',
      component: Foo,
      order: 100,
    })
    
    ctx.slot({
      type: 'custom',
      component: Bar,
      order: 200,
      disabled: () => !store.bar,
    })

`order` 更高的插槽会被优先显示；`disabled` 函数返回 `true` 时，插槽不会被显示。因此在上面的例子中，`Bar` 组件总是显示在 `Foo` 组件的前面，但只有当 `store.bar` 存在时才会显示。

用户设置 实验性 [​](#用户设置)
-------------------

到此为止，我们所了解的插件配置都是 [直接在插件中声明](./../plugin/schema.html)、[存储于配置文件中](./../develop/config.html) 的。这在绝大多数情况下都是合理的——机器人管理员决定了插件的具体行为，而这些行为也不应该由用户决定。但实际上还有另一种情况：插件的某些行为可以由用户自由决定。例如机器人所使用的语言、控制台的主题等等。我们将这些配置统称为「用户设置」。

在控制台中，插件配置和用户配置是分离的。插件配置只有机器人的管理员有权查看和修改，而每个用户都可以查看和修改自己的用户配置。插件开发者也应当妥善区分这两种配置，以提高插件的可定制性。使用 [`ctx.settings()`](./../../api/console/context.html#ctx-settings) 可以在用户设置界面中添加配置表单：

ts

    ctx.settings({
      id: 'appearance',
      schema: Schema.object({
        wallpaper: Schema.object({
          image: Schema.string().description('要使用的背景图片。'),
          opacity: Schema.number().description('前景的不透明度。'),
        }).description('壁纸设置'),
      }),
    })

使用 `useConfig()` 可以在控制台中读取用户设置：

ts

    const config = useConfig()
    config.value.wallpaper.image

动作与菜单 实验性 [​](#动作与菜单)
---------------------

控制台的许多地方都会用到菜单，其中大家最熟悉的便是每个页面标题栏右侧的菜单按钮。除此以外，部分页面还提供了上下文菜单。想要定义菜单，我们首先需要了解 **动作 (Action)** 这一概念。

控制台中可以执行的任何一个操作都可以视为一个动作。每个动作都有着唯一的标识符，例如 `explorer.save` 表示保存当前文件、`explorer.refresh` 表示刷新文件列表等等。已知动作标识符的情况下，可以通过 [`ctx.menu()`](./../../api/console/context.html#ctx-menu) 来描述一个菜单，并在 `<k-layout>` 中引用它：

ts

    ctx.menu('explorer', [{
      id: '.save',
      icon: 'save',
      label: '保存',
    }, {
      id: '.refresh',
      icon: 'refresh',
      label: '刷新',
    }])

vue

    <template>
      <!-- 在页面中指定菜单 -->
      <k-layout menu="explorer">
        页面内容
      </k-layout>
    </template>

当然，光有菜单还不够，我们还需要实现上面的动作。这可以通过 [`ctx.action()`](./../../api/console/context.html#ctx-action) 来完成：

vue

    <script lang="ts" setup>
    import { send, useContext } from '@koishijs/client'
    
    const ctx = useContext()
    
    // 实现菜单动作
    ctx.action('explorer.save', {
      disabled: () => content === oldContent,
      action: () => send('explorer/write', filename, content),
    })
    </script>

如果要实现上下文菜单，同样需要首先在入口文件中描述菜单项：

ts

    ctx.menu('entry', [{
      id: '.rename',
      label: '重命名',
    }, {
      id: '.remove',
      label: '删除',
    }])

然后在组件中使用 [`useMenu()`](./../../api/console/composition.html#usemenu) 来获取菜单项的点击事件：

vue

    <template>
      <!-- 这里显示了文件列表 -->
      <div v-for="entry in entries">
        <!-- 右击任意文件名会呼出上述菜单 -->
        <div @contextmenu.stop="trigger($event, entry)">{{ entry.filename }}</div>
      </div>
    </template>
    
    <script lang="ts" setup>
    import { useContext, useMenu } from '@koishijs/client'
    
    const ctx = useContext()
    const trigger = useMenu('entry')
    
    // 实现菜单动作
    ctx.action('entry.remove', {
      action: ({ entry }) => send('explorer/remove', entry.filename),
    })
    </script>

---



## [https://koishi.chat/zh-CN/guide/console/theme.html](https://koishi.chat/zh-CN/guide/console/theme.html)

主题开发 实验性 [​](#主题开发)
===================

Koishi 也允许插件定义控制台主题。让我们先从简单的色彩主题开始。

色彩主题 [​](#色彩主题)
---------------

[theme-vanilla](https://github.com/koishijs/koishi-plugin-theme-vanilla) 插件提供了许多色彩主题，你可以参考它的源码来开发自己的主题：

ts

    // 引入定义主题色的 CSS 文件
    import './index.scss'
    
    ctx.theme({
      id: 'coffee-dark',
      name: 'Coffee Dark',
    })
    
    ctx.theme({
      id: 'coffee-light',
      name: 'Coffee Light',
    })

如你所见，要定义一个色彩主题非常简单，只需要调用 [`ctx.theme()`](./../../api/console/context.html#ctx-theme) 即可。其中，`id` 用于标识主题，`name` 则会显示在主题选择器中。

TIP

请注意：`id` 必须以 `-dark` 或 `-light` 结尾，否则 Koishi 将无法正确回退 CSS 变量！

接下来让我们看看 `index.scss` 的内容：

scss

    :root, .theme-root {
      &[theme=coffee-dark] {
        --bg1: #231F1E;
        --bg2: #262120;
        --bg3: #292423;
        --bg4: #342A27;
      }
    
      &[theme=coffee-light] {
        --bg1: #EEE9E7;
        --bg2: #EAE4E1;
        --bg3: #E6DFDC;
        --bg4: #E3DBD6;
      }
    }

Koishi 为主题系统预定义了许多 CSS 变量。只需要在属性选择器中修改这些变量的值，一个色彩主题就大功告成了。

改变布局 [​](#改变布局)
---------------

Koishi 同样允许主题改变控制台的布局：

ts

    import root from './root.vue'
    import layout from './layout.vue'
    
    ctx.theme({
      id: 'windows-light',
      name: 'Windows Light',
      components: { root, layout },
    })

在上面的例子中，[`ctx.theme()`](./../../api/console/context.html#ctx-theme) 接受一个额外的 `components` 选项，用于覆盖默认的布局组件。其中，`root` 用于定制整个控制台的布局，`layout` 用于定制 `<k-layout>` 的实现。

---



## [https://koishi.chat/zh-CN/guide/i18n/index.html](https://koishi.chat/zh-CN/guide/i18n/index.html)

基本用法 [​](#基本用法)
===============

TIP

在学习本章之前，建议先完整阅读 [入门 > 国际化](./../../manual/usage/customize.html#国际化)。

如果你在运营一个大型社区，那么你可能会遇到这种场景：群组内设立了许多不同语言的频道，每个频道分别供不同地区的用户进行交流。在这种情况下，最合适的做法是让你的机器人在不同的频道下使用不同的语言进行回复。本质上，这不会改变机器人的运行逻辑，因此最好的做法是将涉及的每一段文本都抽离出来，通过统一的方式进行管理，并在发送前进行本地化渲染。

基本示例 [​](#基本示例)
---------------

让我们先看一个最简单的例子：

ts

    ctx.i18n.define('zh-CN', { hello: '你好！' })
    ctx.i18n.define('en-US', { hello: 'Hello!' })

上面的代码定义了两种语言下 `hello` 对应的翻译文本。其中 `zh-CN` 和 `en-US` 称为语言名，`hello` 称为渲染路径，后面的字符串是对应的翻译文本。

现在我们把它用在 `session.text()` 中：

ts

    ctx.middleware((session, next) => {
      if (session.content === 'greeting') {
        return session.text('hello')
      } else {
        return next()
      }
    })

A

Alice

greeting

Koishi

你好！

我们看到机器人回复了「你好！」，这是因为 Koishi 使用的默认语言是中文。

现在，如果我们希望它在某个频道使用英文，我们只需设置这个频道的属性：

ts

    channel.locales = ['en-US']

A

Alice

greeting

Koishi

Hello!

模板能力 [​](#模板能力)
---------------

### 插值语法 [​](#插值语法)

向 `session.text()` 中传入第二个参数，就可以在模板中使用单花括号插值。花括号 `{}` 中的内容将对应传入列表的索引。

ts

    ctx.i18n.define('zh-CN', { hello: '你好，{0}！' })
    ctx.i18n.define('en-US', { hello: 'Hello, {0}!' })
    
    ctx.middleware((session, next) => {
      if (session.content === 'greeting') {
        return session.text('hello', [session.author.name])
      } else {
        return next()
      }
    })

A

Alice

greeting

Koishi

Hello, Alice!

这里的参数也可以是一个对象，此时花括号中的内容仍然表示对象的索引。

ts

    ctx.i18n.define('zh-CN', { hello: '你好，{username}！' })
    ctx.i18n.define('en-US', { hello: 'Hello, {username}!' })
    
    ctx.middleware((session, next) => {
      if (session.content === 'greeting') {
        return session.text('hello', session.author)
      } else {
        return next()
      }
    })

如果要访问对象深层的内容，只需将多个属性之间用 `.` 连接。利用这种方法，你甚至可以把整个 `session` 传进去：

ts

    ctx.i18n.define('zh-CN', { hello: '你好，{author.name}！' })
    ctx.i18n.define('en-US', { hello: 'Hello, {author.name}!' })

上述三段代码的实际效果完全相同，可以根据自己的需要进行选择。

如果你希望对属性值进行某些计算，传入 Javascript 表达式也是可以的：

ts

    ctx.i18n.define('zh-CN', { list: '列表：{arr.join(",")}' })
    ctx.i18n.define('en-US', { list: 'List: {arr.join(",")}' })

TIP

目前支持的表达能力会受到解析器和特殊语法的限制。请避免在表达式中引入 `}`，以免造成歧义。

此外，如果向 `session.text()` 传入的二参数是一个数组，那么直接写 `{0}` 将表示数组中的第一个元素 (而非作为 JavaScript 表达式的 `0`)。

### 使用消息元素 [​](#使用消息元素)

你也可以在模板中使用 [消息元素](./../basic/element.html) 语法。消息元素的属性同样使用 `{}` 进行插值：

ts

    ctx.i18n.define('zh-CN', { hello: '你好，<at id={userId}/>！' })
    ctx.i18n.define('en-US', { hello: 'Hello, <at id={userId}/>!' })

你也可以使用消息组件，例如使用 `<i18n>` 组件引用其他翻译，或使用 `<i18n:time>` 表示本地化的时间：

ts

    ctx.i18n.define('zh-CN', { remain: '剩余时间：<i18n:time value={value}/>' })
    ctx.i18n.define('en-US', { remain: 'Time Remain: <i18n:time value={value}/>' })

### 条件和循环 实验性 [​](#条件和循环)

我们为模板提供了一些基本的控制流语法，它参考了 [Svelte](https://svelte.dev/) 的设计 (但并未完整实现)。你可以在模板中通过 `{#if}` 和 `{#each}` 来实现条件和循环。例如，下面的代码将会渲染一个列表：

html

    {#if list.length === 0}
      列表中没有元素。
    {:else}
      {#each list as item}
        {item}
      {/each}
    {/if}

TIP

如果要使用这种层面的模板能力，那么你的代码已经不适合使用 `ctx.i18n.define()` 定义了。建议参考 [下一节](./translation.html) 中的做法，将不同语言的模板放入不同的文件中，以方便编辑和管理。

渲染回退 [​](#渲染回退)
---------------

一次完整的本地化渲染可能涉及多种不同优先级的语言和渲染路径。当首选语言的首选路径对应的翻译文本不存在时，会依次尝试使用其他翻译，这就是渲染回退。

### 基于语言的回退 [​](#基于语言的回退)

首先需要了解的是基于语言的回退。根据 [IETF 语言标签](https://zh.wikipedia.org/wiki/IETF%E8%AA%9E%E8%A8%80%E6%A8%99%E7%B1%A4) 规范，一个语言名称可以包含由 `-` 分隔的多个部分，例如 `de-DE-bavarian`。用户可以为应用设置 [`config.i18n.locales`](./../../api/core/app.html#i18n-locales) 来指定可用的语言列表，这些语言将按照 `-` 分隔符形成一棵字典树，而 Koishi 会按照以下规则进行回退：

1.  找到目标语言的在字典树中出现的最长前缀对应的节点；
2.  按照用户配置的优先级渲染改节点的子树所包含的语言，并将它们移除；
3.  如果此时仍有未被渲染过的语言，那么回到 1 继续遍历，直到所有语言被遍历完全。

例如，如果用户配置的语言列表为 `zh-CN`, `en-US`, `zh-TW`, `en-GB`，则对于不同的目标语言会生成对应的回退序列：

*   目标语言为 `en`，回退序列为 `en`, `en-US`, `en-GB`, , `zh`, `zh-CN`, `zh-TW`
*   目标语言为 `zh-TW`，回退序列为 `zh-TW`, `zh`, `zh-CN`, `en`, `en-US`, `en-GB`,
*   目标语言为 `de-DE`，回退序列为 , `zh`, `zh-CN`, `zh-TW`, `en`, `en-US`, `en-GB`
*   目标语言为 `en`, `zh-TW`，回退序列为 `en`, `en-US`, `en-GB`, `zh-TW`, `zh`, `zh-CN`,
*   目标语言为 `zh-TW`, `en`，回退序列为 `zh-TW`, `en`, `en-US`, `en-GB`, `zh`, `zh-CN`,

请注意，空字符串也被视为合法的语言，其所代表的是「没有指定语言」的情况。在实践中，空语言的使用是非常广泛的，例如当用户使用下面的代码定义指令：

ts

    ctx.command('echo', '回声')

此时我们无法推测出「回声」的语言，因此它将会被作为路径 `commands.echo.name` 注册到空语言下。用户可以为其定义其他语言的翻译，但在未命中任何翻译时，它将回退到空语言。

### 基于会话的回退 [​](#基于会话的回退)

实际的本地化渲染通常发生在消息会话中。对于一个会话，我们可以从以下几个维度来确定它的目标语言 (每个维度都可以存在多个目标语言)：

*   会话语言 (`session.locales`)
*   频道语言 (`session.channel.locales`)
*   群组语言 (`session.guild.locales`)
*   用户语言 (`session.user.locales`)

最终的目标语言将会是上述语言按顺序的并集，再根据前面介绍的规则进行回退渲染。

会话语言可以在一些交互场景中被直接感知得到。例如，用户如果在聊天平台中已经设置了语言偏好 (并且聊天平台提供了相应的 API)，则相关的设置可以通过适配器插件提供给会话。又比如，当开发者为一个指令设置了多种语言的别名时，可以为这些别名手动指定语言，当用户调用某一个别名时，Koishi 会按照设定好的语言来回答。

用户语言与频道、群组语言的优先关系可以通过 [`config.i18n.output`](./../../api/core/app.html#i18n-output) 来指定。默认情况下频道和群组的语言优先级高于用户语言，但是你可以将其设置为 `prefer-user` 来改变这一行为。

### 基于路径的回退 [​](#基于路径的回退)

你也可以配置多个路径，将会按照顺序查找翻译，直到找到一个翻译为止。

ts

    session.text(['foo', 'bar'])

TIP

路径回退的优先级低于语言回退。举个例子，假如可选的语言包括 A 和 B，路径包括 1 和 2。翻译 A1 不存在，但是翻译 A2 和 B1 都存在。这种情况下会输出 B1 而非 A2。采用这种设计是因为不同的路径通常表达了不同的逻辑。相比语言的正确性，逻辑的正确性更重要。

利用这种行为，你可以实现静默渲染。下面的代码当未找到翻译时，将只会输出一个空串，并且不会输出警告：

ts

    session.text(['foo', ''])

### 用户侧覆写 [​](#用户侧覆写)

用户可以通过 [locales](./../../plugins/console/locales.html) 插件提供本地翻译，且这些翻译的优先级高于插件自身提供的翻译。可以认为，从用户提供的翻译到插件提供的翻译，也是一种回退关系。

关于用户侧覆写的更多信息，请参见 [入门 > 深入定制机器人](./../../manual/usage/customize.html)。

---



## [https://koishi.chat/zh-CN/guide/i18n/translation.html](https://koishi.chat/zh-CN/guide/i18n/translation.html)

本地化文件 [​](#本地化文件)
=================

`i18n.define()` 允许开发者为自己的插件提供多套翻译，但直接将每种语言的翻译文本写进源代码并不利于代码的解耦。因此我们建议开发者将翻译文件写在一个单独的目录中，在插件中只需要引用这个目录中的文件即可：

diff

    └── example
        ├── src
        │   ├── locales
        │   │   ├── en-US.yml
        │   │   └── zh-CN.yml
        │   └── index.ts
        └── package.json

ts

    ctx.i18n.define('en-US', require('./locales/en-US'))
    ctx.i18n.define('zh-CN', require('./locales/zh-CN'))

TIP

在上面的例子中我们使用了 YAML 作为翻译文件的格式。这是因为它的语法简洁美观，非常适合本地化开发。你也可以采用 JSON 等任何你喜欢的格式进行开发。

TIP

Node.js 并不支持直接加载 `.yaml` / `.yml` 后缀的文件，但我们可以通过适当的 [register](https://nodejs.org/api/cli.html#-r---require-module) 解决这个问题。对此我们的官方脚手架已经内置了相应的支持。

指令本地化 [​](#指令本地化)
-----------------

在 [编写帮助](./../basic/command.html#编写帮助) 一节中，我们已经了解到指令和参数的描述文本都是在指令注册时就定义的。这种做法对单语言开发固然方便，但并不适合多语言开发，因为它将翻译逻辑与代码逻辑耦合了。如果你希望你编写的指令支持多语言，那么需要将翻译文本单独定义：

locales/zh-CN.yml

    commands:
      foo:
        description: 指令描述
        usage: |-
          指令用法
          可以是多行文本
        examples: |-
          foo qux
          foo --bar qux
        options:
          bar: 选项描述

ts

    ctx.command('foo').option('bar')

上述定义在语言文件中的内容会被 [help](./../../plugins/common/help.html) 等插件使用。

### 作用域渲染 [​](#作用域渲染)

如果我们希望在指令中输出一些本地化内容，为了避免与其他指令定义的内容相冲突，最好的办法是将这些内容与其他指令相关文本定义在一起：

locales/zh-CN.yml

    commands:
      greeting:
        description: 指令描述
        messages:
          morning: 早上好！
          evening: 晚上好！

但这样一来，你要在指令回调函数中写的东西就显得有点冗长了：

ts

    if (new Date().getHours < 12) {
      return session.text('commands.greeting.messages.morning')
    } else {
      return session.text('commands.greeting.messages.evening')
    }

有没有好的办法呢？由于我们在调用指令的回调函数时必然知道它属于哪一个指令，因此这些相同的前缀实际上是可以省略的。为了避免与全局定义的路径相冲突，我们用一个 `.` 表示当前指令的 `messages` 中的条目，就像这样：

ts

    if (new Date().getHours < 12) {
      return session.text('.morning')
    } else {
      return session.text('.evening')
    }

配置本地化 实验性 [​](#配置本地化)
---------------------

WARNING

配置本地化仍然是实验性功能，暂不支持被其他插件扩展。

插件配置中出现的文本也可以支持多语言。考虑下面的配置项：

ts

    Schema.object({
      foo: Schema.string().description('这是一个字符串。'),
      bar: Schema.number().description('这是一个数值。'),
    })

为了让其支持多语言，我们在翻译文件中增加名为 `_config` 的属性：

locales/zh-CN.yml

    _config:
      foo: 这是一个字符串。
      bar: 这是一个数值。

接着使用 `schema.i18n()` 加载翻译文件：

ts

    Schema.object({
      foo: Schema.string(),
      bar: Schema.number(),
    }).i18n({
      'zh-CN': require('./locales/zh-CN')._config,
      'en-US': require('./locales/en-US')._config,
    })

### 描述复杂类型 [​](#描述复杂类型)

默认情况下，上述 `_config` 对象的键对应配置项的键，值则是对应的翻译文本。这种写法足以覆盖大部分的情况，即便当出现嵌套的对象或引入 `intersect` 类型时也成立：

ts

    // 一个带有嵌套对象和 intersect 的类型
    Schema.intersect([
      Schema.object({
        foo: Schema.object({
          qux: Schema.boolean(),
        }),
      }),
      Schema.object({
        bar: Schema.string(),
        baz: Schema.number(),
      }),
    ])

yaml

    # 对应的翻译文件
    foo:
      qux: 这是一个配置项。
    bar: 这是另一个配置项。
    baz: 这是再一个配置项。

然而，当想要描述 `union`, `array`, `dict` 等类型，或是要为一个 `intersect` 中的不同对象设置不同的小标题时，上面的方法就行不通了。此时就需要引入一些高特殊属性：

ts

    // 一个带有 union, array 和 dict 的复杂类型
    Schema.intersect([
      Schema.object({
        shared: Schema.string(),
        type: Schema.union(['foo', 'bar']).required(),
      }),
      Schema.union([
        Schema.object({
          type: Schema.const('foo').required(),
          value: Schema.array(Number),
        }),
        Schema.object({
          type: Schema.const('bar').required(),
          text: Schema.Dict(string),
        }),
      ]),
    ])

yaml

    # 对应的翻译文件
    - shared: 公用的配置项。
      type:
        $desc: 选择一个分支。
        $inner:
          - 分支 1
          - 分支 2
    - - $desc: 分支 1
        $inner: 一个数值。
        value: 一个数值构成的数组。
      - $desc: 分支 2
        $inner: 一个字符串。
        text: 一个字符串构成的字典。

其中，任何一个节点的 `$desc` 属性表达其自身的文本，`$inner` 属性则用于描述其子节点 (对于 `array` 和 `dict` 是其内部类型，对于 `intersect` 和 `union` 是其内部类型的数组)。而在对象中，我们可以同时使用普通的属性和带有 `$` 前缀的特殊属性。

控制台本地化 实验性 [​](#控制台本地化)
-----------------------

WARNING

控制台本地化仍然是实验性功能，暂不支持被其他插件扩展。

如果你在开发支持多语言的控制台扩展，你可以组件中使用 `vue-i18n` 这样的国际化库：

ts

    import { useI18n } from 'vue-i18n'
    import zhCN from './zh-CN.yml'
    import enUS from './en-US.yml'
    
    const { t, setLocaleMessage } = useI18n({
      messages: {
        'zh-CN': zhCN,
        'en-US': enUS,
      },
    })
    
    // 支持热重载
    if (import.meta.hot) {
      import.meta.hot.accept('./zh-CN.yml', (module) => {
        setLocaleMessage('zh-CN', module.default)
      })
      import.meta.hot.accept('./en-US.yml', (module) => {
        setLocaleMessage('en-US', module.default)
      })
    }

TIP

注意：此时你的翻译文件应当处于 `client` 目录而非 `src/locales` 目录。

---



## [https://koishi.chat/zh-CN/guide/i18n/lang-pack.html](https://koishi.chat/zh-CN/guide/i18n/lang-pack.html)

语言包开发 实验性 [​](#语言包开发)
=====================

Koishi 及其官方插件通常会内置 `zh-CN` 和 `en-US` 两种语言。除此以外，还有一些语言同样由官方维护，但是并不会直接内置，而是以专门的插件的形式提供：

*   `de-DE`
*   `fr-FR`
*   `ja-JP`
*   `ru-RU`
*   `zh-TW`

对应的插件名将形如 @koishijs/plugin-locale-zh-tw (请注意插件名中只会使用小写字母)。

参与官方翻译项目 [​](#参与官方翻译项目)
-----------------------

我们在 [Crowdin](https://crowdin.com/project/koishi) 上维护了一个翻译项目，你可以在这里参与上述语言的翻译 (包括 `en-US`)。经过审核的翻译将会被自动同步到 GitHub 仓库中。如果你想翻译的语言不在上述列表中，可以向我们提交 Issue，也可以按照下面的指南发布第三方语言包。

编写第三方语言包 [​](#编写第三方语言包)
-----------------------

如果你不仅仅是想提供标准化的翻译，而是希望为 Koishi 提供不同的说话风格，这同样可以通过语言包来实现。根据 [IETF 语言标签](https://zh.wikipedia.org/wiki/IETF%E8%AA%9E%E8%A8%80%E6%A8%99%E7%B1%A4) 规范，我们可以在标准的语言标签后面添加一个后缀，来表示一个语言变种。例如，你可以通过编写名为 `zh-CN-ZAKO` 的语言包，来为 Koishi 提供一个二次元雌小鬼的说话风格：

—— 当要表达「权限不足」时 ——

Koishi

哼，你以为自己是谁啊？没那个本事就别想在这里装大头！

—— 当要表达「调用过于频繁，请稍后再试」时 ——

Koishi

哎哟，不要这么着急嘛，稍微等一下下，让人家缓口气~

---



## [https://koishi.chat/zh-CN/guide/i18n/crowdin.html](https://koishi.chat/zh-CN/guide/i18n/crowdin.html)

接入 Crowdin [​](#接入-crowdin)
===========================

[Crowdin](https://crowdin.com/) 是一个专业的本地化内容管理平台，不少商业项目使用该网站翻译并管理其本地化资源。同时，该网站也为开源项目和教学项目提供了免费或优惠的许可证。当你的项目中需要翻译的字符串较多，或需要支持很多种不同的语言，那么使用专业的管理平台会十分方便。

同时，Crowdin 也不仅仅是 CAT (计算机辅助翻译)，也提供了内容管理的功能，以及多种与第三方工具集成的方案，包括与 GitHub 等代码托管平台集成。由于 Crowdin 提供了 CLI 和 API 等多种方式管理项目资源，你也可以使用 CI (Continuous Integration，持续集成) 等方式管理你的项目资源。

TIP

除了 Crowdin，还有很多其他平台也提供类似的功能，有一些甚至是完全免费的，如：

*   [Transifex](https://www.transifex.com)
*   [Memsource](https://www.memsource.com/)
*   [Lokalise](https://lokalise.com/)
*   [POEditor](https://poeditor.com/)

你也可以尝试搜索 Translation Management System 或 Localization Platform 等关键词，整个互联网上有无数的本地化管理平台等着你去发掘。

注册及登录 Crowdin [​](#注册及登录-crowdin)
---------------------------------

你可以使用邮箱注册，也可以用谷歌账号、Github 账号等登录，与其他网站异曲同工，因此此处不再赘述。

TIP

如果你还是学生，并且成功申请了 GitHub 的学生开发包 (Student Pack)，在你使用 GitHub 账号成功登录 Crowdin 后会自动获赠价值 1500 美元的 1 年 Bronze 计划。

创建本地化项目 [​](#创建本地化项目)
---------------------

成功注册并登录 Crowdin 后，你会被自动导向你的[个人页面](https://crowdin.com/profile)。点击右上角的加号，即可创建项目。

TIP

若你的项目是开放源代码的，并且活跃了 4 个月及以上，你可以申请 Crowdin 的开源项目许可。当你成功创建项目后，填写[这个表单](https://crowdin.com/page/open-source-project-setup-request)，Crowdin 的客服人员会帮助你。

在新建项目界面，需要填写项目名称 (推荐和插件或机器人的名称一致)，选择是否公开项目，设置源语言和目标语言，然后点击创建项目按钮。

TIP

公开项目意味着所有 Crowdin 用户都能搜索到你的项目，也可以看到你的项目的所有内容，也可以向项目贡献翻译。如果你是通过开源项目免费许可的方式创建的项目，则只能创建公开项目。

### 项目结构 [​](#项目结构)

由于 Crowdin 会将待翻译的文件名显示在项目的文件列表中，为了不引起误会，你需要为每个待翻译的文件设置一个易懂的名称。同时，要保证 Crowdin 输出的翻译结果与你的项目结构一致。

因此推荐的做法是，为每种语言建立一个独立的文件夹，然后将待翻译的文件命名为项目名称，如下所示：

text

    echo/
      |-- i18n/
          |-- en/
              |-- echo.yaml
          |-- zh-CN/
              |-- echo.yaml
      |-- index.js
      |-- package.json

上传项目文件 [​](#上传项目文件)
-------------------

你可以通过网页手动上传文件，也可以通过 Crowdin 的 CLI 程序进行上传，或是使用集成让 Crowdin 直接从代码仓库同步文件。

### 手动上传 [​](#手动上传)

导航至 Crowdin 的内容 (Content) 界面，你可以点击上传文件 (Upload Files) 按钮上传**源语言**文件。

### 设置代码仓库集成 [​](#设置代码仓库集成)

除了手动上传，你还可以设置集成，让 Crowdin 自动同步 GitHub 等仓库里的文件，并可设置定期推送译文到相应的分支。

你可以点击[这里](https://support.crowdin.com/github-integration/)直达 Crowdin 关于 GitHub 集成的文档。如果你使用的是 Gitlab 等其他仓库，也可以在知识库里找到相应的指南。

回到项目主页，单击集成 (Integrations) 标签页，可以为你的项目设置集成。Crowdin 支持许多集成方案，找到你所使用的代码仓库并点击。

然后，单击 Set Up Integration，连接到你的代码仓库的账户，选择你想要设置集成的仓库，选择你想要获取原文和推送译文的分支，默认情况下 Crowdin 创建一个新的分支，名为 `l10n_` 加上原分支名，如图中所示的 `l10n_master`。

此外，你还需要点击分支名右边的编辑按钮，然后点添加文件筛选器 (Add File Filter)，在视图左边写上源文件和目标文件的模式匹配字符串之后，在右边切换并预览将会同步到 Crowdin 的文件列表，以及翻译后的文件名及其路径，你还可以添加更多的筛选器。确认添加无误后，单击 Save 按钮保存。

视图下方的 Push Source 选项默认是不勾选的，即 Crowdin 不会自动将翻译推送到仓库，打开这个选项后，Crowdin 会在对应的仓库开启一个 PR，并自动 rebase 到最新的分支，然后同步 Crowdin 上的同步到仓库。设置完成后，Crowdin 并不会自动开始同步，需要手动触发一次：点击表格右上角的 Sync Now，静待片刻即可同步完成。

### 通过 CLI 上传文件 [​](#通过-cli-上传文件)

Crowdin 还提供了一个 CLI 工具，可以通过命令行管理本地和远程的本地化资源文件。你可以通过 npm 或 yarn 安装。

bash

    $ npm i -g @crowdin/cli
    $ yarn global add @crowdin/cli

Crowdin 也提供了 Homebrew / apt 等多种安装方式，对于 Windows 用户，你也可以直接下载 Crowdin 所提供的安装程序安装，请查看 [Crowdin 的文档](https://support.crowdin.com/cli-tool/#installation)获知更多详情。

在运行 Crowdin 的 CLI 工具之前，你需要确保当前项目的根目录下存在名为 `crowdin.yml` 的配置文件，你可以运行 `crowdin init` 创建一个基础配置文件，修改其中的条目以适应你的项目。详细的介绍可以看 [Crowdin 的文档](https://support.crowdin.com/configuration-file/)。

TIP

`crowdin.yml` 中的配置项不仅适用于 Crowdin CLI，还可以在上述的代码仓库集成中发挥作用，Crowdin 会自动读取该文件以确定翻译的范围。

推荐在项目目录下的 `crowdin.yml` 文件中配置好文件筛选器，并且在 `$HOME/.crowdin.yml` 文件中存储你的 Crowdin 密钥等敏感信息，然后你就可以简单地运行 `crowdin upload sources` 上传源文件，而不需要每次都打出冗长的包含通配符的文件路径了。

### 文件类型 [​](#文件类型)

Crowdin 支持许多常见文件类型，如 `HTML`、`docx`、`pdf`，本地化软件框架支持的 `xliff` 与 `po` 等自然也不在话下，如果你不确定你的文件类型是否受支持，你可以在[这里](https://support.crowdin.com/supported-formats/)查看 Crowdin 支持的文件类型列表。

作为示例，我们使用的是 `YAML` 格式的文档，Crowdin 目前仅支持纯文本的 `YAML` 格式的文档，不支持 `anchor` 等高级功能。

当然你也可以使用 `JSON` 格式，但传统的 `JSON` 无法添加注释，显示在 Crowdin 上则会缺少足够的上下文信息。因为译者在 Crowdin 上无法看到源码，也无法看到翻译后的结果的显示样式，作为开发者应当通过各种方式向译者提供详尽的上下文信息。再综合考虑 `koishi` 对 i18n 的处理方式与 Crowdin 支持的格式，采用 `YAML` 是较为经济的选择。

Crowdin 会读取 `YAML` 中的键值和注释作为该待翻译字符串的上下文。以下面的 `YAML` 为例：

yaml

    commands:
      ping:
        description: 回复 ping 信息
        options:
          # 这是一段注释
          detail: 显示网络连接情况
        messages:
          pong: PONG! # 注释也可以写在后方

那么在翻译界面，Crowdin 会为 `回复 ping 信息` 这一字符串添加 `commands.ping.description` 作为其上下文信息。而对于 `显示网络连接情况` 这一字符串，除了显示 `commands.ping.options.detail` 以外，还会显示 `这是一段注释` 作为其上下文信息。当然，除了写在键值的上方，你也可以写在键值后方，效果是一样的。

yaml

    commands:
      dress:
        message:
          dress: '{name}今天穿了{color}色的裙子'

与大部分 CAT 工具一样，Crowdin 同样会标识出诸如 `{name}` 这样的插值语法，并且在译文缺少插值或译者翻译插值变量时报告错误。

进行翻译 [​](#进行翻译)
---------------

当你成功添加源文件之后，就可以着手进行翻译了。点开想要翻译的语言，打开对应文件，就可以进入 Crowdin 的在线翻译编辑器。假设你是从个人电脑打开的，那么视图会从左到右分成三个部分，左边是待翻译的字符串，中间是翻译区，右边是评论和参考区。

如果你对该项目申请了开源项目免费许可，那么该项目还会启用 Global TM 功能。这是 Crowdin 的共享翻译语料库，可以根据其他人的项目中存在的类似文本对当前的待翻译字符串进行提示，你的项目的字符串及翻译结果也会上传到这个语料库中。

下载翻译 [​](#下载翻译)
---------------

与上传翻译一样，Crowdin 提供了多种方式可以下载翻译结果，你可以直接通过网页下载单个或多个文件，也可以通过 Crowdin CLI 下载。如果你设置了与任何代码仓库的集成，并勾选了定时同步，则 Crowdin 会自动推送翻译结果到指定的分支。

---



## [https://koishi.chat/zh-CN/guide/#%E5%A6%82%E4%BD%95%E9%98%85%E8%AF%BB%E6%9C%AC%E6%8C%87%E5%8D%97](https://koishi.chat/zh-CN/guide/#%E5%A6%82%E4%BD%95%E9%98%85%E8%AF%BB%E6%9C%AC%E6%8C%87%E5%8D%97)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E4%B8%8E%E5%85%A5%E9%97%A8%E6%95%99%E7%A8%8B%E7%9A%84%E5%85%B3%E7%B3%BB](https://koishi.chat/zh-CN/guide/#%E4%B8%8E%E5%85%A5%E9%97%A8%E6%95%99%E7%A8%8B%E7%9A%84%E5%85%B3%E7%B3%BB)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E4%B8%8E%E8%BF%9B%E9%98%B6%E6%8C%87%E5%8D%97%E7%9A%84%E5%85%B3%E7%B3%BB](https://koishi.chat/zh-CN/guide/#%E4%B8%8E%E8%BF%9B%E9%98%B6%E6%8C%87%E5%8D%97%E7%9A%84%E5%85%B3%E7%B3%BB)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E9%A2%84%E5%A4%87%E7%9F%A5%E8%AF%86](https://koishi.chat/zh-CN/guide/#%E9%A2%84%E5%A4%87%E7%9F%A5%E8%AF%86)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E5%85%B3%E4%BA%8E-typescript](https://koishi.chat/zh-CN/guide/#%E5%85%B3%E4%BA%8E-typescript)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E8%AE%A9%E6%88%91%E4%BB%AC%E5%BC%80%E5%A7%8B%E5%90%A7](https://koishi.chat/zh-CN/guide/#%E8%AE%A9%E6%88%91%E4%BB%AC%E5%BC%80%E5%A7%8B%E5%90%A7)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---



## [https://koishi.chat/zh-CN/guide/#%E5%BC%80%E5%8F%91%E6%8C%87%E5%8D%97](https://koishi.chat/zh-CN/guide/#%E5%BC%80%E5%8F%91%E6%8C%87%E5%8D%97)

开发指南 [​](#开发指南)
===============

如何阅读本指南 [​](#如何阅读本指南)
---------------------

TIP

本篇指南旨在向有一定 Node.js 开发基础的人介绍 Koishi 的全部知识。如果你只想快速搭建自己的机器人而非学习 Koishi 开发，请前往 [起步](./../manual/starter/) 了解更多安装方式。

Koishi 是一个强大的机器人框架，因此有大量的内容可供学习。不过请不用担心，我们为学习者提供了一部循序渐进的教程，帮助你从最基础的概念出发，逐步掌握关于 Koishi 的一切——运行原理、开发方式和最佳实践。

本篇指南分为了多个章节，每个章节通常围绕一个主题展开。由于许多章节之间存在一定的依赖关系，因此我们建议你按照目录中的顺序阅读本篇指南。当然，每个章节也不必全部读完，你完全可以先产生大致的印象，并在后续的使用中随时回来了解更多的细节。

### 与入门教程的关系 [​](#与入门教程的关系)

TIP

前往 → [入门教程](./../manual/introduction.html)

要想更好地开发 Koishi 插件，我们应当首先了解 Koishi 的功能本身。因此，开发指南中的部分章节会基于入门教程中的前置知识。如果你是第一次接触 Koishi，那么我们推荐你先阅读入门教程，再回到这里学习。就算没有读完入门教程也不必担心：我们会在章节的开头提供相关链接，让你可以快速地了解前置知识。

### 与进阶指南的关系 [​](#与进阶指南的关系)

TIP

前往 → [进阶指南](./../cookbook/)

本篇指南会系统地介绍 Koishi 开发的核心用法，而关于 Koishi 的设计原理和最佳实践则会在进阶指南中进行补充。如果你已经阅读完本篇指南，或是在实际开发中无所适从，相信进阶指南会给你带来更多的帮助。

预备知识 [​](#预备知识)
---------------

Koishi 是一个 Node.js 框架，因此我们假定你已经拥有了一定的 JavaScript 和 Node.js 开发基础。如果你对自己的基础不自信，可以参考下面的两篇教程：

*   [JavaScript 语言概览](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Overview)
*   [现代 JavaScript 教程](https://zh.javascript.info/)

### 关于 TypeScript [​](#关于-typescript)

TypeScript 是 JavaScript 的超集，前者在后者的基础上额外提供了强大的类型系统，可以让你的代码更加健壮，开发也更加快捷。Koishi 本身就是用 TypeScript 编写的，因此我们推荐你使用 TypeScript 来进行 Koishi 开发。如果你对 TypeScript 不熟悉，这里有一篇 [TypeScript 教程](https://www.typescriptlang.org/zh/docs/handbook/typescript-in-5-minutes.html)。

本篇指南中的所有代码示例都使用了 TypeScript。这对于插件开发者来说这并不是必需的。如果你不想用 TypeScript 来开发插件，你可以自行忽略那些类型标注，并使用原生 JavaScript 或其他方言来编写代码。

让我们开始吧！ [​](#让我们开始吧)
--------------------

继续向下滚动，你将在每一页的底部看到前往下一节的链接。

---

