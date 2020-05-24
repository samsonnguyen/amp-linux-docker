Installs and runs the AMP for Endpoints linux connector inside of docker. Supports Centos7 only

# Usage

* Git clone
* Download an AMP for Endpoints Linux (RHEL 7) to the directory from the AMP for Endpoints portal
* `docker-compose up --build`

You should see the new connector registered into AMP for Endpoints portal

# Issues

* Not all supported AMP for Endpoints features are available since we have limited kernel functionality within containers
* Only one rpm should be inside this directory. The entrypoint expects a single rpm and will attempt to install any rpm found. There may be issues if you have more than one
