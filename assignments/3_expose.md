https://docs.digitalocean.com/products/kubernetes/how-to/configure-load-balancers/#ssl-certificates

kcf apply -f ../assignments/loadb.yml

kcf describe pods demoapp-loadbalancer


kcf get service
kcf delete service demoapp-loadbalancer