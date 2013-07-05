# Gears Present

A simple munin plugin for charting the number of active/idle gears
present on your application node instances.

# Setup Instructions

No special steps required for installation.

# Example Charts

Look at `server-gears_present` to see the syntax required to create
the charts you see in **nodes-small.ose-poc** and
**nodes-all.ose-poc**.


## node01.ose-poc

This chart is an example of the kind of data you can expect to see if
you're just installing the plugin on any given application node
instance.

It's not too fancy, x-axis = time, y-axis = number of gears
present/idle.


## nodes-small.ose-poc

I think this chart is way more more exciting than
**node01.ose-poc**. This chart shows the gear distribution across an
entire district (our **small** district, to be specific). This chart
does not show idle gears, only active gears.


## nodes-all.ose-poc

This chart is an extension of **nodes-small** showing the gear
distribution across all nodes in all districts.
