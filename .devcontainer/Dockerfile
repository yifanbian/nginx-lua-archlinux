FROM archlinux:latest

RUN pacman -Syyu --noconfirm base-devel sudo bash-completion nano git

# Add defualt user
RUN useradd vscode \
 && mkdir -p /home/vscode \
 && chown -R vscode:vscode /home/vscode/ \
 && usermod -aG wheel vscode \
 && echo 'root:1234' | chpasswd \
 && echo 'vscode:1234' | chpasswd \
 && echo 'vscode ALL=(ALL:ALL) NOPASSWD: ALL' | tee /etc/sudoers


# Set default user
USER vscode