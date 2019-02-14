FROM ubuntu:18.04
RUN apt-get update && apt-get install cowsay -y
COPY cowsay /usr/local/bin/cowsay
COPY docker.hon /usr/local/share/cows/
RUN ln -sv /usr/local/share/cows/docker.hon /usr/local/share/cows/default.cow
ENTRYPOINT ["/usr/local/bin/cowsay"]
