# bengland/fedora:28 includes git and any other packages that we use
FROM docker.io/fedora:28
MAINTAINER Ben England <bengland@redhat.com>
RUN dnf install -y python2 git
RUN git clone https://github.com/distributed-system-analysis/smallfile
RUN ln -sv /smallfile/smallfile_remote.py /usr/local/bin
COPY launch.sh /
CMD /launch.sh
