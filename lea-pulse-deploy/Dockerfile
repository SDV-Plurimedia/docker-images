FROM node:9.8.0

# Update sources.list for yarn usage
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" > /etc/apt/sources.list.d/yarn.list

# Sources update + installation for : jq, curl, apt-transport-https, yarn, openssh-client
RUN apt-get update && apt-get install jq curl apt-transport-https yarn openssh-client -y 
