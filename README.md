# node-containerpilot

Node + [containerpilot](joyent.com/containerpilot) docker images for bootstrapping your [autopiloted](joyent.com/blog/applications-on-autopilot) apps

[**Dockerhub Link**](https://hub.docker.com/r/johnhof/node-containerpilot/)

**Usage:**
```
FROM johnhof/node-containerpilot:[NODE_VERSION]:[CONTAINERPILOT_VERSION]

COPY /path/to/app/source /path/to/app/source

COPY /path/to/yourcontainerpilot.json /etc/containerpilot.json
# OR
ENV CONTAINERPILOT=file:///path/to/your/containerpilot.json

CMD ["containerpilot", "node", "/path/to/app/source"]
```
