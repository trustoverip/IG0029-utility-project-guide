# Copyright (c) 2020 ToIP Foundation

# Pull base image from official Material for MkDocs repo
FROM squidfunk/mkdocs-material

# Add bash as alternative to default ash shell env in Alpine
RUN apk add --no-cache --upgrade bash python3 py-pip

# Add make command utility
RUN apk add --update --no-cache make=4.3-r0

# Add MkDocs dependencies
RUN pip install --upgrade pip
RUN pip install --upgrade mkdocs-enumerate-headings-plugin

# Set working directory to the name of a Docker Volume
WORKDIR /host_mkdocs
