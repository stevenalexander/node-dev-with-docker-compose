# Node development within containers

![BuildStatus](https://travis-ci.org/stevenalexander/node-dev-with-docker-compose.svg?branch=master)

This is a sample solution showing how you can do Node development within docker containers.

Uses [nodemon](https://github.com/remy/nodemon) and volumes that map the host source directories to the app directories in the containers. This means that any changes on the host source cause the container node apps to restart node and take effect. 

This is useful in solutions where you want to use docker-compose for local development, linking the node apps to other containers, but don't want to have to rebuild the containers for all source changes.

For a production version you would need to switch the start script in package.json to use node.
