# Tanzu .NET Web App

```
tanzu apps workload create tanzu-dotnet-web-app \
--git-repo https://github.com/fjb4/tanzu-dotnet-web-app \
--git-branch master \
--type web \
--label app.kubernetes.io/part-of=tanzu-dotnet-web-app \
--yes

tanzu apps workload create tanzu-dotnet-web-app -f ./config/workload.yaml --yes

tanzu apps workload tail tanzu-dotnet-web-app --since 10m --timestamp
```