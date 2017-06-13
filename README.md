# Habitat in Production

## ChefConf 2017 Talk by Fletcher Nichol

|                         |                              |
|-------------------------|------------------------------|
| Event                   | [ChefConf 2017](https://chefconf.chef.io/2017/) |
| Presentation Recording  | https://youtu.be/chDWP52rrHs |
| Online Slides           | https://fnichol.github.io/talk-chefconf2017-habitat-in-production/ |
| PDF Slides              | https://speakerdeck.com/fnichol/chefconf-2017-habitat-in-production |

## Abstract

The Habitat Supervisor is responsible for deploying, managing, and choreographing running Habitat services. This session will explore a number of the operational concerns that the supervisor enables. See how to manage secrets, store configuration changes in version control systems, update running applications, and choreograph application upgrades. This is the talk for anyone who is ready to run Habitat services in a production environment.

## Development

### Running Local Presentation

```sh
# Install dependencies
npm install

# Start local server
npm start
```

### Exporting PDF Slides

```sh
# Determine your workstation's IP address
ip_addr=10.0.0.15

# Export using Docker
docker run --rm --net=host -v $(pwd):/slides astefanutti/decktape http://${ip_addr}:8000 slides.pdf
```
