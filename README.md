# Tidewave 🌊

## Installation
- Clone this repo to the desired path
- Add the gem to your Gemfile by referencing the path:
`gem 'tidewave', path: '/path/to/the/cloned/repo'`

## Usage
I have tested it againt the official MCP inspector ATM:
`npx @modelcontextprotocol/inspector`

Launch your rails server on port other than 3000 (as MCP inspector's proxy runs on 3000):
`bundle exec rails s -p 3001`

Then, access the inspector's UI, choose SSE protocol, and for the URL, enter: `http://localhost:3001/tidewave/mcp`

## Cursor Settings
open ~/.cursor/mcp.json:
```json
{
  "mcpServers": {
    "tidewave": {
      "url": "http://localhost:3001/tidewave/mcp"
    }
  }
}
```
