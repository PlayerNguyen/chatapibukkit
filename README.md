# ChatAPI Bukkit
Example Plugin ChatAPI Bukkit
# Install
You can download this plugin from <a href="http://dev.bukkit.org/bukkit-plugins/chat-api-dev/">Bukkit Page</a>
Install the plugin to folder /plugin from server file
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
# Remember
Add to message
```
return boolean;
```
Replace boolean to True/False
# Example Code
```
/*
 * This is example Message
 */

public class example extends JavaPlugin{
	
	ChatAPI capi = ChatAPI.message();
	
	public void onEnable(){
		capi.log("Message log");
	}
	
	// Command 
	public boolean onCommand(CommandSender sender, Command cmd, String label, String[] arrays){
		if(label.equalsIgnoreCase("example")){
		    // Custom Message
			capi.custom(sender, ChatColor.BLUE, "This is message blue color");
			
			// Red Color
			capi.red(sender, "Red Message");
			
			// MAGIC
			capi.magic(sender, "Magic Message");
			
			// Broadcast
			capi.broadcast("Broadcast Message");
			
			// Green Color
			capi.green(sender, "Green Message");
			
			// Yellow
			capi.yellow(sender, "Yellow Message");
			
			
			return true;
		}
		return true;
	}
}
```
