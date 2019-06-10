# :zap: Zap Starter Kit :zap:
This repository is a starter kit for anyone who wishes to build using the Zap.org layer 3 blockchain framework.

```bash
Zap@linux $ sudo apt-get update
Zap@linux $  sudo apt-get install -y build-essential libssl-dev curl git-core python
Zap@linux $  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```



```bash

Zap@linux $ exec bash
Zap@linux $ export NVM_DIR="${XDG_CONFIG_HOME/:-$HOME/.}nvm"
Zap@linux $ [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
Zap@linux $ exec bash
```

Now that you have your environmental variables set up you can install a version of nodejs and npm.
I suggest you use 10.15.3 for this install because I have tested at length, but any should work.



```bash
Zap@linux $ nvm install 10.15.3
```
After your install check to make sure your nvm is set up properly by checking the versions of node and npm by entering node -v and npm -v in your terminal

```bash
Zap@linux $ node -v 
Zap@linux $ npm -v
```
ok just one more step here to getting Zap-term up and running...


```bash
Zap@linux $ node -g lerna typescript
Zap@linux $ npm install -g truffle ganache-cli
Zap@linux $ npm install -g zap-term
Zap@linux $ exec bash
Zap@linux $ zap-term
```
After waiting for the install scripts to finish and punching in zap-term you should have a couple options mainly to use kovan or mainnet! If you have finished this congratulations! you have finished the first tutorial lets try and do more advanced things in step two!
