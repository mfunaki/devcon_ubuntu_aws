FROM mcr.microsoft.com/devcontainers/base:jammy

# Allow GPG signing from inside of a container
RUN apt-get update && apt-get install gnupg2 -y

# Install awscliv2
RUN curl -sL https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip -o awscliv2.zip
RUN unzip -q awscliv2.zip
RUN ./aws/install
RUN rm awscliv2.zip
RUN rm -rf ./aws
