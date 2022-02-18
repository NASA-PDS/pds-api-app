# NASA PDS Federated API

This repository is the entry point for the NASA PDS federated API specifications.

PDS is willing to develop restful web APIs for different applications (so far, data search, dois) without a priori limitation of what the API is relevant for.

Each of the applications for which an official PDS API end-point is published should be registered in this repository.

# API specifications available:

- registry (specification discussed in the PDS API Working Group)
- doi

# API entry points

The API base urls are provided under the following pattern:

    https://pds.nasa.gov/api/<application>/<version>

For example

    https://pds.nasa.gov/api/doi/0.2/


# API implementations

## Registry

Server: https://github.com/NASA-PDS/registry-api
Client: https://github.com/NASA-PDS/pds-api-client

## DOI

Server: https://github.com/NASA-PDS/doi-service
Client (UI): https://github.com/NASA-PDS/doi-ui
Client (react component): to be completed


# For developers, generate the API documentation

The openAPI yaml unrevolved specifications are stored in the `specs` directory.

The naming of the the specification are:
    PDS_APIs-<application>-<version>-swagger.yaml

For example:
    PDS_APIs-registry-1.0.0-SNAPSHOT-swagger.yaml
    

Generaate the doc with command line:

    pip install -e '.[dev]'
    sphinx-build -b html docs/source docs/build







# API implementations 

## Registry:

Various implementation flavors are available:

-   Java library: https://github.com/NASA-PDS/pds-api-javalib
-   Java official server (alpha version): https://github.com/NASA-PDS/registry-api-service , deployed on https://pds-gamma.jpl.nasa.gov/api/swagger-ui.html
-   Python client: https://github.com/NASA-PDS/pds-api-client


# API Documentation 

The API Documentation is available at: https://nasa-pds.github.io/pds-api/

We also publish [a draft of the PDS API Specification](https://docs.google.com/document/d/16d0MVh48bFLvWsa5-B_Hy-cby1rGWdnNojWOJpUcOvA/edit#heading=h.3pbz9ppxrxvr).


