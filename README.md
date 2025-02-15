# FreeBSD-kmod
This place gives some kernel modules in sync with kernel in the shape of installable packages.

When a new minor version of FreeBSD is released, three months are required before the repositories get compiled with this new version.
For mundane softwares, there is no incidence, but for the ones that are kernel modules, this can lead to some problems, including crashes.

# Naming
They are in the form _Version_-**name_of_the_port**.pkg  
Example: _14.1_-**drm-61-kmod-6.1.92**.pkg

# Use
Install this package with:  
`# pkg add Version-name_of_the_port.pkg`  
`# pkg lock name_of_the_port`  

Don't forget to unlock it when the repositories get updated to the new minor version of FreeBSD.

## Example

Using the GitHub _raw_ link for a `.pkg` file: 

`pkg add https://github.com/Emrion/FreeBSD-kmod/raw/refs/heads/main/14.2-virtualbox-ose-kmod-6.1.50.pkg`
