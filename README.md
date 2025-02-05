# datacube-docker

General purpose Docker Images related to the Open Data Cube project

## How this works

Each folder has a Dockerfile and a version.txt, as a minimum. There are two GitHub Actions
pipelines per image, one to test and one to build. In order to rebuild an image and have
it pushed to GitHub, you should increment the number in the version.txt file. Changing _anything_
in the folder of an Image currently triggers a run too.

Each project should have a docker-compose file that can be used to run and test the image.

## List of images

* [opendatacube/datacube-statistician](https://github.com/opendatacube/odc-stats/): Obsolete beyond 0.4.17 in this repo. The new location is [odc-stats/docker](https://github.com/opendatacube/odc-stats/tree/develop/docker)
* [opendatacube/datacube-index](index/readme.md): A suite of tools to manage indexing into an Open Data Cube database

