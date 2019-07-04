# BurpSuite Extension - Asset Discover[<img src="https://redhuntlabs.com/assets/images/target-audience-512-512x512.png" align="right" width="100">](https://redhuntlabs.com/)
Burp Suite extension to discover assets from HTTP response using passive scanning. Refer our blog [Asset Discovery using Burp Suite](https://redhuntlabs.com/blog/asset-discovery-burp-extension.html) for more details.

# Description
Passively parses HTTP response of the URLs **in scope** and identifies different type assets such as **domain, subdomain, IP, S3 bucket** etc. and lists them as informational issues.

# Setup
- Setup the python environment by providing the [jython.jar](https://www.jython.org/downloads.html) file in the 'Options' tab under 'Extender' in Burp Suite.
- Download the [extension](https://github.com/redhuntlabs/BurpSuite-Asset_Discover/archive/master.zip).
- In the 'Extensions' tab under 'Extender', select 'Add'.
- Change the extension type to 'Python'.
- Provide the path of the file ‘Asset_Discover.py’ and click on 'Next'.

<kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Add%20Extension.jpg" width="420" height="275"></kbd> <kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Add%20URL%20to%20scope.jpg" width="420" height="275"></kbd>

# Usage
- Add a URL to the 'Scope' under the 'Target' tab. The extension will start identifying assets through passive scan. 

<kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Asset%20Discovery%201.jpg" width="420" height="275"></kbd> <kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Asset%20Discovery%202.jpg" width="420" height="275"></kbd>

# Requirements
- [Jython 2.7.0](https://www.jython.org/downloads.html)
- [Burp Suite Pro v2.1](https://portswigger.net/burp)

# Code Credits
A large portion of the base code has been taken from the following sources:
- [OpenSecurityResearch CustomPassiveScanner](https://github.com/OpenSecurityResearch/CustomPassiveScanner)
- [PortSwigger example-scanner-checks](https://github.com/PortSwigger/example-scanner-checks)

# License
The project is available under MIT license, see [LICENSE](https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/LICENSE) file.
