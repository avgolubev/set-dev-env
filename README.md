# Some IDEs settings that you have to search all over the Internet.
## Set up working through proxy (in windows corporate network use cntlm, in addition to all of the settings below)
### nodejs/npm:
In a command prompt:  
  `npm config set proxy http://proxy.company.com:port  `  
  `npm config set https-proxy http://proxy.company.com:port`  


### ant:
In a command prompt:  
`set ANT_OPTS=-Dhttp.proxyHost=myproxy -Dhttp.proxyPort=3128`  

or for authenticated proxy:

`set ANT_OPTS=-Dhttp.proxyHost=myproxyhost -Dhttp.proxyPort=8080 -Dhttp.proxyUser=myproxyusername   -Dhttp.proxyPassword=myproxypassword -Dhttps.proxyHost=myproxyhost -Dhttps.proxyPort=8080`  


### atom editor:
In a command prompt:  
`apm config set proxy http://proxy.company.com:port`  
`apm config set https-proxy http://proxy.company.com:port`  


### git
Set proxy:  
`git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:port`  
#### or
`set http_proxy=http://proxy.company.com:port`  
`set https_proxy=http://proxy.company.com:port`  

Check the currently set proxy:  
`git config --global --get http.proxy`  

Reset proxy:  
`git config --global --unset http.proxy`  

### Haskell/Stack:
In a command prompt:  
`set http-proxy=http://proxy.company.com:port`  
`set https-proxy=http://proxy.company.com:port`  


## Netbeans file encoding
To force the ide to use UTF-8 add  
`-J-Dfile.encoding=UTF-8`  
to netbeans_installation_path/etc/netbeans.conf  in parameter netbeans_default_options.
