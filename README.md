# Some IDEs settings that you have to search all over the Internet.
## Set up working through proxy
### nodejs/npm:
In a command prompt: 

  npm config set proxy http://proxy.company.com:port

  npm config set https-proxy http://proxy.company.com:port

### atom editor:
In a command prompt: 

  apm config set proxy http://proxy.company.com:port

  apm config set https-proxy http://proxy.company.com:port

## Netbeans file encoding
To force the ide to use UTF-8 add 

-J-Dfile.encoding=UTF-8

to netbeans_installation_path/etc/netbeans.conf

in parameter netbeans_default_options.
