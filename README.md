# Parent POM

![badge-version](https://img.shields.io/badge/Version-v1.0.0-green.svg)

## Introduction
This Maven parent POM is the base parent POM for all of the company's Maven artifacts. It contains the general 
information and settings shared by all Maven modules.

Relevant settings to be conscious of are:
* Encoding, both source and output, is set to **UTF-8**
* Resources under _src/main/resources_ are filtered
* SNAPSHOT versions are only allowed during development

## Usage
Include the following in the Maven POM of the Maven module you're working on (or use a derived parent which better suits your needs):

    <parent>
        <groupId>nl.agility.maven</groupId>
        <artifactId>parent-pom</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </parent>

## Profiles
The following profiles are included:

* [release-notes](#release-notes)

### release-notes
The *release-notes* plugin is activated when a **changes.xml** file is present in the **src/changes** folder of the
current module.

Every Maven module should keep track of its changes. 
