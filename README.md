# Pizza Planet

[![Build Status](https://app.travis-ci.com/capsulecorplab/pizza-planet.svg?branch=master)](https://app.travis-ci.com/github/capsulecorplab/pizza-planet)
[![Release](https://img.shields.io/github/v/tag/capsulecorplab/pizza-planet?label=release)](https://github.com/capsulecorplab/pizza-planet/releases/latest)
[![Documentation](https://img.shields.io/badge/Documentation-HTML-orange)](https://capsulecorplab.github.io/pizza-planet/) 
[![Gitpod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/capsulecorplab/pizza-planet) 

An OML model of a pizza restaurant, based on Tutorial 1 for creating an OML project http://www.opencaesar.io/oml-tutorials/.

## Clone
```
  git clone https://github.com/capsulecorplab/pizza-planet.git
  cd pizza-planet
```

## Build
Equivalent to owlReason task
```
./gradlew build
```

## Generate Docs
You must first have Bikeshed (the app itself) installed from [here](https://tabatkins.github.io/bikeshed/#install-final)
```
./gradlew generateDocs
```
Note: if bikeshed is not in the PATH, you can add -pBIKESHED=path/to/bikeshed argument

## Run OWL Reasoner
```
./gradlew owlReason
```

## Start Fuseki Server
```
./gradlew startFuseki
```

## Stop Fuseki Server
```
./gradlew stopFuseki
```

## Load to Fuseki Dataset
```
./gradlew owlLoad
```
Pre-req: A Fuseki server with a pizza-planet dataset must be running at http://localhost:3030/pizza-planet (see below)  

## Run SPARQL Queries
```
./gradlew owlQuery
```
Pre-req: A Fuseki server with a pizza-planet dataset must be running at http://localhost:3030/pizza-planet (see below)  

## Run SHACL Rules
```
./gradlew owlShacl
```
Pre-req: A Fuseki server with a pizza-planet dataset must be running at http://localhost:3030/pizza-planet (see below) 

## Publish to Maven Local
```
./gradlew publishToMavenLocal
```
