## newrelic-k8s-guestbook
### simple dockerized node.js express application
#### Thank you to Clay Smith and Vinod Vydier

This is an intentially simple express-based node.js web app that talks to a redis database. It's designed to run on a Kubernetes cluster, including managed clusters like Google Container Enginer (GKE) but can also run standalone. 

### dev requirements

* `node` > 6
* `express` (4.16.3) and the `newrelic` agent (4.8.0)

### running locally

```
    node index.js
```

### building the image

```
    docker build . -t wreckedreddocker/newrelic-k8s-guestbook
```

### running the image locally

```
    docker run -d -p 3000:3000 wreckedreddocker/newrelic-k8s-guestbook
```
