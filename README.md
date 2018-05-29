# Package Management Glossary :package:

A glossary of terms relating to package management.

## Project

The complete umbrella of a software project that may have one or more packages distributed across multiple package managers.

## Package (or Distribution)

A uniquely named record of a project being distributed on a registry, with one or more releases.

## Release (or Version)

A (mostly) immutable snapshot of a project's source code published at a point in time under a unique version number.

## Dependency

The declaration of the dependency of one package on another.

## Transitive Dependency

A transitive dependency is one that wasn't directly depended on by a package but instead the dependencies of one of a package's declared dependencies.

## Dependency Tree

A graph of all the resolved dependencies of a single package or manifest.

## Manifest

A file where a package or application can declare it's top level dependencies, often with version ranges.

## Lockfile

The place where a successfully resolve dependency tree is recorded so that it can be recreated at a later date.

## Dependency Resolution Algorithm

The strategy used to decide which releases of each package should be picked to produce the complete dependency graph for a package or manifest.

## Versioning scheme

The format and meaning applied to each release version number, often in the format X.Y.Z.

Two popular schemes are https://semver.org and http://calver.org.

## Version Range

A short hand for declaring or constraining which version numbers are acceptable for a package when resolving dependency trees.

## Client

The locally installed software for installing and managing packages, usually provided as a command line interface. Often communicates with one or more registries to find package and release metadata and to download releases.

## Registry

A source of metadata about packages, their releases and where to download those releases.

## Source Distribution

Packages that are published in the form of uncompiled source code, this is usually the default for scripting languages that cannot be compiled.

## Binary Distribution

Packages that are published in the form of a pre-compiled binary, usually without the original source code. There are often multiple binary distributions available for a single package, each compiled for a particular cpu architecture or operating system.

## Source Repository

The version control repository where development of a software project is co-ordinated, often hosted on GitHub, GitLab or Bitbucket.

## Application

The end-user software project that utilises other software projects as dependencies but is not something that can be directly depended upon or published as a package.
