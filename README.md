# ArchivesSpace Analytics for the PUI

## Getting started

Download and unpack the latest release of the plugin into your
ArchivesSpace plugins directory:

```
    $ curl ...
    $ cd /path/to/archivesspace/plugins
    $ unzip ...
```

Add the plugin name to the list of enabled plugins in `config/config.rb`:

```
AppConfig[:plugins] = ['some_plugin','aspace_analytics']
```

## What does it do?
The plugin adds Google and Matomo analyitcs to the PUI.

Joshua Shaw (<Joshua.D.Shaw@Dartmouth.EDU>)  
Digital Library Technologies Group  
Dartmouth College Library  
