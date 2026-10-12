# Networking Basics 1

| File | Task |
| --- | --- |
| `0-change_your_home_IP` | Map localhost to 127.0.0.2 and facebook.com to 8.8.8.8 |
| `1-show_attached_IPs` | Display active IPv4 addresses |
| `2-port_listening_on_localhost` | Listen on localhost port 98 |

## Host mappings

The first script changes `/etc/hosts`. Save a copy before running it on a practice machine:

```sh
sudo cp /etc/hosts /etc/hosts.before-network-task
sudo ./0-change_your_home_IP
```

Restore the original mappings when finished:

```sh
sudo cp /etc/hosts.before-network-task /etc/hosts
```

## IP addresses

```sh
./1-show_attached_IPs
```

## Local listener

In the first terminal:

```sh
sudo ./2-port_listening_on_localhost
```

In another terminal, connect and type a message:

```sh
nc localhost 98
```
