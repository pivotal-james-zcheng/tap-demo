1. Install kubectl, docker
2. Set up kube config and change current namespace to delta
```
kubectl config set-context --current --namespace=delta
```
4. Harbor login
```
docker login harbor.services.tanzu -u 'robot$workshop+labs-sg'
```
4. Install TAP CLI
```
cd ~/Downloads/cli
export TANZU_CLI_NO_INIT=true
install core/v*/tanzu-core-darwin_amd64 /usr/local/bin/tanzu
tanzu plugin install --local . all
```
5. Install tilt from brew
```
curl -fsSL https://raw.githubusercontent.com/tilt-dev/tilt/master/scripts/install.sh | bash
```
6. Install Intellij (version 222) with Tanzu plugin
7. Use Java 17. Add the following to .zshrc
```
export JAVA_HOME=`/usr/libexec/java_home -v 17`
```
