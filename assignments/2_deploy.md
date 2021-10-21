kcf run demoapp --image=registry.hub.docker.com/hansimais/demoapp --port=8080 
<!-- --command -- make start -->
kcf delete pod demoapp

<!-- docker run -ti registry.hub.docker.com/hansimais/demoapp -->

kcf describe pods demoapp

kcf get pod demoapp --template='{{(index (index .spec.containers 0).ports 0).containerPort}}{{"\n"}}'
<!-- i'm still using 8080 local -->
kcf port-forward --address 127.0.0.1 demoapp 8088:8080