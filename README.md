# OpenHAB Config and Support Tools

## /yamlcomposer

A collection of configuration packages and templates built for **openHAB 5.3+**, designed to standardize and make the deployment of identical device models **easily replicable**.

### Core Philosophy

Rather than manually configuring every single sensor or actuator, this repository enforces a **template-driven, standardized structure**:
* **Structural Consistency**: Every instance of the same device model follows identical naming conventions for Things, Channels, Items, and metadata.
* **Plug-and-Play Replicability**: Adding a new unit of an existing device model only requires cloning its package/template import and replacing the unique device properties (e.g., MQTT topic, IP address, or device ID).

### Configuration Examples

Inside the repository folders, you will find sample configuration files ('*-example.yml') based on my use cases. You can use them as a quick reference to:
* Understand the standard structure for variables.
* Easily clone the logical structure when deploying a new unit of the same model.

### Prerequisites

* **openHAB 5.3+**

## /backup-script/oh4-full-backup.sh

Backup script for OpenHAB and Influxdb 2 (running on docker).

**Credit to oliranks https://github.com/oliranks/openHAB3-full_backup_and_restore**

For remote copy to work (using SCP), you have to copy ssh key from RPI to NAS, using ssh-copy-id script. See https://www.ssh.com/academy/ssh/copy-id

## /pages

Yml source code for my pages

### ./tablet1

My main control panel running on an Android wall-mounted tablet with HabPabelViewer