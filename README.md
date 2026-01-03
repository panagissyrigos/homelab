# Homelab

Homelab projects and adventures.

* The default_software.yml contains all the default software I deploy to every host in my homelab.

* docker-trixie.yml contains the necessary packages and installation steps specifically for Debian 13 (trixie). 

* docker-swarm.yml initializes a swarm environment within docker.

* docker-services.yml sets up an environment with a custom home folder for docker, and deploys the necessary services, such as glusterfs (for shared data between the hosts), portainer (for installation, and management of services across the swarm).

* ansible.cfg contains the configuration options to make ansible work the way I want it to work.

* hosts contains a list of all the hosts and the roles they fulfill.

* updates.yml performs updates, upgrades and autoclean (via apt) to all the hosts.

* bitwarden.yml deploys a bitwarden-lite service in the swarm. It includes a supported version of mariadb.

* vscode.yml deploys vscode to specific hosts (I have 2 linux laptops that have a GUI and if I have to reload any of the hosts, I deploy it during installation) It uses the vsdefs.yml and vsvars.yml.

* msedge.yml it deploys Microsoft's Edge browser to specific hosts

* powershell.yml deploys Powershell to the specific hosts.