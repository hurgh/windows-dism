# DISM Puppet Module

Thie module provides a DISM puppet resource type on Windows. Windows Deployment Image Servicing and Management (DISM.exe) is used to enable or disable Windows features on Windows 7, Windows Server 2008 R2.

Original cloned from https://github.com/puppetlabs/puppetlabs-dism

To use, the directory name needs to be changed to dism.

http://technet.microsoft.com/en-us/library/dd744582(v=ws.10).aspx

# Usage:

    dism { 'NetFx3':
      ensure => present,
    }

    dism { 'IIS-WebServer':
      ensure => present,
      answer => 'C:\answer\iis.xml',
    }
