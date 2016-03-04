### Joomla Vulnerability Scanner Docker Container

==================================================

***JoomlaVS*** is a Ruby application that can help automate assessing how vulnerable a Joomla installation is to exploitation. It supports basic finger printing and can scan for vulnerabilities in components, modules and templates as well as vulnerabilities that exist within Joomla itself.

Pass the options while launching the Container

***Available Options:***

```
Basic options
    -u, --url              The Joomla URL/domain to scan.
    --basic-auth           <username:password> The basic HTTP authentication credentials
    -v, --verbose          Enable verbose mode
Enumeration options
    -a, --scan-all         Scan for all vulnerable extensions
    -c, --scan-components  Scan for vulnerable components
    -m, --scan-modules     Scan for vulnerable modules
    -t, --scan-templates   Scan for vulnerable templates
    -q, --quiet            Scan using only passive methods
Advanced options
    --follow-redirection   Automatically follow redirections
    --no-colour            Disable colours in output
    --proxy                <[protocol://]host:port> HTTP, SOCKS4 SOCKS4A and SOCKS5 are supported. If no protocol is given, HTTP will be used
    --proxy-auth           <username:password> The proxy authentication credentials
    --threads              The number of threads to use when multi-threading requests
    --user-agent           The user agent string to send with all requests

```

***Example:***

```
docker run -it jsitech/joomlavs -u jsitech.com --scan-all --follow-redirection

```
***Override Entrypoint***

```
docker run -it --entrypoint /bin/bash jsitech/joomlavs
```

JoomlaVS Project URL: https://github.com/rastating/joomlavs
