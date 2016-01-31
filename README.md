# minid
This project aims to create a Minimal Viable Identifier (MVI). An identifier that is sufficiently simple to make creation and use trivial, while still having enough substance to make data easily findable, accessible, interoperable, and reusable (FAIR). 

## Installation
The CLI can be installed using Python setuptools. 

## Configuration
To use the CLI you will need create a configuration file with your details in `~/.minid/minid-config.cfg`

```
[general]
minid_server: http://minid.bd2k.org/minid
local_server: <Globus endpoint or HTTP server>
username: <Name>
orcid: <Orcid>
```

## Usage

The CLI supports the following simple operations (Note: the test flag will create names in a test namespace that will be removed periodically, remove the test flag for creating production minids.): 

* Create a new identifier: `minid.py <file_name> --test --register [--title <title>]`
* Retrieve metadata about a file: `minid.py <file_name> --test` 
* Retrieve metadata about an identifier: `minid.py <identifier> --test`

Landing pages are accessible via the minid website: minid.bd2k.org/minid/<identifier>. 

## More information
More information about the project can be found at: [minid.bd2k.org](http://minid.bd2k.org/)
