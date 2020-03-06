# Batch Connect - OSC RClone Server

An interactive app designed for OSC OnDemand that launches an RClone Server
within a Quick batch job.

## State

This application is in an alpha state. It is currently a proof of concept and
does not run in production at OSC. It is meant to be an example and something
build on.

## Install

Use git to clone this app and checkout the desired branch/version you want to
use:

```sh
scl enable git19 -- git clone <repo>
cd <dir>
scl enable git19 -- git checkout <tag/branch>
```

To install the current version of rclone:

```sh
sh install_rclone.sh
```

If you want to run RClone CLI, simply use the RClone executable under the `rclone-*-linux-amd64` folder as [here](https://rclone.org/docs/). 

You will also not need to restart this app as it isn't a Passenger app.

To update the app you would:

```sh
cd <dir>
scl enable git19 -- git fetch
scl enable git19 -- git checkout <tag/branch>
```

Again, you do not need to restart the app as it isn't a Passenger app.

## Contributing

1. Fork it ( https://github.com/OSC/bc_osc_rclone/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
