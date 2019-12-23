FROM ubuntu

# RUN mkdir /build
WORKDIR /build

# RUN dpkg --add-architecture i386
RUN apt-get update
RUN apt-get install \
    -y \
    git-core \
    gnupg \
    flex \
    bison \
    gperf \
    build-essential \
    zip \
    curl \
    zlib1g-dev \
    lib32z1 \
    lib32ncurses5 \
    x11proto-core-dev \
    libx11-dev \
    libxml-simple-perl \
    libc6-dev \
    libgl1-mesa-dev \
    tofrodos \
    python-markdown \
    libxml2-utils \
    xsltproc \
    chrpath \
    gawk \
    texinfo \
    openjdk-8-jdk \
    python3 \
    python2.7 \
    locales \
    cpio diffstat wget 

RUN ln -sf /bin/bash /bin/sh
# RUN ln -sf /usr/bin/python3 /usr/bin/python

RUN locale-gen en_US.UTF-8
RUN update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
ENV LANG en_US.UTF-8

RUN useradd -c 'Non-root user' -m -d /home/lime -s /bin/bash lime
RUN chown -R lime.lime /build
USER lime
ENV HOME /home/lime

# RUN touch /build/poky/build/conf/sanity.conf

# COPY . .
# ENV TARGET_TYPE scooter
# CMD ["/bin/bash", "-c", "make"]