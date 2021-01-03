FROM kalilinux/kali-rolling

RUN apt-get update && \
  apt-get install -y \
  gcc \
  gdb \
  git && \
  git clone https://github.com/longld/peda.git /peda && \
  echo "source /peda/peda.py" >> ~/.gdbinit \
  metasploit-framework

CMD tail -f /dev/null
