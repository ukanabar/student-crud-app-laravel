<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

## CRUD in Laravel 5.8

This tutorial is created to illustrate the basic CRUD (Create , Read, Update, Delete) operation using SQL with Laravel 5.8. 

<b>Run manually</b>

- Run Compser Update
- Edit the .env file with relevant database credentials.
- Run 'php artisan migrate'
- Run php artisan serve

<b>Run using docker</b>

- docker build -t laravel-app .
- docker run -p 8181:8181 laravel-app
- To tag docker tag laravel-app ukanabar/laravel-student-app:1.0
- To push to docker hub docker push ukanabar/laravel-student-app:tagname

<b>Free DB</b>
- One can create free DB at https://www.db4free.net/
- Update DB settings in .env file of laravel
- Better approach will be to use config map from kubernetes

<b>Deploy to kubernetes or Azure Kubernetes Service</b>
- Deployment instruction can be found here: https://github.com/BuddhikaMayadunna/Aks/wiki/6.-Deploy-Docker-image-to-Azure-Kubernetes-Service-(-AKS-)-from-Dashboard
- If you receive permission errors on AKS similar to article https://unofficialism.info/posts/accessing-rbac-enabled-kubernetes-dashboard/, one can run 
     kubectl create clusterrolebinding kubernetes-dashboard --clusterrole=cluster-admin --serviceaccount=kube-system:kubernetes-dashboard