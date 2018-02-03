# StarCorp VBox

The scripts that build the StarCorp VBox development environment.

## Usage

You probably don't want this repo.

* Clone [chef/bento](https://github.com/chef/bento) into same top level folder as this repo.
* Run `./bin/copy-to-bento.sh`
* Replace `scripts/cleanup.sh` with `scripts/server.sh` in file `ubuntu/ubuntu-16.04-amd64.json`
* Follow normal [Packer](https://www.packer.io/) practice of building `ubuntu/ubuntu-16.04-amd64.json`
* Run `./packer build -only=virtualbox-iso ubuntu-16.04-amd64.json` in folder `chef/bento/ubuntu`
