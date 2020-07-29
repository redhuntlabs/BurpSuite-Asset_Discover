# BurpSuite Extension - Asset Discover[<img src="https://i1.wp.com/redhuntlabs.com/wp-content/uploads/2020/05/RedHunt-Logo-Without-Text-Dark.png?w=512&ssl=1" align="right" width="100">](https://redhuntlabs.com/)
Burp Suite extension to discover assets from HTTP response using passive scanning. Refer our blog [Asset Discovery using Burp Suite](https://redhuntlabs.com/blog/asset-discovery-burp-extension.html) for more details.

The extension is now part of the BApp store and can be installed directly from the Burp Suite. https://portswigger.net/bappstore/d927f0065171485981d6eb49a860fc3e

<kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/raw/master/Screenshots/Asset_Discovery_Burp_Extension.jpg" width="420" height="275"></kbd>

**[`To know more about our Attack Surface Management platform, check out NVADR.`](https://redhuntlabs.com/nvadr)**

# Description
Passively parses HTTP response of the URLs **in scope** and identifies different type assets such as **domain, subdomain, IP, S3 bucket** etc. and lists them as informational issues.

# Setup
- Setup the python environment by providing the [jython.jar](https://www.jython.org/download.html) file in the 'Options' tab under 'Extender' in Burp Suite.
- Download the [extension](https://github.com/redhuntlabs/BurpSuite-Asset_Discover/archive/master.zip).
- In the 'Extensions' tab under 'Extender', select 'Add'.
- Change the extension type to 'Python'.
- Provide the path of the file ‘Asset_Discover.py’ and click on 'Next'.

<kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Add%20Extension.jpg" width="420" height="275"></kbd> <kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Add%20URL%20to%20scope.jpg" width="420" height="275"></kbd>

# Usage
- Add a URL to the 'Scope' under the 'Target' tab. The extension will start identifying assets through passive scan. 

<kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Asset%20Discovery%201.jpg" width="420" height="275"></kbd> <kbd><img src="https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/Screenshots/Asset%20Discovery%202.jpg" width="420" height="275"></kbd>

# Requirements
- [Jython 2.7.0](https://www.jython.org/download.html)
- [Burp Suite Pro v2.1](https://portswigger.net/burp)

# Code Credits
A large portion of the base code has been taken from the following sources:
- [OpenSecurityResearch CustomPassiveScanner](https://github.com/OpenSecurityResearch/CustomPassiveScanner)
- [PortSwigger example-scanner-checks](https://github.com/PortSwigger/example-scanner-checks)

# License
The project is available under MIT license, see [LICENSE](https://github.com/redhuntlabs/BurpSuite-Asset_Discover/blob/master/LICENSE) file.
