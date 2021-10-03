terraform init
terraform plan
terraform apply
terraform destroy

 sudo apt install ca-certificates

curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -
sudo apt-get install apt-transport-https --yes
echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm

helm install web ./helm/ --debug --dry-run 
helm install web ./helm/
helm upgrade web ./helm/
helm rollback web 1
helm history web
