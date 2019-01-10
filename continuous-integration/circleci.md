# Circle CI

Uses `jobs` and `workflows` (which run jobs and can be 
parallelized).

## Job Syntax
```yml
jobs:
  job-name:
    docker:
      - image: circleci/image:version

    steps:
      - checkout  # shorthand checking out your code, can see it on your dashboard and make your own
      - run:
        # ...
```

## Workflow Syntax
```yml
workflows:
  version: 2
  workflow-name:
    jobs:
      # these get run in parallel
      - job1
      - job2
```
