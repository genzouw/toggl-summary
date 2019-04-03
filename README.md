# toggl-summary

This is a script used to output working time information in a table format for a specified period using the [Toggl](https://toggl.com) API.

*Please contact me anytime if you have a problem or request! My information is posted at the bottom of this document.*

## Requirements

None.

## Dependencies

* [PHP](http://php.net/)
* [Composer](https://getcomposer.org/)


## Installation

```bash
# Download
$ git clone git@github.com:genzouw/toggl-summary.git
```

## Usage

```bash
# When no argument is specified, the work time of the current month is output.
$ ./tgl-summary

# When the first argument is specified, the work time from the specified date to the end of the current month is output.
$ ./tgl-summary 2019-02-01
project,description,duration,start,tags
pos-system,coding,0.73,2019-02-09T04:33:04+00:00,
pos-system,coding,1.35,2019-02-13T21:55:52+00:00,
pos-system,coding,0.83,2019-02-14T22:30:03+00:00,
pos-system,coding,2.28,2019-02-16T06:43:19+00:00,
pos-system,coding,0,2019-02-16T06:43:20+00:00,
pos-system,meeting,0.08,2019-02-16T07:50:38+00:00,
pos-system,meeting,0.57,2019-02-16T07:56:02+00:00,
pos-system,coding,1.15,2019-02-16T09:00:42+00:00,
pos-system,coding,1.74,2019-02-16T12:30:26+00:00,
pos-system,coding,0.58,2019-02-17T22:30:02+00:00,
pos-system,coding,4.76,2019-02-18T03:25:22+00:00,
pos-system,coding,0.65,2019-02-19T03:20:31+00:00,
pos-system,system_design,0.92,2019-02-21T21:50:56+00:00,
pos-system,system_design,0.57,2019-02-22T10:56:48+00:00,
pos-system,system_design,2.72,2019-02-23T02:46:15+00:00,
pos-system,system_design,0,2019-02-23T02:46:17+00:00,
pos-system,system_design,3.19,2019-02-23T05:40:47+00:00,
pos-system,system_design,2.33,2019-02-24T21:35:35+00:00,
pos-system,system_design,0,2019-02-24T22:00:35+00:00,
pos-system,system_design,1.87,2019-02-25T03:44:00+00:00,
pos-system,system_design,0.68,2019-02-25T11:49:02+00:00,
pos-system,meeting,0.73,2019-02-27T10:00:44+00:00,
pos-system,webpush,0.04,2019-02-27T11:28:15+00:00,
pos-system,system_design,0,2019-02-27T11:30:47+00:00,
pos-system,system_design,0.99,2019-02-27T22:35:25+00:00,
pos-system,webpush,0.25,2019-02-28T23:00:07+00:00,


# When the first argument and the second argument are specified, the work time from the day of the first argument to the day of the second argument is output.
$ ./tgl-summary 2019-02-01 2019-02-20
project,description,duration,start,tags
pos-system,coding,0.73,2019-02-09T04:33:04+00:00,
pos-system,coding,1.35,2019-02-13T21:55:52+00:00,
pos-system,coding,0.83,2019-02-14T22:30:03+00:00,
pos-system,coding,2.28,2019-02-16T06:43:19+00:00,
pos-system,coding,0,2019-02-16T06:43:20+00:00,
pos-system,meeting,0.08,2019-02-16T07:50:38+00:00,
pos-system,meeting,0.57,2019-02-16T07:56:02+00:00,
pos-system,coding,1.15,2019-02-16T09:00:42+00:00,
pos-system,coding,1.74,2019-02-16T12:30:26+00:00,
pos-system,coding,0.58,2019-02-17T22:30:02+00:00,
pos-system,coding,4.76,2019-02-18T03:25:22+00:00,
pos-system,coding,0.65,2019-02-19T03:20:31+00:00,
```



## Configuration

```bash
# Setting
## For information on how to obtain Toggl's API Token, see the following page.
## [Documentation for the Toggl API](https://github.com/toggl/toggl_api_docs#api-token)
$ export TOGGL_API_TOKEN='xxxxxxxxxxxxxxxx'

# If you hope, you append system environment in .bashrc
$ cat <<'EOF' >>~/.bashrc
export TOGGL_API_TOKEN='xxxxxxxxxxxxxxxx'
EOF
```


## Relase Note

| date       | version | note           |
| ---        | ---     | ---            |
| 2019-03-01 | 0.1     | first release. |


## License

This software is released under the MIT License, see LICENSE.


## Contribution


## Author Information

[genzouw](https://genzouw.com)

* Twitter   : @genzouw ( https://twitter.com/genzouw )
* Facebook  : genzouw ( https://www.facebook.com/genzouw )
* LinkedIn  : genzouw ( https://www.linkedin.com/in/genzouw/ )
* Gmail     : genzouw@gmail.com
