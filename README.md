# Google Container Registry Mirror

The purpose of this project is to store the tags of the gcr.io image, they have been pushed to [dockerhub](https://hub.docker.com/u/k8sio/) and quay ([google-containers](http://quay.io/google-containers), [google-samples](http://quay.io/google-samples), [google-appengine](http://quay.io/google-appengine)). In addition, you can get the corresponding Dockerfile from <https://github.com/k8sio>. Inspired by [anjia0532/gcr.io_mirror](https://github.com/anjia0532/gcr.io_mirror).

## How to pull

### From docker.io (Docker Hub)

```bash
# 'google-containers' repository
$ docker pull k8sio/kube-apiserver-amd64:v1.10.0
$ docker tag k8s/kube-apiserver-amd64:v1.10.0 gcr.io/google-containers/kube-apiserver-amd64:v1.10.0

# 'google-samples' repository
$ docker pull k8sio/cassandra:v14
$ docker tag k8sio/cassandra:v14 gcr.io/google-samples/cassandra:v14

# 'google-appengine' repository
$ doker pull k8s/golang:v1.8.0
$ doker tag k8s/golang:v1.8.0 gcr.io/google-appengine/golang:v1.8.0
```

### From quay.io

```bash
# 'google-containers' repository
$ docker pull quay.io/kube-apiserver-amd64:v1.8.0
$ docker tag quay.io/google-containers/kube-apiserver-amd64:v1.8.0 gcr.io/google-containers/kube-apiserver-amd64:v1.8.0

# 'google-samples' repository
$ docker pull quay.io/google-samples/cassandra:v14
$ docker tag quay.io/google-samples/cassandra:v14 gcr.io/google-samples/cassandra:v14

# 'google-appengine' repository
$ doker pull quay.io/google-appengine/golang:v1.8.0
$ doker tag quay.io/google-appengine/golang:v1.8.0 gcr.io/google-appengine/golang:v1.8.0
```

## Repository

* [google_containers](./google_containers/README.md)
* [google_samples](./google_samples/README.md)
* [google-appengine](./google-appengine/README.md)