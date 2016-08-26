# MQTT Docker Publisher

An MQTT Docker publisher for the BigBoat ecosystem.

## How to run

    docker run \
      -e DOCKER_HOST=tcp://dockerhost:2375 \
      -e MQTT_URL=mqtt://mqttserver \
      -e MQTT_TOPIC_NS=/docker \
      --name docker-publisher
      ictu/bigboat-docker-publisher

## Contributing

If you want to contribute please fork the repo and submit a pull request in
order to get your changes merged into the main branch.

### Development

Below you find an example of how to run the agent for development.

    #!/bin/bash

    DOCKER_HOST=tcp://dockerhost:2375 \
    MQTT_URL=mqtt://mqttserver \
    MQTT_TOPIC_NS=/docker \
    nodemon index.coffee
