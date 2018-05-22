# docker-wscat

### As a binary alias

```sh
alias wscat='docker run -it --rm --net=host monotykamary/wscat'
```

### Execute on Docker

```sh
sudo docker run -it --rm --net=host monotykamary/wscat -- -c ws://echo.websocket.org
```

### Execute on Kubernetes

```sh
kubectl run --rm -i --tty wscat --image=monotykamary/wscat --restart=Never -- -c ws://echo.websocket.org
```

### Execute on Openshift

```sh
oc run --rm -i --tty wscat --image=monotykamary/wscat --restart=Never -- -c ws://echo.websocket.org
```
