# home-assistant-docker
smartthings integration with home assistant running on qnap notes

Run MQTT
```

docker run \
    -d \
    --name="mqtt" \
    -v /opt/mosca:/db \
    -p 1883:1883 \
    matteocollina/mosca
    
    
docker run \
-d \
--name="mqtt-bridge" \
-v /opt/mqtt-bridge:/config \
-p 8080:8080 \
stjohnjohnson/smartthings-mqtt-bridge


```
