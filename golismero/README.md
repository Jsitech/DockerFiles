### Golismero Docker Container
=======================================
GoLismero is an open source framework for security testing. It's currently geared towards web security, but it can easily be expanded to other kinds of scans.

***The most interesting features of the framework are:***

*    Real platform independence. Tested on Windows, Linux, BSD and OS X.
*    No native library dependencies. All of the framework has been written in pure Python.
*    Good performance when compared with other frameworks written in Python and other scripting languages.
*    Very easy to use.
*    Plugin development is extremely simple.
*    The framework also collects and unifies the results of well known tools: sqlmap, xsser, openvas, dnsrecon, theharvester...
*    Integration with standards: CWE, CVE and OWASP.

***To run the container***

```
docker run jsitech/golismero COMMAND [Target] [options]
```

***Examples***

```
docker run jsitech/golismero scan test.com
```
***Override Entrypoint***

```
docker run --entrypoint /bin/bash jsitech/golismero
```

For more information and more usage examples visit the proyects page

https://github.com/golismero/golismero
