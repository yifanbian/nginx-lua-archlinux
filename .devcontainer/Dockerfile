FROM archlinux:latest

RUN pacman -Syyu --noconfirm build-devel sudo bash-completion nano git

# Add defualt user
RUN useradd vscode \
 && mkdir -p /home/vscode \
 && chown -R vscode:vscode /home/vscode/ \
 && usermod -aG wheel vscode

# Set default user
USER vscode