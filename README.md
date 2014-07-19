Knife Solo Sample Application
=============================

It is a simple sample knife solo application to setup OpenVpn server and clients.


h2. Installation

h3. Install dependicies

Run `bundle install` to setup all required libraries.

h3. Setup a server node

Create a new node file in the `nodes` folder. Use the ip in the filename. Example: `nodes/127.0.0.1.json`.
The sample configuration is:

```json
{
  "run_list": []
}
```

h3. Setup a client node

Create a new node file in the `nodes` folder. The sample configuration is:

```json
{
  "run_list": []
}
```

h3. Deploy

```
knife solo prepare root@10.0.0.201
knife solo cook root@10.0.0.201
```

h2. References

- http://matschaffer.github.io/knife-solo/
- http://berkshelf.com
