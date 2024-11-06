![banner](./assets/banner.png)
<p align="center">
   <a href="https://discord.gg/MGSvZBdc4p"><img alt="Discord Server" src="https://invidget.switchblade.xyz/MGSvZBdc4p"></a>
</p>

## Register
1. Fork the repo.
2. Make a json file named `example.json` in the `domains` directory
3. Add the following file format to the json you just made:
```json
{
    "owner": {
        "username": "yourgithubusername",
        "email": ["test@example.com", "another@example.com"]
    },

    "record": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["2606:4700:4700::1111", "2606:4700:4700::1001"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "NS": ["ns1.example.com", "ns2.example.com"],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ]
    },

    "proxied": false
}
```
> [!NOTE]
> Only select the records you need, this is just a example on what all the records we support should be.

4. After the pull request is merged, DNS should propagate within about 15 minutes to a maximum of 24 hours.
5. That's all, enjoy your `is-truly-a.pro` domain!

> [!WARNING]
> We only give out NS records to those who have a reasonable use case for them. If you don't have a reasonable use case for them, we will close your PR.


## Issues
If you have any problems or want to report a subdomain, feel free to [open a issue](https://github.com/is-truly-a-pro/register/issues/new/choose).

### Similar Services
If you want to find services similar to is-truly-a.pro, please check out [Open Domains](https://github.com/open-domains/register) and [is-a.dev](https://github.com/is-a-dev/register).
