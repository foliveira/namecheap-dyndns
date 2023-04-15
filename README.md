# Namecheap DynDNS 🌐

![GitHub version](https://img.shields.io/github/package-json/v/foliveira/namecheap-dyndns?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/foliveira/namecheap-dyndns?style=for-the-badge)
[![GitHub license](https://img.shields.io/github/license/foliveira/namecheap-dyndns?style=for-the-badge)][1]

Namecheap DynDNS is a command-line tool that allows you to update your dynamic DNS configurations for your domains using Namecheap API. With this tool, you can update your DNS record under a domain to a specific IP address.

## 🚀 Getting Started

### Prerequisites
  - Node.js 14.x or later

### Installing

```bash
npm install -g namecheap-dyndns
```

### Usage

You must pass three parameters to the application to authenticate and update your dynamic DNS configuration:
  - hostname
  - domain
  - key

These parameters can be passed to the application through:
 - **Command line switches**:
```bash
ncdd --hostname [hostname] --domain [domain] --key [accountKey]
```
- **Environment variables**:

```bash
ncdd_hostname=[hostname] ncdd_domain=[domain] ncdd_key=[accountKey]
```
  - **Config file**: $HOME/.ncddrc or $HOME/.$ncdd/config
```json
{
  "hostname": "[hostname]",
  "domain": "[domain]",
  "key": "[key]"
}
```

*Note: The default value for hostname is @.*

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 💻 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page or create a pull request.

## 📢 Acknowledgments

- [Namecheap API Documentation][3]

[1]: https://github.com/foliveira/namecheap-dyndns/blob/master/LICENSE
[3]: https://www.namecheap.com/support/api/
