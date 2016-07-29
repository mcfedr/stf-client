# Stf::Client

Automation client for connecting to [OpenSTF](https://github.com/openstf/stf) devices.

Designed with the following scenario in mind:

1. Connect to remote devices
2. Do something with the device via adb (Instrumentation Test, adb install, etc)
3. Disconnect from device

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'stf-client'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install stf-client

## Usage

```
NAME
    stf-client - Smartphone Test Lab client

SYNOPSIS
    stf-client [global options] command [command options] [arguments...]

GLOBAL OPTIONS
    --help             - Show this message
    -t, --token=arg    - Authorization token (default: none)
    -u, --url=arg      - URL to STF (default: none)
    -v, --[no-]verbose - Be verbose

COMMANDS
    clean      - Frees all devices that are assigned to current user in STF. Doesn't modify local adb
    connect    - Search for a device available in STF and attach it to local adb server
    disconnect - Disconnect device(s) from local adb server and remove device(s) from user devices in STF
    help       - Shows a list of commands or help for one command
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/Malinskiy/stf-client.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).