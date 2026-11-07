# Proxy Config

A customized Subconverter external configuration for Mihomo and Clash.

This project provides custom proxy groups, regional node selection, automatic node fallback, and curated routing rules to generate personalized proxy configurations.

## Disclaimer

**本仓库所有内容禁止以任何形式转载分享至中国大陆任何平台，否则您将承担所有法律责任。**

**本资源仅供中华人民共和国全境以外且不持有中华人民共和国任何地区国籍者使用，若您符合上述任一条件，请立即退出，严禁任何形式的浏览、保存、使用或分享，否则一切法律责任及不利后果自负。**

**所有内容仅适用于合法国家或地区，本人不承担任何法律责任。**

## Features

- **Regional Proxy Groups** — Automatically organize available nodes into Taiwan, Hong Kong, Japan, South Korea, Singapore, and United States groups.
- **All Nodes Selection** — Provides a centralized group containing all available subscription nodes.
- **Load Balancing** — Distributes incoming traffic across multiple nodes using advanced balancing strategies (e.g., Round-Robin, Least Connections) with real-time health checks to ensure high availability and optimal performance.
- **Custom Proxy Selection** — Provides a main `SELECT` group for convenient switching between different proxy groups.
- **Custom Routing Rules** — Includes routing rules for Google, Apple, Microsoft, Steam, GitHub, Telegram, OpenAI, and other services.
- **Direct Connection Rules** — Routes private networks, local services, and specified domains directly.
- **Ad Blocking** — Rejects traffic matching specified advertising rules.

## Configuration File

| File | Description |
|---|---|
| `Config-EliteL.ini` | Main Subconverter external configuration |

## Usage

1. Open the `Config-EliteL.ini` file in this repository.
2. Copy its **Raw** URL.
3. Add the URL to the external configuration section of a compatible Subconverter service.
4. Provide your proxy subscription URL and select the desired target format.
5. Generate the configuration and import it into your compatible proxy client.

### Raw URL

```text
https://raw.githubusercontent.com/youreverst/Proxy-Config/refs/heads/main/Config-EliteL.ini
```

## Proxy Groups

The configuration includes the following main proxy groups:

| Group | Description |
|---|---|
| `SELECT` | Main proxy selection group |
| `🇺🇳 ALL` | All available subscription nodes |
| `🇹🇼 ROC` | Taiwan Province nodes |
| `🇭🇰 HKG` | Hong Kong nodes |
| `🇯🇵 JPN` | Japan nodes |
| `🇰🇷 KOR` | South Korea nodes |
| `🇸🇬 SGP` | Singapore nodes |
| `🇺🇸 USA` | United States nodes |

## Compatibility

- **Configuration format:** Subconverter External Configuration (INI)
- **Primary converter:** Subconverter
- **Other converters:** Compatible with implementations supporting Subconverter external configuration syntax.
- **Target clients:** Mihomo and Clash-compatible clients.

Compatibility with other converters and clients may vary depending on their implementation and supported features.

> **Note:** This repository contains a Subconverter external configuration file, not a standalone Mihomo YAML configuration or a proxy subscription. A compatible converter is required to generate the final client configuration.

## License

This project is licensed under the [GNU Affero General Public License v3.0](LICENSE).

You are free to use, modify, and redistribute this project under the terms of the AGPL-3.0 license.
