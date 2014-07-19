Knife Solo Sample Application
=============================

It is a simple sample knife solo application to setup OpenVpn server and clients.


## Installation

### Install dependicies

Run `bundle install` to setup all required libraries.

### Setup a server node

Create a new node file in the `nodes` folder. Use the ip in the filename. Example: `nodes/127.0.0.1.json`.
The sample configuration is:

```json
{
  "run_list": []
}
```

### Setup a client node

Create a new node file in the `nodes` folder. The sample configuration is:

```json
{
  "run_list": []
}
```

### Deploy

```
knife solo prepare root@10.0.0.201
knife solo cook root@10.0.0.201
```

## References

- http://matschaffer.github.io/knife-solo/
- http://berkshelf.com
