# Elasticsearch Node Js (Updating)

From: https://www.digitalocean.com/community/tutorials/how-to-build-a-real-time-search-engine-with-node-vue-and-elasticsearch

## Content

1. [Development Enviroment](#development-environment)
2. [Continuous Integeration](#continuous-integeration)
3. [Test Execution](#test-execution)
4. [Git workflow](#git-workflow)
5. [Documentation](#documentation)

## Development Enviroment

- Software:
  - Firefox
  - [Ruby 2.6 with bundler](https://gorails.com/setup/ubuntu/16.04)

## Continuous Integeration

- Using Docker, see [gitlab-ci.yml](https://gitlab.com/lux-tech/automation-tests/-/blob/master/.gitlab-ci.yml)

## Test Execution

- All test case:

  `bundle exec rspec`
- A file only

  `bundle exec rspec <path_to_file>`
- A test only

  `bundle exec rspec <path_to_file>:<line_number>`

## Git workflow

- Get latest code at master branch

  `git pull origin master`

- From branch master

  `git checkout <new_branch_name>`

- Make changes on this branch

- Record the change

  ```sh
  git status
  git add .
  git commit -m "<your_message>"
  git push -f origin <new_branch_name>
  ```

- Create merge request on Git server

## Documentation

- [Capybara](https://github.com/teamcapybara/capybara)
