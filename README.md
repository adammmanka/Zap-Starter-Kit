![Zap.org Logo](https://zap.org/img/logos/official.png "Zap.org")
# :zap: Zap Starter Kit :zap:
This repository is a starter kit for anyone who wishes to build layer 3 blockchain technologies using the Zap.org blockchain agnostic framework.


##Linux
Zap development will require a few different packages `git-core` `python` `build-essential` `curl` and a few others. We also use `nvm` in this tutorial to ensure no errors occur. 

```bash
Zap@linux $ sudo apt-get update
Zap@linux $  sudo apt-get install -y build-essential libssl-dev curl git-core python
Zap@linux $  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
After the packages install the curl command will call an install script for nvm.
Then we need to refresh the terminal and export an Environmental Variable to our .bashrc file we do this by running the commands below. 


```bash
Zap@linux $ exec bash
Zap@linux $ export NVM_DIR="${XDG_CONFIG_HOME/:-$HOME/.}nvm"
Zap@linux $ [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
Zap@linux $ exec bash
```

Now that you have your environmental variables set up you can install a version of nodejs and npm.
I suggest you use 10.15.3 for this install because I have tested at length, but any should work.
**If you like to check out the other available versions of 'node' enter in the command `nvm ls-remote` wouldn't recommend unless you know what you are doing`


```bash
Zap@linux $ nvm install 10.15.3
```
After your install check to make sure your nvm is set up properly by checking the versions of node and npm by entering node -v and npm -v in your terminal

```bash
Zap@linux $ node -v 
Zap@linux $ npm -v
```
Ok just one more step here to getting Zap-term up and running, lets install some global packages to npm so we can run our zap-term tool and start building oracles!



```bash
Zap@linux $ node -g lerna typescript
Zap@linux $ npm install -g truffle ganache-cli
Zap@linux $ npm install -g zap-term
Zap@linux $ exec bash
```
After waiting for the install scripts to finish type `zap-term` into your shell!

```bash
Zap@linux $ zap-term
```


You should have a couple options mainly to use kovan or mainnet! If you have finished this congratulations! you have finished the first tutorial lets try more advanced things in step two!



 :tada:  :tada:  :tada:  :tada: Congrats on running zap-term! we are one step closer to making you a layer 3 blockchain dev!  :tada:  :tada:  :tada:  :tada: 
