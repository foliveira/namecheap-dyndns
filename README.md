# namecheap-dyndns

Allows you to update your dynamic DNS configurations for your domains

## Getting Started
Install this package globally with: `npm install -g namecheap-dyndns` or `yarn global add namecheap-dyndns`

## Usage

Three parameters must be passed to the application so it can authenticate and update your Dynamic DNS configuration:

* **Hostname**
* **Domain**
* **Key**

These can be passed to the application, through **command line switches**:

`$ ncdd --hostname [host] --domain [domain] --key [accountKey]`

**environment variables**:

`$ ncdd_hostname=[host] ncdd_domain=[domain] ncdd_key=[accountKey]`

or **stored on file**, under `$HOME/.ncddrc` or `$HOME/.$ncdd/config`, with the following structure:

```
{
  "hostname": "[hostname]",
  "domain": "[domain]",
  "key": "[key]"
}
```



### Default Values

* Hostname => '@'

## License
Copyright (c) 2017 Fábio Oliveira <curious@foliveira.me>. Licensed under the MIT license.
