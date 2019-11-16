# normalize.ci

> A tool to turn the continious integration / deployment variables into a common format for generally usable scripts without any dependencies.

## installation

```bash
sudo curl -L -s -o /usr/local/bin/normalizeci https://www.philippheuer.me/linux_amd64
sudo chmod +x /usr/local/bin/normalizeci
```

## usage

```bash
eval $(normalizeci)
```

## normalized variables

- [Specification: Variables](docs/spec/variables.md)

## supported systems

NAME | SLUG
--- | --- |
[Azure DevOps Pipeline](pkg/azuredevops/README.md) | `azure-devops`
[GitLab CI/CD](pkg/gitlabci/README.md) | `gitlab-ci`
[GitHub Actions](pkg/githubactions/README.md) | `github-actions`
[Local Git Repository](pkg/localgit/README.md) | `local`

*Note:* If none of the above systems is detected, repository information is determined based on the local Git repository.

## planned systems

- [AppVeyor](https://www.appveyor.com/docs/environment-variables)
- [AWS CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-env-vars.html)
- [Bamboo](https://confluence.atlassian.com/bamboo/bamboo-variables-289277087.html)
- [Bitbucket](https://confluence.atlassian.com/bitbucket/environment-variables-794502608.html)
- [Bitrise](https://devcenter.bitrise.io/builds/available-environment-variables/#exposed-by-bitriseio)
- [Buddy](https://buddy.works/knowledge/deployments/how-use-environment-variables#default-environment-variables)
- [Buildkite](https://buildkite.com/docs/builds/environment-variables)
- [CircleCI](https://circleci.com/docs/2.0/env-vars/#built-in-environment-variables)
- [Cirrus CI](https://cirrus-ci.org/guide/writing-tasks/#environment-variables)
- [Codefresh](https://codefresh.io/docs/docs/codefresh-yaml/variables#system-provided-variables)
- [Codeship](https://documentation.codeship.com/basic/builds-and-configuration/set-environment-variables/#default-environment-variables)
- [Drone](https://readme.drone.io/reference/environ/)
- [Jenkins](https://wiki.jenkins.io/display/JENKINS/Building+a+software+project)
- [Sail CI](https://sail.ci/docs/environment-variables)
- [Semaphore](https://semaphoreci.com/docs/available-environment-variables.html)
- [Shippable](http://docs.shippable.com/ci/env-vars/#stdEnv)
- [TeamCity](https://confluence.jetbrains.com/display/TCD10/Predefined+Build+Parameters)
- [Travis CI](https://docs.travis-ci.com/user/environment-variables#default-environment-variables)
- [Visual Studio Team Services](https://docs.microsoft.com/en-us/vsts/pipelines/build/variables)
- [Wercker](http://devcenter.wercker.com/docs/environment-variables/available-env-vars#hs_cos_wrapper_name)
