# Pluton.Core.Hooks

## On_PluginLoaded

```javascript
function On_PluginLoaded(plugin) {
    Util.Log(plugin.Name + " plugin was loaded!");
}
```

```python
def On_PluginLoaded(self, plugin):
    Util.Log(plugin.Name + " plugin was loaded!")
```

```csharp
public void On_PluginLoaded(BasePlugin plugin)
{
    Util.Log("{plugin.Name} plugin was loaded!");
}
```

```lua
function On_PlayerConnected(plugin)
    Util.Log(plugin.Name .. " plugin was loaded!")
end
```

> The above command logs when a plugin is loaded.

Whatever.

### Parameter

<a href="#pluton-core-pluginloaders-baseplugin">BasePlugin</a>

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Congrats! You are on your way making awesome things happen!
</aside>
# Pluton.Core.PluginLoaders

## Pluton.Core.PluginLoaders.BasePlugin

```javascript
function On_PluginLoaded(plugin) {
    Util.Log(plugin.Name + " plugin was loaded!");
}
```

```python
def On_PluginLoaded(self, plugin):
    Util.Log(plugin.Name + " plugin was loaded!")
```

```csharp
public void On_PluginLoaded(BasePlugin plugin)
{
    Util.Log("{plugin.Name} plugin was loaded!");
}
```

```lua
function On_PlayerConnected(plugin)
    Util.Log(plugin.Name .. " plugin was loaded!")
end
```

> The base class for every plugin

### Inherits

CountedInstance
IPlugin

### Methods



### Fields

Name | Type | Description
-----|------|------------
Author | string | Your name.
Name | string | Name of the plugin.
