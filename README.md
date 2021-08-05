# BInstall

Currently in DEVELOPMENT

This tool shall provide a simplification to add pre-build binaries into your user space and to
help automate the process into new environments or for new setups.

Stuck working on a corporate environment with very limited abilities to add tools, this here shall
help including pre-build binaries into your user space and adding them to PATH.

You don't need root or compiling (and thus development tools) of packages, but only wget or curl and
some tools for unpacking archives.

## Usage

Setup some environments for convenience

```bash
export BINSTAL_PATH="~/local/bin/folder"
export BINSTAL_FOLDER="~/path/to/download/and/install"
export BINSTAL_REGISTRY="/path/to/binstall/registry"
```

and run 
```bash
# if any source, or bin_name not github-project name
binstall url bin_name
# if github url and bin_name is project-name
binstall url
# if you have an entry in your registry
binstall registry_entry_name
```

## Installation

Clone this Repository somewhere into your system and run `make install` this shall check dependencies
and ask you for input in some parts.

It will most probably also suffice to copy the source code and run ./binstall or put it in path.
Environment variables in use are for convenience, but can be omitted, thus binstall will try to infer
them and fallback to its install\_dir if no other viable solution is found.

## Collaborating

Everybody interested is very welcome to provide feedback, input or pull requests.
For me it is my first publicly shared project and I definitely lack experience and some skills, but
am happy for any collaboration or feedback.

## Credits

I want to mention projects that helped or insipred me:

- [bash3boilerplate](https://bash3boilerplate.sh/) helped and inspired me for my scripting
- [webinstall](https://webinstall.dev/) adresses a similar issue with an interesting approach and
helped me alot already.
