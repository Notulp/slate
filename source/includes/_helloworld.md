# Hello World

> Your first plugin:

```javascript
function On_PlayerConnected(player) {
    player.Message("Hi, " + player.Name);
}
```

```python
class Example:
    def On_PlayerConnected(self, player):
        player.Message("Hi, " + player.Name)
```

```csharp
namespace Example
{
    using Pluton.Rust.PluginLoaders;
    using Pluton.Rust.Objects;
    
    public class Example : CSharpPlugin
    {
        public void On_PlayerConnected(Player player)
        {
            player.Message("Hi, {player.Name}!");
        }
    }
}
```

```lua
function On_PlayerConnected(player)
    Player.Message("Hello, " .. player.Name)
end
```

> Make sure in c# the name of the main class containing the hooks is the same as the namespace and the name of the plugin. And in python the class name is the same as the file name.

TODO: add useful stuff
