### 1. Install TAP CLI
```
cd ~/Downloads/cli
export TANZU_CLI_NO_INIT=true
install core/v*/tanzu-core-darwin_amd64 /usr/local/bin/tanzu
tanzu plugin install --local . all
```

### 2. Harbor login
> docker login harbor.services -u 
