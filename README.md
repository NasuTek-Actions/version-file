version-file Action
===================
This allows creating of a yaml file containing version data for use in applications to get the following:
* Version
* Special Version (ex. -rc1, -b25, -dev)
* Revision (Uses a YYDDD type, ex 9/10/23 is 23253)
* GIT Commit SHA
* Time File was created

Inputs
------
* `version` [Required] - Version of the application.
* `special-build` [Optional] - The Special Build (ex -rc1). If blank it uses -b plus the action build number
* `file-output` [Required] - Location to drop the generated YAML File.

Example
-------
```
version: 1.0.0
revision: "23253"
special_build: -b4
git_revision: 8b994bf8e3d3c35c89e24cf79e62ecfa35812fc2
build_time: 2023-09-10T08:11:33.740+00:00
```