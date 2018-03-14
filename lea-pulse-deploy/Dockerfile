FROM node:9.8.0

# Sources update + installation for curl
RUN apt-get update && apt-get install curl -y

# Update sources.list for yarn usage
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" > /etc/apt/sources.list.d/yarn.list

# Sources update + installation for : jq, apt-transport-https, yarn, openssh-client
RUN apt-get update && apt-get install jq apt-transport-https yarn openssh-client -y 
