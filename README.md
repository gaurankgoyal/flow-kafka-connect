# flow-kafka-connect

This repo conatines the JDBC sink properties for the flow Project.

There are 2 folders in this repositories:-

# jdbc-sink-connector-config-json

conatines the files in json format

# jdbc-sink-connector-config-properties

containes the files in properties format

# How to Deploy?
In order to deploy below command needs to be run (localhost need to be change with DNS name of the server in case if these are being deployed remotly)

curl -X POST -d @ods-item-loc-soh-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-item-loc-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-code-detail-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-sa-store-day-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-sa-tran-head-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-sa-tran-item-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-sa-tran-igtax-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"

curl -X POST -d @ods-sa-tran-disc-sink.json http://localhost:8084/connectors --header "Content-Type:application/json" --header "Accept:application/json"


# How to Test?
curl localhost:8084/connectors/ods-item-loc-soh-sink/status

curl localhost:8084/connectors/ods-item-loc-sink/status

curl localhost:8084/connectors/ods-code-detail-sink/status

curl localhost:8084/connectors/ods-sa-store-day-sink/status

curl localhost:8084/connectors/ods-sa-tran-head-sink/status

curl localhost:8084/connectors/ods-sa-tran-item-sink/status

curl localhost:8084/connectors/ods-sa-tran-igtax-sink/status

curl localhost:8084/connectors/ods-sa-tran-disc-sink/status

