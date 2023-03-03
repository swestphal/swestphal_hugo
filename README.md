# swestphal_hugo

Install hugo
-> brew install hugo
enable Cloud Build api, Compute Engine
in Cloud Build settings enable Compute Engine and Service Accounts

Set up trigger in Cloud Build
// with Cloud Build configuration file (YAML or JSON)
// not docker, because first build website, then build docker image

Install Docker credential helper for Cloud Build
-> gcloud components install docker-credential-gcr
-> gcloud auth configure-docker

Install local builder
-> gcloud components install cloud-build-local
// if shell executable not found: brew cask info google-cloud-sdk

1) cloudbuild.YAML