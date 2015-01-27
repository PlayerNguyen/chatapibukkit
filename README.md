# ChatAPI Bukkit
Example Plugin ChatAPI Bukkit
# Install
You can download this plugin from <a href="http://dev.bukkit.org/bukkit-plugins/chat-api-dev/">Bukkit Page</a> and <a href="http://www.spigotmc.org/resources/chatapi.3500/">Spigot Page</a><br>
Import the file from IDE With:<br>
<ul>
  <li>Eclipse: Right Mouse to Project -> Properties -> Java Build Path -> Add External JARs -> Select ChatAPI.jar -> OK</li>
</ul>
Use API:<br>
```
import com.playernguyen.ChatAPI;
```
# Code
<h4>Print to console.</h4>

```
ChatAPI.message().log("Message in here");
```
<h4>Broadcast</h4>
```
ChatAPI.message().broadcast("Message In Here");
```
<h4>Chat with Color</h4>
Use the color replace to blue
```
ChatAPI.message().blue(sender, "Message in here");
```
<h4>Custom chat</h4>
```
ChatAPI.message().custom(sender, color, "Message in here");
```
<h4>Bold</h4>
```
ChatAPI.message().bold(sender, color, "Message In Here");
```
<h4>And etc</h4>
```
ChatAPI.message().magic(sender, color, "Message In Here");
```
# Example Code
```

```
