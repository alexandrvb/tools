FROM ubuntu:20.04

ARG TERRAFORM_VERSION

RUN apt-get update && apt-get -y install wget unzip && rm -rf /var/lib/apt/lists/*

RUN wget https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip && \
    unzip terraform_${TERRAFORM_VERSION}_linux_amd64.zip && \
    mv terraform /usr/local/bin/ && \
    rm -rf terraform_${TERRAFORM_VERSION}_linux_amd64.zip
