This is a MCP (Model COntext Protocol) learning project. More details about the tools, resources and prompts, look at research_server.py.

To setup MCP server with vscode:
1. Ensure you have github copilot installed.
2. In the copilot prompt, click on tools icon -> Add more tools -> Add MCP server
3. settings.json should looks like below:
    {
    "mcp": {
        "servers": {
            "<servername- this is autocreated>": {
                "type": "stdio",                
                "command": "python",
                "args": ["/path/to/mcp_project/research_server.py"]
            }
        }
    }
}
4. In the settings.json file, start the MCP server.
5. pull settings.json file into github co-pilot prompt.
6. start prompt.

U can see the list of tools by clicking github copilot prompt tool icon
U can see the prompt templates by typing in the prompts /<prompt> <name> <args>
U can see the resources (data) by issuing the prompt "papers://folders" 

(OR)

U can also create your own MCP client