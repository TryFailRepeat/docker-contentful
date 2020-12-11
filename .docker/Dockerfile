FROM node:9

# By default, Docker runs container as root which inside of the container can pose as a security issue.
# You would want to run the container as an unprivileged user wherever possible. The node images provide
# the node user for such purpose
USER node

# Global npm dependencies
# If you need to install global npm dependencies, it is recommended to place those dependencies in
# the non-root user directory
RUN mkdir /home/node/.npm-global
ENV PATH=/home/node/.npm-global/bin:$PATH
ENV NPM_CONFIG_PREFIX=/home/node/.npm-global

# installing global packages
RUN npm install contentful-cli -g
RUN npm install contentful-export@6.0.4 -g

WORKDIR /home/node/app

