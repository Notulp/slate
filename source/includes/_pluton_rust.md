
# Pluton.Rust.Hooks

## On_PlayerConnected

```javascript
function On_PlayerConnected(player) {
    player.Message("Hi, " + player.Name);
}
```

```python
def On_PlayerConnected(self, player):
	player.Message("Hi, " + player.Name)
```

```csharp
public void On_PlayerConnected(Player player)
{
	player.Message("Hi, {player.Name}!");
}
```

```lua
function On_PlayerConnected(player)
    player.Message("Hi, " .. player.Name)
end
```

> This hooks is called when a player connects the server.

A player connected to the server.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### Parameter

<a href="#pluton-rust-objects-baseplayer">BasePlayer</a>

# Pluton.Rust.Objects

## Pluton.Rust.Objects.Player

```javascript
if (player.Admin) {
	player.Message("You are an admin!");
} else {
	player.Message("You are not an admin");
}

```

```python
if player.Admin:
	player.Message("You are an admin!")
elif:
	player.Message("You are not an admin")
```

```csharp
if (player.Admin) {
	player.Message("You are an admin!");
} else {
	player.Message("You are not an admin");
}
```

```lua
if player.Admin then
	player.Message("You are an admin!")
else
	player.Message("You are not an admin");
end
```

> A wrapper class that represents a player in rust and lets you interact with it in a convinient way.

### Inherits

Pluton.Rust.Objects.Entity

### Methods

Name | Parameters | Return type | Description
-----|------------|-------------|------------
Kick | [string:reason] | void | Kick the player with optional reason.
Message | string:message | void | Send a message to the player's chat.
MessageFrom | string:from
 | string:message | void | Send a message to the player's chat from specific name.

### Fields

Name | Type | Description
-----|------|------------
Admin | boolean | False if the player is not an admin and true if it is.
GameID | ulong | SteamID of the player.
Name | string | Name of the player.
