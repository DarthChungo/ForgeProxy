# ForgeProxy

A simple minecraft mod for allowing 1.12+ forge clients to connect to proxy networks.

Minecraft proxy software, like bungeecord and velocity, stopped supported proxying modded clients ever since version 1.13 came out.
This was because of changes made in the forge protocol to accommodate the way Mojang implemented datapack handling in client-server communications.
This project attempts to circumvent this restriction by bypassing the proxy completely for forge servers.
Instead, it sends a custom packet to clients, once they request to connect to one of such servers, with all the information necessary for them to make the connection themselves.
Once the client leaves the other server, it will reconnect back to the proxy server.
For this to work, both client and proxy must have this mod installed.
This shouldn't really cause problems with forge clients, as hosting a forge server already requires players to install the server's modpack locally.

## License

The code in this repository is licensed under the MIT license:

```
ForgeProxy, a simple minecraft mod for allowing 1.12+ forge clients to connect to proxy networks.
Copyright © 2023 Antonio de Haro

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

