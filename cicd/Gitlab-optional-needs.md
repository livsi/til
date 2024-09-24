# Gitlab optional needs

There was a need to link two jobs. But if one of them may not start due to a number of conditions, then we have a problem.

You can mention it as an optional dependency:

```yaml
job1: 
  if: "$CI_COMMIT_BRANCH == master"
job2:
  needs:
    - job: job1
      optional: true
```

source: https://www.iduoad.com/til/gitlab-optional-needs/