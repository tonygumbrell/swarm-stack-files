# swarm-stack-files

This repo hosts the details for running MISP and TheHive project docker images within a docker swarm for an enterprise deployment, whereby the 5 containers run on a common overlay network so that integration is possible.

The swarm nodes require common data volumes (ie shared data via NFS / SAN / NAS) so that application specific data can be written to regardless of the node the container is active on. This also provides a level of high availability.

The regular MISP and Hive compose files found within the core project have been uplifted to version 3 yaml files and all depracated flags removed. 

The images are hosted on a local registry server so it will function within an air-gapped infrastructure and this is exampled within the compose files.


