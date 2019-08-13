# Docker Kaniko

## Usage

.gitlab-ci.yml
```yml
include:
  - project: 'hong.viet-ext/gitlab-pipeline-template'
    ref: master
    file: '.DockerKaniko.gitlab-ci.yml'

variables:
  DOCKER_IMAGE: "CHANGE_ME"
```

* The `latest` tag is linked to the `master` branch
* Each `push` will build an image with the `branch name` and the `git commit id`
* Each `tag` will build an image with the `tag name`
