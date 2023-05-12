# OpenBash Burp Suite Plugin

This is a Burp Suite plugin that enables users to utilize the OpenBash surface scanner service for discovering hidden attack vectors in web applications and their infrastructure.

## Table of Contents

- [Description](#description)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Source Code](#source-code)
- [License](#license)
- [Contributing](#contributing)

## Description

The OpenBash plugin for Burp Suite allows users to perform various types of scans directly from the Burp Suite interface and receive information about potential vulnerabilities and exposures in real-time. By integrating OpenBash with Burp Suite, users can improve their web application security assessments and discover hidden attack vectors more efficiently.

## Requirements

- Burp Suite Professional or Community Edition
- Jython standalone JAR file (for Burp Suite to support Python plugins)
- OpenBash API key (obtainable at https://www.openbash.com)

## Installation

1. Download the `.py` file containing the plugin code.
2. Configure Jython in Burp Suite by following the [official guide](https://portswigger.net/burp/documentation/desktop/tools/extender#options-python-environment).
3. Open Burp Suite and go to the "Extender" tab.
4. In the "Extender" tab, select the "Extensions" subtab and click on the "Add" button.
5. In the pop-up window, select "Python" as the extension type and click on the "Select file" button.
6. Browse and select the `.py` file you downloaded earlier.
7. Click on the "Next" button and, if everything loads correctly, you will see the "Successfully loaded" message and the extension will appear in the list of installed extensions.

## Usage

1. Go to the "OpenBash" tab in Burp Suite.
2. Enter your OpenBash API key in the "API-KEY OPENBASH" field and click on "Save". If you do not have an API key, you can obtain one at https://www.openbash.com.
3. With the API key configured, select a request in any Burp Suite tab (e.g., "Proxy" -> "HTTP history").
4. Right-click on the selected request and you will see a context menu with various scan options provided by the OpenBash plugin:
    - Subdomains and Surface: Subdomains enumeration.
    - Discovery Web: Web discovery.
    - Infra ports 1-65535: Infrastructure ports scanning in the range of 1 to 65535.
    - Free demo: Free demo scan.
5. Click on the desired scan option and the plugin will send a request to OpenBash to initiate the scan.
6. The text area in the
