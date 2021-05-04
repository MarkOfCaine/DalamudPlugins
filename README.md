https://raw.githubusercontent.com/akira0245/DalamudPlugins/cn/pluginmaster.json

https://raw.fastgit.org/akira0245/DalamudPlugins/cn/pluginmaster.json

## Making a plugin

Please see the [API documentation](https://goatcorp.github.io/Dalamud/api/index.html) for information about creating plugins.

## Publishing/updating your plugin

Create a pull request with your own subfolder in the plugins directory of this folder. It should be named the "internal" name(name of the DLL) of your plugin and contain a [plugin definition file](https://github.com/goatcorp/DalamudPlugins/blob/master/plugins/owofy/owofy.json) with the same name.
It should also contain a zip called "latest.zip" containing your plugin DLL, dependencies, resources and the plugin definition json ins the same folder as the plugin DLL.

When the AssemblyVersion of the locally installed plugin doesn't match the "AssemblyVersion" field of the plugin definition json pushed to this repository, a redownload of the plugin is forced.

For a sample of this, please see my [sample plugin](https://github.com/goatcorp/DalamudPlugins/blob/master/plugins/owofy).
