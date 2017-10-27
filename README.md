## Use:
https://raw.githubusercontent.com/niklaushirt/chartslocal/master/repo/stable/
for repository URL

To preload images:

sudo docker pull bitnami/mariadb:10.1.23-r2
sudo docker pull bitnami/wordpress:4.8.1-r0
sudo docker pull bitnami/ghost:0.11.10-r2
sudo docker pull gcr.io/google-samples/gb-frontend:v4
sudo docker pull gcr.io/google_samples/gb-redisslave:v1
sudo docker pull gcr.io/google_containers/redis:e2e
sudo docker pull bitnami/mariadb:10.1.23-r2
sudo docker pull ibmcom/ucds:6.2.5.2.929926
sudo docker pull ibmcom/ucda:6.2.5.2.929926
sudo docker pull ibmcom/ucdr:6.2.5.2.929926

Login
docker login mycluster:8500

For UrbanCode Local
docker tag ibmcom/ucds:6.2.5.2.929926 mycluster:8500/devops/ucds:6.2.5.2.929926
docker tag ibmcom/ucda:6.2.5.2.929926 mycluster:8500/devops/ucda:6.2.5.2.929926
docker tag ibmcom/ucdr:6.2.5.2.929926 mycluster:8500/devops/ucdr:6.2.5.2.929926

docker push mycluster:8500/devops/ucds:6.2.5.2.929926
docker push mycluster:8500/devops/ucda:6.2.5.2.929926
docker push mycluster:8500/devops/ucdr:6.2.5.2.929926

And create namespace "devops"
