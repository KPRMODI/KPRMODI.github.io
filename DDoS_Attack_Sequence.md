```mermaid
sequenceDiagram
participant Attacker
participant BotNet
participant Bots
participant Firewall
participant WebServer
participant User

Attacker->>BotNet: "Go attack the web server!"
Attacker-->BotNet: Gets botnet to attack 
BotNet ->> Attacker: "Alright!"
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Overrides with HTTP requests
WebServer ->> Firewall: Is overun with requests
BotNet --> Bots: Controls the bots/zombies to attack webserver.
BotNet ->> Bots: Go attack the web server Bots!
Bots ->> BotNet: Okay!
Firewall ->> Bots: Conducts traffic analysis to see requests
Firewall ->> Bots: Is in between webserver and bots
Firewall ->> Bots: Attempts to limit requests and filter them
Bots ->> Firewall: OverWhelms/Overfloods firewall
Bots ->> Firewall: Spams HTTP requests to webserver, firewall gets in way
Bots ->> Firewall: Sends HTTP request
Bots ->> Firewall: Sends HTTP request
Bots ->> Firewall: Sends HTTP request
Bots ->> Firewall: Sends HTTP request
Bots ->> Firewall: Sends HTTP requestt
Bots ->> Firewall: Sends HTTP request
Bots ->> Firewall: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
Bots ->> WebServer: Sends HTTP request
WebServer ->> User: Attempts to give user data
User ->> WebServer: Can't access WebServer Services 
WebServer --> User: Webserver is overwhelmed and shut downs
```
## Documentation
In a DDos attack (Distributed Denial-of-serive attack) an attacker purchases, uses, or makes their own botnet to perform the DDos attack. This can be due to many reasons such as a particular grudge against a webserver or just for their own entertainment. Then the botnet controls bots/zombies in order to spam or flood a web server with HTTP requests to overwhelm the server into shutting down or slowing down.

The bots begin to send several HTTP requests as seen in the diagram, but the firewall helps protect the webserver by conducting traffic analysis and limiting possible malicious requests.

However at some point the firewall is overwhelmed and it cannot keep up with HTTP requests and they start heading directly to the webserver. The webserver is quickly overflooded with requests and will either shutdown or slow down significantly.

The user is impacted the most, as they will go to the webserver to request a service just to find out that it is shut down or slowed making them use another web service or having to wait a long time.