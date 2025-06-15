# Bacularis plugins

This is repository with Bacularis plugins both for the web interface, API and
Common parts.

The files in this repository are part of Bacularis.

## Installation

### Step 1 - copy plugin to Bacularis

Depending on the plugin destination, there are three types of Bacularis plugins:

 * Plugins for the web interface
 * Plugins for the common part of Bacularis
 * Plugins for API

Before installing plugin, please make sure in the documentation what type is
the plugin that you want to install. This determines to which directory you should
copy the plugin file.

The general install plugin command form is the following:

```
cp ./{DESTINATION}/plugin-{PLUGIN_NAME_ID}/* {PROJECT_DIR}/protected/vendor/bacularis/{MODULE_NAME}/{DESTINATION}/Plugins/
```

where:

  * ``{DESTINATION}`` is the Bacularis component name in form:

    * ``Web`` for the web interface plugin
    * ``API`` for API plugin
    * ``Common`` for the common type plugin

  * ``{PLUGIN_NAME_ID}`` - plugin name identifier, for example for the API host job
    access plugin this is ``api-host-job-access``
  * ``{PROJECT_DIR}`` - is the main Bacularis directory
  * ``{MODULE_NAME`` - is the Bacularis module name in form:

    * ``bacularis-web`` - for the web interface
    * ``bacularis-common`` - for the common module
    * ``bacularis-api`` - for the API


Installing the web interface plugin can look like below. This is example for
the API host job access plugin:

```
cp ./Web/plugin-api-host-job-access/* {PROJECT_DIR}/protected/vendor/bacularis/bacularis-web/Web/Plugins/
```

### Step 2 - configure plugin

#### Web interface plugin

This plugin configuration is done on on the web interface.

To create the plugin configuration please go to the Bacularis web interface to
the ``Add-ons`` page available in the main menu. On the ``Plugins`` tab
please click the ``Add plugin settings`` button. Follow on the plugin
documentation in the [bacularis.app](https://bacularis.app/doc/) service.

#### API plugin

The plugin is configured in the API panel. Please go to the API panel
to the ``Settings`` page. On the ``Plugins`` tab please click the ``Add plugin
settings`` button. Follow on the plugin documentation in the
[bacularis.app](https://bacularis.app/doc/) service.

#### Common plugin

If documentation does not state differently, the plugin configuration is
done on on the web interface.

To create the plugin configuration please go to the Bacularis web interface to
the ``Add-ons`` page available in the main menu. On the ``Plugins`` tab
please click the ``Add plugin settings`` button. Follow on the plugin
documentation in the [bacularis.app](https://bacularis.app/doc/) service.

