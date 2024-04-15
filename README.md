# coding-project-template

# cd /home/project/ibm-fullstack_developer_capstone/server/database
docker build . -t us.icr.io/sn-labs-oyesinaoyedu/senti_analyzer
docker push us.icr.io/sn-labs-oyesinaoyedu/senti_analyzer
ibmcloud ce application create --name sentianalyzer --image us.icr.io/sn-labs-oyesinaoyedu/senti_analyzer --registry-secret icr-secret --port 5000