# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.2.0] - 2020-05-08

### Added
- `exec` to run commands inside a running container
- `logs` to display and tail a container's output
- Support for running scripts inside `zeus.d` directory when machine is created
    - Can be run directly with `scripts`
- `top` to display CPU, memory, network and disk IO of running containers

## [1.1.0] - 2019-01-15

### Added
- `update` to fetch latest Docker images
- Ability to set a static IP during `create` if [docker-machine-ipconfig](https://github.com/fivestars/docker-machine-ipconfig) is installed 

### Changed
- Improved speed when checking if Docker machine is running

## [1.0.0] - 2019-01-14
### Added
- `run` command to run commands inside a container
- `env` command to simplify eval'ing a Docker machine
- Ability to restart the containers without restarting the Docker machine

### Changed
- Highlight output by `zeus`
