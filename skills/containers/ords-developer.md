# `ords-developer` OCR Repository

## Overview

`database/ords-developer` is the Oracle Container Registry repository for Oracle REST Data Services (ORDS) Developer. Oracle lists this repository in the OCR Database business area and publishes both a latest pull command and a tags table for selecting concrete image versions.

## Repository Snapshot

- **Registry path:** `container-registry.oracle.com/database/ords-developer`
- **OCR short description:** Oracle REST Data Services (ORDS) Developer
- **Latest pull command shown on OCR:** `docker pull container-registry.oracle.com/database/ords-developer:latest`
- **License note on OCR:** OCR states that the software in this repository is licensed under the Oracle Free Use Terms and Conditions provided in the container image.

## What Oracle Documents Here

- The OCR detail page says `ords-developer` is the Oracle REST Data Services Developer image and includes APEX alongside ORDS.
- OCR explicitly marks the image as deprecated beginning with ORDS version 24.4.0.
- The same page says `ords-developer` will be completely removed from the container registry by May 2026 and points users to the supported `ords` image.

## Oracle Version Notes (19c vs 26ai)

The OCR detail page includes the key version note for this repository: `ords-developer` is deprecated beginning with ORDS 24.4.0 and is scheduled for removal from OCR by May 2026.

## When to Use / When Not to Use

- **Use this image when:** Use only for short-term legacy workflows that still depend on this image.
- **Use another image when:** Avoid for new deployments; use ords.
- **Cross-image decision aid:** `skills/containers/container-selection-matrix.md`

## Prerequisites and Minimal Run Pattern

- **Prerequisite:** Accept OCR repository terms and authenticate to container-registry.oracle.com before pull.
- **Pull:** `docker pull container-registry.oracle.com/database/ords-developer:<tag>`
- **Run pattern:** `docker run --name <name> --rm -it container-registry.oracle.com/database/ords-developer:<tag>`
- **Important:** Use the OCR README example command for exact environment variables, mounted volumes, and published ports for this image.

## Sources

- https://container-registry.oracle.com/ords/ocr/ba/database/ords-developer
- https://container-registry.oracle.com/ords/ocr/ba/database/ords
- https://apex.oracle.com/
- https://www.oracle.com/rest/
