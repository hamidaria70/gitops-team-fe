# gitops-team-fe

In this repository, there are helm charts and `ArgoCD` application. The
applicaton is quite simple and it will deploy the `guestbook` application in
the cluster. 

About the `argocd-chart` helm chart, It is as same as the argocd-chart in the
[devops-assesment-test](https://github.com/hamidaria70/devops-assessment-test.git),
but without ingress and much more simple.

The tarball file, which is called **argocd-chart-team-fe-0.1.0.tgz**, is the
argocd-chart package which will be used by the `launcher` script in the
devops-assessment-test. If you need to add some changes to the package, you
only need to edit the `argocd-chart` and then create a package by running this
command:

```bash
helm package argocd-chart
```

Your new package is created.

**Note: Do not rename the tarball file name, otherwise the launcher script will
not be able to use it**
