# ipfs-sync

Script to sync files from one IPFS node to another.

## Install

```sh
git clone https://github.com/ProjectTwelve/ipfs-sync.git
```

## Usage

Transfer _all_ files from one IPFS node to another:

```sh
./bin/ipfs-sync sync-files --from <URL> --to <URL> [--skip-existing]
```

Note: It support http basic auth in URL


Transfer only specific files from one IPFS node to another:

```sh
./bin/ipfs-sync sync-files --from <URL> --to <URL> --file-list <FILE> [--skip-existing]
```

In this case, `<FILE>` has to be a file with one IPFS hash per line for each
file that should be synced from the `--from` node to the `--to` node.

