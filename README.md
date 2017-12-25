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
