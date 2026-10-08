# ArchivesSpace Analytics for the PUI

Adds Google Tag Manager and Matomo analytics snippets to the PUI.

## Getting started

Copy or clone the plugin into your ArchivesSpace plugins directory:

```
$ cd /path/to/archivesspace/plugins
$ git clone <repository-url> aspace_analytics
```

Add the plugin name to the list of enabled plugins in `config/config.rb`:

```
AppConfig[:plugins] = ['some_plugin','aspace_analytics']
```

Restart ArchivesSpace.

## Configuration

The snippets are included by default. To turn them off (e.g. on dev/test
instances) add this to `config/config.rb`:

```
AppConfig[:aspace_analytics_enabled] = false
```

## What does it do?

The plugin uses the PUI's plugin hooks to add:

* `public/views/layout_head.html.erb` - the GTM and Matomo scripts, in `<head>`
* `public/views/body_top.html.erb` - the GTM `<noscript>` fallback, at the top of `<body>`

The GTM container ID, Matomo URL/site ID and domain list are hardcoded in
these files; edit them to suit your site.

Compatible with ArchivesSpace 4.2.1.

Joshua Shaw (<Joshua.D.Shaw@Dartmouth.EDU>)  
Digital Library Technologies Group  
Dartmouth College Library  
