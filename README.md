# devpod-try-go-vscode
Build a devpod with go image and VS Code as the IDE. 

## Prerequisites
- [Docker](https://docs.docker.com/get-docker/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [DevPod](https://devpod.sh) (Optional, but recommended)

## Steps

1. Set your devpod provider to `docker`
```devpod provider docker```

2. Verify your devpod provider
```devpod provider list```

3. Create a new devpod with the go image
```devpod up https://github.com/beckitrue/devpod-try-go-vscode --ide code```

4. VS Code will open.

### Advanced Steps

Some options you may want to set for your devpod:

1. Set your `dotfiles` URL
```devpod context set-options DOTFILES_URL <URL>```

2. Inject Git credentials into your devpod workspace
```devpod context set-options -o SSH_INJECT_GIT_CREDENTIALS=<true|false>```

3. Inject Docker credentials into your devpod workspa
```devpod context set-options -o SSH_INJECT_DOCKER_CREDENTIALS=<true|false>```

4. For a full list of options, and to veryify your context option settings:
```devpod context options```


## Next Steps
- You can use the terminal in VS Code to clone your own repository and start coding. 
- You can configure your `.devcontainer.json` file to customize your devpod and VS Code settings.
- You can use your `.devcontainer.json` file to install additional tools and extensions.
- You can use your `.devcontainer.json` file to clone repos and run scripts on start up.
