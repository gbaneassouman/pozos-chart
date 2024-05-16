# dirs
```
mkdir -p lab-1/pozos-chart
```
# Package
```
helm package pozos-api
```
Successfully packaged chart and saved it to: /home/gbane/Projet-Devops/kubernetes/helm/lab-1/pozos-api-0.1.0.tgz

```
cp pozos-api-0.1.0.tgz pozos-chart
```
# Index
```
helm repo index pozos-chart/
```
```
ls -l pozos-chart/
```

```
total 16
-rw-r--r-- 1 gbane gbane  388 mai   15 21:09 index.yaml
-rw-rw-r-- 1 gbane gbane 4569 mai   15 21:05 pozos-api-0.1.0.tgz
-rw-rw-r-- 1 gbane gbane 1188 mai   16 09:30 README.md
```
# Repo github
```
git init 
```
- result
Dépôt Git vide initialisé dans /home/gbane/Projet-Devops/kubernetes/helm/lab-1/pozos-chart/.git/

``` 
git remote add origin https://github.com/gbaneassouman/pozos-chart.git
git pull origin main
git add .
git commit -m "Add pozos-chart
```
- 
```
[main 8b69c98] Add pozos-chart
 3 files changed, 45 insertions(+), 1 deletion(-)
 create mode 100644 index.yaml
 create mode 100644 pozos-api-0.1.0.tgz
```
- branche
```
git branch -M main
git push origin main
```
```
Énumération des objets: 7, fait.
Décompte des objets: 100% (7/7), fait.
Compression par delta en utilisant jusqu'à 12 fils d'exécution
Compression des objets: 100% (5/5), fait.
Écriture des objets: 100% (5/5), 5.41 Kio | 5.41 Mio/s, fait.
Total 5 (delta 0), réutilisés 0 (delta 0), réutilisés du pack 0
To https://github.com/gbaneassouman/pozos-chart.git
   6253b28..8b69c98  main -> main
```
# Ajout du répo à website

