FROM fedora:46

# git

RUN dnf install -y git

# setup claude code

COPY claude/claude-code.repo /etc/yum.repos.d/claude-code.repo

RUN dnf install -y claude-code

# setup user
RUN useradd -u 1000 -m ai
WORKDIR /home/ai
USER ai
