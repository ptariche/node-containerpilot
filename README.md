# node-containerpilot

Node + [containerpilot](https://www.joyent.com/containerpilot) docker images for bootstrapping your [autopiloted](https://www.joyent.com/blog/applications-on-autopilot) apps

[**Dockerhub Link**](https://hub.docker.com/r/ptariche/node-containerpilot/)

**Usage:**
```
FROM ptariche/node-containerpilot:[NODE_VERSION]:[CONTAINERPILOT_VERSION]

COPY /path/to/app/source /path/to/app/source

COPY /path/to/yourcontainerpilot.json /etc/containerpilot.json
# OR
ENV CONTAINERPILOT=file:///path/to/your/containerpilot.json

CMD ["containerpilot", "node", "/path/to/app/source"]
```
