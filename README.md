# ChatAPI Bukkit
Example Plugin ChatAPI Bukkit
# Install
Import the file from IDE With:<br>
Eclipse: Right Mouse to Project -> Properties -> Java Build Path -> Add External JARs -> Select ChatAPI.jar -> OK
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
ChatAPI.message().blue(sender, "Message in here")
```
<h4>Custom chat</h4>
```
ChatAPI.message().custom(sender, color, "Message in here")
```
