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

Paste any analytics snippets into `public/views/layout_head.html.erb` 
The plugin will add the contents of this file to all pages in the PUI.

For Google Tag Manager or other analytics that also have `<noscript>`
content, place that content in `public/views/body_top.html.erb` 

## What does it do?
The plugin adds a space to place analytics snippets for tracking usage of the PUI 
and can be used for tracking with Google, Matomo and other packages.

Joshua Shaw (<Joshua.D.Shaw@Dartmouth.EDU>)  
Digital Library Technologies Group  
Dartmouth College Library  
