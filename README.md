[![LucasBrosi](https://circleci.com/gh/LucasBrosi/Project05DevopsUdacity.svg?style=svg)](https://app.circleci.com/pipelines/github/LucasBrosi/Project05DevopsUdacity)

## Project Overview

Udacity Cloud DevOps Engineer
This repository contains all files for submission of Project 05.

app.py is an application that runs API-Calls against a pre-trained sklearn model that predicts housing prices in boston.
Together with an environment, described in the makefile and the requirements.txt file, it is bundled in a docker image as described in the Dockerfile and initiated by the run_docker.sh shellscript. At the end of run_docker, the app is run in a docker container.
Through upload_docker.sh, the image is uploaded to a cloud repository, docker hub in this case.
run_kubernetes spins up kubernetes cluster in which the container is deployed.

Inside the output_txt_files folder, the two documents contain the terminal output of the app when run in docker and kubernetes.
Circleci is used to test if the build works properly by linting the dockerfile (via hadolint) and linting the app.py (via pylint), confirming a successful build via a green badge displayed at the top of this document.




