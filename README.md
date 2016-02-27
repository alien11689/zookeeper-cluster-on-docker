Example of cluster of Zookeepers
================================

To start cluster, enter command:

```sh
$ docker-compose up
```

Clients could connect to cluster via `localhost` on ports `2181`, `2182` and `2183`.

`dockcer-compose` assumes, that your IP of your `docker0` interface is `172.17.0.1`. You could check it via command `ip addr show docker0`.

To test cluster run dockers one by one (in separate consoles or use `-d` option):

```sh
$ docker-compose up zookeeper1
$ docker-compose up zookeeper2
$ docker-compose up zookeeper3
```

and play.
