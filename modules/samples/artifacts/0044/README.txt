---------------------------------------------
To Test KMeansMiniBatch
---------------------------------------------
1. Copy {WSO2SPHome}/samples/artifacts/0039/steaming-kmeans-minibatch-sample.siddhi file to {WSO2SPHome}/deployment/siddhi-files

2. Copy {WSO2SPHome}/samples/artifacts/0020/kmeans-mini-batch-test.json file to {WSO2SPHome}/deployment/simulation-configs

3. Copy {WSO2SPHome}/samples/artifacts/0039/testKMeansMiniBatch.csv file to {WSO2SPHome}/deployment/csv-files.

4. Start the worker using ./{WSO2SPHome}/bin/worker.sh

5. Run the following curl command to simulate KMeansMiniBatch with events in testKMeansMiniBatch.csv
   curl -X POST http://localhost:9090/simulation/feed/kmeans-mini-batch-test/?action=run

6. See the output in the WSO2SP terminal

---------------------------------------------
To Test KMeansIncremental
---------------------------------------------
1. Copy {WSO2SPHome}/samples/artifacts/0039/steaming-kmeans-incremental-sample.siddhi file to {WSO2SPHome}/deployment/siddhi-files

2. Copy {WSO2SPHome}/samples/artifacts/0020/kmeans-incremental-test.json file to {WSO2SPHome}/deployment/simulation-configs

3. Copy {WSO2SPHome}/samples/artifacts/0039/testKMeansIncremental.csv file to {WSO2SPHome}/deployment/csv-files.

4. Start the worker using ./{WSO2SPHome}/bin/worker.sh

5. Run the following curl command to simulate KMeansMiniBatch with events in testKMeansMiniBatch.csv
   curl -X POST http://localhost:9090/simulation/feed/kmeans-incremental-test/?action=run

6. See the output in the WSO2SP terminal
