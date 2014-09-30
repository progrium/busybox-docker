# progrium/docker

32 MB container with the Docker binary. Pass it a socket and use Docker inside Docker.

## Example

	$ docker run -d -v /var/run/docker.sock:/var/run/docker.sock progrium/docker \
		/bin/sh -c 'docker rmi $(docker images -q -f dangling=true)'


## License

BSD