FROM ubuntu:18.04
WORKDIR /home
COPY agent.jar .
RUN apt-get update && apt-get install -y curl openjdk-11-jdk git maven docker.io
RUN adduser  --disabled-password --gecos "" jenkins
#ENTRYPOINT java -jar agent.jar -jnlpUrl ${NODE_URL}/jenkins-agent.jnlp -secret ${SECRET} -workDir "/home/"


