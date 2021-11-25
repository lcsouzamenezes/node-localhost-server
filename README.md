# Node.js Localhost Server
> A Node.js server for localhost environment.

<br>

## Dependencies

1. [Node.js](https://nodejs.org/en/download/)
2. [npm](https://www.npmjs.com/get-npm)

<br>

## Installation

```sh
cd node-localhost-server
npm install
```

<br>

## Configuration

Inside the root directory, there is a directory named **projects**. This directory is where you will put all your projects.

You can still configure vhosts (see `server.js` with examples). Don't forget to configure your **hosts** file like:

```sh
# LOCALHOST
127.0.0.1 example.com example.com.br
```

### Problems with ports

If you have some problems with ports on **Linux**, you can run:

```sh
# Enable your user to run node apps on the default HTTP port (80)
sudo apt-get install libcap2-bin
sudo setcap cap_net_bind_service=+ep `readlink -f \`which node\``
```

<br>

## Commands

#### Run
```sh
npm run start
# localhost listening using ports 80 and 443
```

#### List
```sh
npm run list
```

#### Stop
```sh
npm run stop
```

<br>

## References

* [Vhost com NodeJS e Express](https://www.youtube.com/watch?v=GV3hWa5VIQg)
* [PM2](http://pm2.keymetrics.io/)
