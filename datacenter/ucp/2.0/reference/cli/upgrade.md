---
description: Upgrade the UCP components on this node
keywords: docker, dtr, cli, upgrade
title: docker/ucp upgrade
---

Upgrade the UCP components on this node

## Usage

```bash
docker run -it --rm docker/ucp \
  upgrade [command options]

```

## Description

This commands upgrades the UCP running on this node.
To upgrade UCP:

* Upgrade the Docker Engine in all nodes (optional)
* Run the upgrade command in all manager nodes
* Run the upgrade command in all worker nodes

After upgrading UCP in a node, go to the UCP web UI and confirm the node is
healthy, before upgrading other nodes.


## Options

| Option                    | Description                |
|:--------------------------|:---------------------------|
|`--debug, D`|Enable debug mode|
|`--jsonlog`|Produce json formatted output for easier parsing|
|`--interactive, i`|Run in interactive mode and prompt for configuration values|
|`--admin-username`|The UCP administrator username|
|`--admin-password`|The UCP administrator password|
|`--pull`|Pull UCP images: 'always', when 'missing', or 'never'|
|`--registry-username`|Username to use when pulling images|
|`--registry-password`|Password to use when pulling images|
|`--id`|The ID of the UCP instance to upgrade|
|`--host-address`|Override the previously configured host address with this IP or network interface|
