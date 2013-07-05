# OpenShift Munin Plugins

## What's here?

A plugin suitable for charting interesting data about the number of
gears running in your
[OpenShift](https://github.com/openshift/origin-server)
environment.

This plugin creates a new group called **OpenShift**. There's only 1
plugin here now. If you're interested in contributing some more, then
by all means submit a pull request!


### Plugins

Plugins are organized by name in the **plugins** directory of this git
repository.

### Example server configs

You may also find example munin server configurations in the plugin
directories. Those files will have a **server-** prefix.

### Plugin Configurations

As necessary, a plugin directory will have one or more `*.conf` files
present for plugin configuration.

### Documentation

Any special or additional information about a plugin will be found in
a `README.md` file in its respective directory under
**plugins**. Information you can expect to find in these files
includes:

* Plugin descriptions
* Special installation instructions
* Descriptions and references to example charts (perhaps in the
  **charts** directory) produced by this plugin


## OpenShift?

Allow me to [quote them directly](https://www.openshift.com/products/online):

> OpenShift Online is Red Hat's public cloud application development
> and hosting platform that automates the provisioning, management and
> scaling of applications so that you can focus on writing the code
> for your business, startup, or next big idea.

Check out [https://www.openshift.com/](https://www.openshift.com/) if
you want to try it out for free.

There's also an
[Enterprise Edition](https://www.openshift.com/products/enterprise)
available for on-site deployment.


# Getting Started

## Standard Operating Procedure

On a host you want to gather data to make charts from:

1. Copy the plugin to the appropriate directory (usually that's `/usr/share/munin/plugins/`, but YMMV)
2. Link the plugin in `/etc/munin/plugins`: `cd /etc/munin/plugins; ln -s /usr/share/munin/plugins/PLUGIN_NAME`
3. Install the appropriate plugin configuration file in `/etc/munin/plugin-conf.d`

## Special Instructions

Any special or unusual installation instructions will be documented in
that plugins README.md file.

# Show me the charts

Example charts may be found in the **charts** directory. The file
names are prefixed with the plugin name. That is to say:
**openshift_gears_present-node01** would be an example of the chart
created by the `openshift_gears_present` plugin.


__TODO: Inline some example PNGs here__

