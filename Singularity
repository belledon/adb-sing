bootstrap: docker
from: ubuntu:16.04

%environment

  export PATH="/src/platform-tools:$PATH"

%post
  apt-get update && apt-get -y install locales
  locale-gen en_US.UTF-8

  apt-get install -y wget unzip

  mkdir /src && cd /src
  wget https://dl.google.com/android/repository/platform-tools-latest-linux.zip
  unzip platform-tools-latest-linux.zip && rm platform-tools-latest-linux.zip
