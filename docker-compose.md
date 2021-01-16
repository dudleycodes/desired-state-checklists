# Desired State Checklist: Docker Compose

* I like setups that don't bind ports to host's `0.0.0.0`.
  * Should bind to `127.0.0.1:<host-port>:<container-port>` for local access.
* I like setups that don't use the host network.
