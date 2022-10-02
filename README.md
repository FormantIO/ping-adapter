# Formant Ping Adapter

This adapter pings a remote host and then posts the result to a Formant stream to keep track of the robot's ping over time.

Note that the recorded ping is to an internet site, and will not necessarily reflect the ping to a remote operator.

## Configuration

The adapter requires the following configuration:

`hostname` - The hostname or IP address to ping.

`interval` - The interval in seconds between pings.

`timeout` - The timeout for the ping, in seconds.

`formant_stream` - The name of the stream to post the ping to.

## Tags

Successful pings will be posted with a `success: true` tag, and failed pings will be posted with a `success: false` tag.