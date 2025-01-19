# devpod-devcontainer-labs

This is an introductory devcontainer lab. Our goal is to learn about devcontainers, how to use them, and how to customize them.

We are using DevPod to make this introduction easier and faster for the participants. DevPod is a tool that allows you to create and manage devcontainers without having to know everything about the underlying technology.

After completing this lab, you will have a better understanding of how to use devcontainers and how to customize them to fit your needs.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [DevPod](https://devpod.sh/docs/getting-started/install#install-devpod)

## IDEs
- [Visual Studio Code](https://code.visualstudio.com/)
- [JetBrains](https://www.jetbrains.com/) and [JetBrains Gateway](https://www.jetbrains.com/remote-development/gateway/) (Optional) 

Other IDEs are supported, but this lab will use VS Code and IntelliJ as examples. For example, if you want to run a fully configured [Neovim](https://neovim.io/) devcontainer, you can use the following image link: [devpod-neovim](https://github.com/beckitrue/devpod-neovim)


## CLI instructions to create a DevPod Workspace with VS Code 

1. Set your devpod provider to Docker
```devpod provider docker```

2. Verify your devpod provider
```devpod provider list```

3. Set your IDE to `vscode` 
```devpod ide use vscode```

3. Create a new devpod with one of the quick start images below
```devpod up <image link>```

4. VS Code will open

### Image Links

Copy the image link to use in step 3 above. You can also use these links to create a Github Codespace.

- [Go](https://github.com/microsoft/vscode-remote-try-go)
- [Python](https://github.com/microsoft/vscode-remote-try-python)
- [Node JS](https://github.com/microsoft/vscode-remote-try-node)
- [Java](https://github.com/microsoft/vscode-remote-try-java)
- [Rust](https://github.com/microsoft/vscode-remote-try-rust)
- [Dotnet](https://github.com/microsoft/vscode-remote-try-dotnet)
- [C++](https://github.com/microsoft/vscode-remote-try-cpp)

### Quick Start Image Links

Use these links if you want to use the DevPod Desktop instead of the CLI to create a new workspace. Clicking on the link will open your DevPod Desktop and create a new workspace with the selected image.

- [Go](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-go)
- [Python](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-python)
- [Node JS](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-node)
- [Java](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-java)
- [Rust](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-rust)
- [Dotnet](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-dotnet)
- [C++](https://devpod.sh/open#https://github.com/microsoft/vscode-remote-try-cpp)

### Advanced Configuration Steps

Some options you may want to set for your [DevPod Workspace](https://devpod.sh/docs/developing-in-workspaces):

1. Set your `dotfiles` URL
```devpod context set-options DOTFILES_URL <Your dotfiles URL>```

2. Inject Git credentials into your devpod workspace
```devpod context set-options -o SSH_INJECT_GIT_CREDENTIALS=<true|false>```

3. Inject Docker credentials into your devpod workspa
```devpod context set-options -o SSH_INJECT_DOCKER_CREDENTIALS=<true|false>```
4. For a full list of options, and to veryify your context option settings:
```devpod context options```


## Next Steps to Try

- Use the terminal in VS Code to clone your own repository and start coding 
- Add a [startup script](https://devpod.sh/docs/developing-in-workspaces/dotfiles-in-a-workspace) to your `dotfiles` repository to clone your repositories and run your setup scripts
- Make a copy of the provided `.devcontainer.json` and modify it to customize your devcontainer and [IDE settings](https://code.visualstudio.com/docs/devcontainers/containers#_dev-container-features)
- Configure your `.devcontainer.json` file to install additional tools ([Features](https://containers.dev/features))
- Try using the [JetBrains IDE](https://devpod.sh/docs/getting-started/quickstart-jetbrains) with the devcontainer
- See what other IDEs are supported by DevPod and try one that you use ```devpod ide list```
-
## Resources

- [DevPod Quickstart Documentation](https://devpod.sh/docs/getting-started/quickstart)
- [DevPod Documentation](https://devpod.sh/docs/)
- [VS Code Remote Development](https://code.visualstudio.com/docs/remote/remote-overview)
- [JetBrains cutomizing devcontainer](https://www.jetbrains.com/help/idea/customizing-devcontainer-json-file.html)
- [Devcontainer Available Feautres](https://containers.dev/features)
- [Devcontainer Specification](https://containers.dev/implementors/spec/)
- [DevPod Providers Documentation](https://devpod.sh/docs/managing-providers/add-provider)

