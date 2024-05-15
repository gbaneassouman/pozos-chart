# dirs
mkdir -p lab-1/pozos-chart

# Package
helm package pozos-api 
Successfully packaged chart and saved it to: /home/gbane/Projet-Devops/kubernetes/helm/lab-1/pozos-api-0.1.0.tgz

cp pozos-api-0.1.0.tgz pozos-chart

# Index
helm repo index pozos-chart/
ls -l pozos-chart/

# Repo github
git init 
- result
Dépôt Git vide initialisé dans /home/gbane/Projet-Devops/kubernetes/helm/lab-1/pozos-chart/.git/
- 
git add .
git commit -m "Initial commit"

- 
[main (commit racine) 600f511] Initial commit
 3 files changed, 33 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.yaml
 create mode 100644 pozos-api-0.1.0.tgz

- branche
git branch -M main
git remote add origin https://github.com/gbaneassouman/pozos-chart.git
