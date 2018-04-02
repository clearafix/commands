#Kubernetes

kubectl --context mycontext --namespace mynamespace get secrets
kubectl --context mycontext --namespace mynamespace get secret mysecret -o yaml
kubectl --context mycontext --namespace mynamespace create -f ./path/to/yaml/secret/file
kubectl --context mycontext --namespace mynamespace create secret generic ssh-key-secret --from-file=ssh-privatekey=/path/to/.ssh/id_rsa --from-file=ssh-publickey=/path/to/.ssh/id_rsa.pub