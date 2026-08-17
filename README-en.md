<h1 align="center">DPanel Third-Party App Store</h1>

<p align="center">
  A collection of Docker application configurations adapted for the <code>DPanel</code> app store. Can be imported directly into DPanel.
</p>

<p align="center">
  <img src="docs/afdian-logo.png" alt="Docker Apps project banner" width="640">
</p>

<p align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-2875B6?style=flat-square" alt="Simplified Chinese (current language)"></a>
  <a href="README-en.md"><img src="https://img.shields.io/badge/English-D9D9D9?style=flat-square" alt="Read in English"></a>
</p>

## Support the Project

<p align="center">
  <a href="https://ifdian.net/a/QUAN_GE"><strong>Support on AFDIAN: Power with Love</strong></a><br><br>
</p>

<details>
<summary><strong>Table of Contents</strong></summary>

- [Support the Project](#support-the-project)
- [Disclaimer](#disclaimer)
  - [1. Image Container Adaptation](#1-image-container-adaptation)
  - [2. Compliance with Laws](#2-compliance-with-laws)
  - [3. Acceptance of Disclaimer](#3-acceptance-of-disclaimer)
- [1. Introduction](#1-introduction)
- [2. Usage](#2-usage)
- [3. Contributing Apps](#3-contributing-apps)
- [Retired Apps](#retired-apps)

</details>

***

## Disclaimer

### 1. Image Container Adaptation

This project only adapts the original `docker` image container operation for the `DPanel` app store. We do not make any express or implied warranties or representations about the validity of any original images, and we are not responsible for any consequences arising from the use of applications in this repository. Users assume all risks when using this project.

### 2. Compliance with Laws

Users must comply with the laws and regulations of their respective countries and regions when using this repository. Some applications may be restricted by specific national laws, and users are responsible for understanding and following relevant legal requirements. This repository is not responsible for any consequences resulting from users' violations of laws or regulations.

### 3. Acceptance of Disclaimer

By importing this repository and using the applications within, users signify that they have read, understood, and accepted all terms and conditions of this disclaimer.

Please note that this disclaimer applies only to the use of this repository and does not cover other third-party applications or services. We are not responsible for the accuracy, completeness, reliability, or legality of any third-party content linked from this repository.

Before using this repository, please ensure that you have read, understood, and accepted all terms and conditions of this disclaimer.

***

## 1. Introduction

This repository organizes application directories, metadata, form variables, and Docker Compose configurations according to the DPanel v2 application specification. The goal is to make applications installable immediately after import, minimizing manual deployment and repetitive configuration.

## 2. Usage

Add a custom app store in the panel with the following URL:

    https://github.com/quan-ge/dpanel-appstore

For users with poor network connectivity to GitHub, please use:

    https://down.nigx.cn/github.com/quan-ge/dpanel-appstore

## 3. Contributing Apps

> [!IMPORTANT]
> Before submitting a PR for an app, third-party developers are strongly encouraged to use [okxlin/1panel-app-adapter](https://github.com/okxlin/1panel-app-adapter) to generate or validate the app package. It checks the 1Panel v2 directory structure, `data.yml`, `docker-compose.yml`, environment variable closure, i18n labels, and common release issues, helping to reduce rework.

When submitting a PR, please prioritize providing reproducible official sources, image sources, default ports, data directories, dependencies, and test results. Only the final app directory is required in the repository; do not commit temporary test artifacts or intermediate files.

## Retired Apps

Apps that cannot be installed and have no trustworthy alternative image will be removed from the active catalog to avoid misleading new users. Retirement reasons and the last recorded versions are documented in [`.github/retired-apps.yml`](.github/retired-apps.yml). The complete app files can still be recovered from Git history.