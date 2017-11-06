This is an OpenFaaS plugin for the Serverless Inc framework.

## Were you looking for OpenFaaS?

You are probably looking for [OpenFaaS - openfaas/faas](https://github.com/alexellis/faas).

## serverless-openfaas

### Testing Instructions

#### Prereqs

* NodeJS 6+
* Docker 17.05+
* faas-cli

Get the OpenFaaS CLI:

```
$ curl -sSL https://cli.openfaas.com | sudo sh
```

#### Prepare the environment

###### Get the plugin

```
$ git clone https://github.com/openfaas/serverless-openfaas
$ ./prep.sh
```

###### Test all commands with a script

```
$ ./test-plugin.sh
```

###### Manually test commands

Run `./test-plugin.sh` then:
```
$ cd driver/faas-func
$ sls <command>
```

###### Currently supported commands
```
sls init
sls package
sls deploy
sls deploy function -f <your-function>
sls deploy list
sls invoke -f <your-function> -d <your-data> # -d flag optional
sls remove
```
