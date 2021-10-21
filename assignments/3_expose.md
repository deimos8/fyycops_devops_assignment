https://docs.digitalocean.com/products/kubernetes/how-to/configure-load-balancers/#ssl-certificates

kcf apply -f ../assignments/loadb.yml

kcf describe service http-lb


kcf get service
kcf delete service demoapp-loadbalancer