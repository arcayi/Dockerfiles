FROM ubuntu

# RUN mkdir /build
WORKDIR /build

RUN dpkg --add-architecture i386
RUN apt-get update
RUN apt-get install \
    gcc-arm-linux-gnueabi \
    g++-arm-linux-gnueabi \
    build-essential \
    libffi-dev\
    -y

# COPY . .
ENV TARGET_TYPE scooter
CMD ["/bin/bash", "-c", "make"]