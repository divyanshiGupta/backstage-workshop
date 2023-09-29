# Deploying an instance of Backstage using a Helm Chart on OpenShift

### Prerequisites

- OpenShift cluster

### Janus Backstage Helm Chart

1.  Login into OpenShift cluster web-console

2.  Create a namespace `backstage-workshop`

3.  Go to `+Add` page and select `Helm Chart` under `Developer Catalog`

4.  Search for Backstage helm chart and select it

5.  Click on create to open helm-chart yaml editor

6.  In the editor update `backstage-showcase` image tag to the latest nightly build which can be found ([here](https://quay.io/repository/janus-idp/backstage-showcase?tab=tags))

    ```
    image:
      registry: quay.io
      repository: janus-idp/backstage-showcase
      tag: nightly-20230929
    ```

7.  Click on Create

8.  In topology view click on URL decorator on the backstage deployment node to open the `backstage-showcase` app

# Deploying an instance of Backstage using a Helm Chart on Minikube

1. Follow the instructions ([here](https://github.com/divyanshiGupta/backstage-workshop/blob/main/backstage-helm-chart/README.md)) to deploy an instance of backstage using helm chart on minikube.
