FROM ubuntu:20.04

ENV ANSIBLE_HOST_KEY_CHECKING False

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN apt-add-repository ppa:ansible/ansible

RUN apt-get update
RUN apt-get install -y ansible

# sshpass (Able to run $ansible-playbook -i inventry.ini playbook.yml --ask-pass)
RUN apt-get install sshpass

CMD /bin/bash

# docker exec -it keisoku-ansible bash
# ansible-playbook -i inventry.ini playbook.yml --ask-pass


# Vim
RUN echo y | apt-get install vim