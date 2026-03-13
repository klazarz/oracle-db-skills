# `express` OCR Repository

## Overview

`database/express` is the Oracle Container Registry repository for Oracle Database Express Edition. Oracle lists this repository in the OCR Database business area and publishes both a latest pull command and a tags table for selecting concrete image versions.

## Repository Snapshot

- **Registry path:** `container-registry.oracle.com/database/express`
- **OCR short description:** Oracle Database Express Edition
- **Latest pull command shown on OCR:** `docker pull container-registry.oracle.com/database/express:latest`
- **License note on OCR:** OCR states that the software in this repository is licensed under the Oracle Free Use Terms and Conditions provided in the container image.

## What Oracle Documents Here

- The OCR readme documents this image as Oracle Database XE Release 21c (21.3.0.0) running on Oracle Linux 7.
- The page says the image contains a pre-built multitenant database with one pluggable database, which makes startup fast for development and CI/CD scenarios.
- OCR also documents custom configuration support and Podman secret support for securely supplying passwords.

## Oracle Version Notes (19c vs 26ai)

The OCR detail page documents `express` as Oracle Database XE Release 21c (21.3.0.0). This repository is not presented as a 19c or 26ai image line on OCR.

## When to Use / When Not to Use

- **Use this image when:** Use when you need Oracle Database XE 21c behavior in a compact local image.
- **Use another image when:** Avoid when you need newer AI Database 26ai capabilities; use free/enterprise.
- **Cross-image decision aid:** `skills/containers/container-selection-matrix.md`

## Prerequisites and Minimal Run Pattern

- **Prerequisite:** Accept OCR repository terms and authenticate to container-registry.oracle.com before pull.
- **Pull:** `docker pull container-registry.oracle.com/database/express:<tag>`
- **Run pattern:** `docker run --name <name> --rm -it container-registry.oracle.com/database/express:<tag>`
- **Important:** Use the OCR README example command for exact environment variables, mounted volumes, and published ports for this image.

## Sources

- https://container-registry.oracle.com/ords/ocr/ba/database/express
- https://www.oracle.com/downloads/licenses/oracle-free-license.html
