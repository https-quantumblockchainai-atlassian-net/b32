# B32
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhttps-quantumblockchainai-atlassian-net%2Fb32.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhttps-quantumblockchainai-atlassian-net%2Fb32?ref=badge_shield)


> [Signature collection of smart contract method & event.](https://b32.vecha.in)

To help retrieving method/event's JSON ABI by its signature.

## Submit JSON ABI

* Initiate a new [pull request](https://github.com/vechain/b32/new/master/ABIs)
* Fill the file name like <`my-awesome-contract.json`>
* Fill the file content with full JSON ABI produced by [solidity compiler](https://github.com/ethereum/solidity/releases)


## Query JSON ABI

```bash
# replace 0x06fdde03 with your signature
> curl https://b32.vecha.in/q/0x06fdde03.json
```

The output will be 
```JSON
[{"constant":true,"inputs":[],"name":"name","outputs":[{"name":"","type":"string"}],"payable":false,"stateMutability":"pure","type":"function"}]
```

which is an array of objects which share the same signature.



## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhttps-quantumblockchainai-atlassian-net%2Fb32.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhttps-quantumblockchainai-atlassian-net%2Fb32?ref=badge_large)