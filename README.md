# PSLANScan

[![version](https://img.shields.io/badge/version-1.0.1-blue.svg)](https://semver.org)

PSLANScan is a PowerShell module for layer 2 host discovery. It quickly finds live hosts on your network segment given a list of IP addresses, even if the hosts have ICMP/ping blocked by a firewall. 

The module is a single function but is packaged for convenience. 

## Installation


### Via PowerShell Gallery

`Install-Module -Name PSLANScan CurrentUser`


### Via Git

Clone the repository and run `.\build.ps1 deploy`.

This will install several modules if you do not already have them, see `build.ps1` for details. These are only required for the build process and are not otherwise used by `PSLANScan`.


### Manually

Copy the files from `src` to `$Home\Documents\WindowsPowerShell\Modules\PSLANScan` for PowerShell 5.1 or `$Home\Documents\PowerShell\Modules\PSLANScan` for PowerShell 7, and rename the `.ps1` file(s) to `.psm1`. 

## Usage

`Find-LANHosts -IP <String[]> [-DelayMS <int>] [-ClearARPCache]`

## More info

See this [blog post](https://xkln.net/blog/layer-2-host-discovery-with-powershell-in-under-a-second/) for further details