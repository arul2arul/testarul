FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu

# Install Docker CE CLI
RUN apt-get update && apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common lsb-release
RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -
RUN add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
RUN apt-get update && apt-get install -y docker-ce-cli

# Install Azure CLI
RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash