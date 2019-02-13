# release-it job sample

release-it in CircleCI Job sample

## :pushpin: Description

### DEMO

![](./sample.png)
<!-- add gif image if you like -->

## :white_check_mark: Features
<!-- list up your product features. -->
- bump up your app version triggered with API
```
## export CIRCLE_API_USER_TOKEN=xxxxxxxxxx
## ${TYPE} is expected one of below
## export TYPE=patch
## export TYPE=minor
## export TYPE=major
$ curl -u ${CIRCLE_API_USER_TOKEN}: -d build_parameters[CIRCLE_JOB]=release -d build_parameters[RELEASE_VERSION]=${TYPE} https://circleci.com/api/v1.1/project/github/mesh1nek0x0/release-sample/tree/master
```
- there are 3 jobs(build/test/release)
- build & test workflow will be started when you push repository

---

## :information_source: Anything else
- need github user key at circleci project setting
- need [personal token](https://circleci.com/account/api) to call CircleCI Job

## :pencil: Author
[mesh1nek0x0](https://github.com/mesh1neko)

## :clipboard: LICENCE
[MIT](https://github.com/mesh1neko/README-templates/blob/master/LICENSE)