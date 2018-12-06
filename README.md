## Kubernetes

Issue: The connection to the server localhost:8080 was refused - did you specify the right host or port?
Answer: remove old config under ~/.kube/, add new admin.conf, then run:
 *       `sudo chown $(id -u):$(id -g) ~/.kube/admin.conf`
 *       `export KUBECONFIG=/home/ubuntu/.kube/admin.conf`
