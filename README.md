# This repository, explains how you can deploy Pacman with ACM or ArgoCD

- First QuickStart explains how to deploy Pacman on ACM console.
- Second QuickStart explains how to deploy Pacman with ArgoCD.
- You can also use oc kustomize to deploy ACM pacman application: 

  ```
  git clone -c http.sslVerify=false https://gitlab.hpintelco.org/githit/pacman.git
  oc kustomize pacman/acm-application | oc apply -f -
  ```

Pacman can work without mongo, but if ODF is installed, mongo will use a ceph rbd PVC

