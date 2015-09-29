container.deploy
=========

This Ansible role will deploy a list of containers to a server.

Requirements
------------


Role Variables
--------------
docker_registry = URL of the Docker registry.
container_image = The container image name to pull from the registry. (ex. `docker pull 'mysql'` <- container_image)
container_name = What to name the container after it has been pulled locally.  (ex. `docker run --name 'yourmysql'` <- container_name)
internal_docker_port: Internal Docker port to map to an external port on the server.
external_server_port: External port on the server that exposes the internal port for the container.

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GNU General Public License v2.0

Author Information
------------------

Chris Livermore

[@e30chris](https://twitter.com/e30chris)

[Sandors Systems Scribbles](http://sandorsscribbl.es/)
