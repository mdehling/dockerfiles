# Dockerfiles for GitHub Codespaces
To update, enter subdirectory and run, e.g., the following:

    $ docker build -t mdehling/ms-python-extra:1-3.10 .
    $ docker push mdehling/ms-python-extra:1-3.10

The first time, you will have to authenticate with docker:

    $ docker login -u $DOCKER_USER -p $DOCKER_ACCESS_TOKEN

FYI, this is my current build system:

    $ uname -a
    Linux ubuntu 6.2.0-33-generic #33~22.04.1-Ubuntu SMP PREEMPT_DYNAMIC Thu Sep  7 10:33:52 UTC 2 x86_64 x86_64 x86_64 GNU/Linux
    $ docker --version
    Docker version 24.0.5, build 24.0.5-0ubuntu1~22.04.1

