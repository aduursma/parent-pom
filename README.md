# Parent POM

## Introduction
This Maven parent POM is the base parent POM for all of the company's Maven artifacts.

It contains the general information and settings shared by all Maven modules.

## Usage
Include the following in the Maven POM of the Maven module you're working on:

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
