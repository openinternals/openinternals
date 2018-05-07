---
title: "github.com/mholt/caddy"
date: 2018-05-07T15:19:43+05:30
draft: false
---

Caddy is a cool web server written in Golang. Go standard library already has a production ready server, used to serve the chromium downloads etc, according to Andrew Gerrand. What caddy does is piggyback on that barebones implementation and add a lot of goodies to it. This includes automatic HTTPS and HTTP/2 support, QUIC support etc.

The entire project is implemented as a pluggable architecture, so much so that the "http" type of server is a plugin. The TLS features are plugins, all the directives in the Caddyfile is a plugin.

The webserver can be configured with a command line arguments or with a Caddyfile. The Caddyfile is not JSON or YAML etc, it has it's own minimal syntax. The project has a parser to parse the Caddyfile.
The project source is licensed under Apache 2.0, but the official binaries obtained from the website are not free for commercial usage.

The docs are great and the website is lovely. Here we'll be talking to Matthew Holt, the author of Caddy

