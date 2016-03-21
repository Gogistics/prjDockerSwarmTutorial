###Configuration of IPFS with Docker

1. access the virtual machine via ssh

2. create your working dir

$ mkdir -p /tmp/ipfs_docker_staging && mkdir -p /tmp/ipfs_docker_data

$ docker run -d --name ipfs_node_1 -v /tmp/ipfs_docker_staging:/export -v /tmp/ipfs_docker_data:/data/ipfs -p 5050:5050 -p 4001:4001 -p 127.0.0.1:5001:5001 jbenet/go-ipfs:latest