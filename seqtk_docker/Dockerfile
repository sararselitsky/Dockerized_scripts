FROM ubuntu:18.04
# Metadata
LABEL software="Seqtk"
LABEL description="Seqtk docker, able to subset FASTQs"
LABEL maintainer="sararselitsky@gmail.com"

# update the OS related packages
RUN DEBIAN_FRONTEND=noninteractive \
    TZ=America/Detroit \
    apt-get update && apt-get install -y \
    build-essential \
    cmake \
    gcc-8-base \
    libz-dev \
    git



RUN git clone https://github.com/lh3/seqtk.git
WORKDIR seqtk
RUN make
