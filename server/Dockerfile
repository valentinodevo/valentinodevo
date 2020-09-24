### Using image with installed netcat
FROM ubuntu-upstart:utopic

COPY server.sh /home/server/

CMD ["80","Test-OK"]

ENTRYPOINT ["/bin/bash", "/home/server/server.sh"]
