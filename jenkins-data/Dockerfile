FROM debian:jessie

MAINTAINER lev epshtein

RUN mkdir -p /var/jenkins_home
RUN useradd -d /var/jenkins -u 1000 -m -s /bin/bash jenkins
RUN mkdir -p /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins
VOLUME ["/var/log/jekins","/var/jenkins_home"]

USER jenkins
CMD ["echo", "Data container for Jenkins"]
