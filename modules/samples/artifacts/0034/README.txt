Purpose of this sample is to test the functionality of sentiment extension in SP 4.0.0

1. Copy {WSO2SPHome}/samples/artifacts/0034/priorityExtensionSample.siddhi file to {WSO2SPHome}/deployment/siddhi-files

2. Start the worker using ./{WSO2SPHome}/bin/worker.sh

3. Run following curls commands to send some login events

curl -X POST \
  http://localhost:9090/simulation/single \
  -H 'content-type: text/plain' \
  -d '{
  "siddhiAppName": "priorityExtensionSample",
  "streamName": "userWallPostStream",
  "timestamp": null,
  "data": [
    "Mohan",
    "Hello World!",
    "1"
  ]
}'


curl -X POST \
  http://localhost:9090/simulation/single \
  -H 'content-type: text/plain' \
  -d '{
  "siddhiAppName": "priorityExtensionSample",
  "streamName": "userWallPostStream",
  "timestamp": null,
  "data": [
    "Nuwan",
    "Good Morning!",
    "3"
  ]
}'

4. See the output in the WSO2SP terminal
