# versionchecker

Check for outdated packages installed on your system and get the latest version number

### Installation
 `pip install versionchecker`

### Usage
The package list should be in the format  {package_name: online_name}

package_name -> name of the package in your system

online_name -> name of package at [pypi](https://pypi.org/). If you are confused, just navigate to the project page (eg: https://pypi.org/project/notificationcenter/) and grab 'notificationcenter'

```
from versionchecker import check_packages

packages = {
	'urllib3': 'urllib3',
	'bs4': 'beautifulsoup4'
	}
	
results, latest_version = check_packages(packages)

print(results)
print(latest_version)
```

### Result
    {'urllib3': True, 'bs4': False}
    {bs4': '4.8.0'}



License
----
MIT
