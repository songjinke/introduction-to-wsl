# Introduction to WSL
The WSL (Windows Subsystem for Linux) lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.

The big benefit is that developers can access the power of both Windows and Linux at the same time on a Windows machine.

## Documents
- [Overview](https://learn.microsoft.com/en-us/windows/wsl/about)
- [Install](https://learn.microsoft.com/en-us/windows/wsl/install)

## Tips
- WSL 2 is recommended ([details](https://learn.microsoft.com/en-us/windows/wsl/compare-versions#whats-new-in-wsl-2)), run `wsl --set-default-version 2` after the installation.
- Visual Studio Code is recommended ([details](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode)).
- nvm is recommended for node version manager ([details](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-wsl#install-nvm-nodejs-and-npm)). And in case you encouter issues with nvm like me, n is recommended ([alternative version managers](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-wsl#alternative-version-managers)). Here is a tip for n to auto switch node version: [link](https://github.com/tj/n/issues/714#issuecomment-1062172970).
- In case you encouter internet connectivity issues behind corporate proxy like me, here is a tip to fix it: [link](https://gist.github.com/mandeepsmagh/f1d062fc59e4e6115385c2609b5f0448).
- In case you want to customize domains instead of using `localhost` ([details](https://learn.microsoft.com/en-us/windows/wsl/networking#accessing-linux-networking-apps-from-windows-localhost)) during development, you can modify the hosts file in WSL, install Google Chrome in WSL, and launch it from WSL.

## Demo
- Set Auto Attach to Always in Visual Studio Code ([details](https://code.visualstudio.com/docs/nodejs/nodejs-debugging#_auto-attach)).
- 
    ```sh
    npm install
    npm run dev
    ```
- Add a breakpoint and debug server side code.