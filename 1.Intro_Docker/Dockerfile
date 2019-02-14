FROM ubuntu:18.04
RUN apt-get update && apt-get install wget cowsay -y
RUN wget https://raw.githubusercontent.com/performantpro/hce_demo/master/1.Intro_Docker/docker.hon -O /usr/share/cowsay/cows/docker.hon
RUN rm -f /usr/share/cowsay/cows/default.cow
RUN ln -sv /usr/share/cowsay/cows/docker.hon /usr/share/cowsay/cows/default.cow
ENTRYPOINT ["/usr/games/cowsay"]
