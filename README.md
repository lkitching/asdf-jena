#asdf-jena
[Apache Jena](https://jena.apache.org/) plugin for [asdf](https://asdf-vm.com/). This plugin manages only the tools, to manage
Fuseki versions, see the [asdf Fuseki plugin](https://github.com/lkitching/asdf-fuseki).

## Install
Ensure [asdf](https://asdf-vm.com/) is installed and then install the plugin with

```bash
asdf plugin add jena https://github.com/lkitching/asdf-jena.git
```

## Usage
Once installed the plugin can be used via asdf to list and install available versions of the tools e.g.

```bash
asdf list all jena
asdf install 3.4.0
```

The plugin exports the executables in the `bin` directory of the jena distribution. If the adsf shims directory is on your `PATH`
these will be available e.g.

```
tdbloader --loc /path/to/database input.ttl
```