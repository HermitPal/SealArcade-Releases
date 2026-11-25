# Seal Arcade Releases

Download the latest build from [Releases](https://github.com/HermitPal/SealArcade-Releases/releases/latest).

| Download | What it is |
| --- | --- |
| `SealPlayer-<platform>.zip` | Runs a single Seal Arcade game |
| `SealServer-<platform>.zip` | Dedicated server for hosting an arcade |

## Running the server

Unzip and run `SealServer`. It prints:

- **Friend code**: for desktop players
- **Browser Joining**: a code and `wss://` address for players in a web browser, provided through the bundled `cloudflared`
- **Same network**: a LAN address

Options:

| Flag | Effect |
| --- | --- |
| `--port=27015` | Port to listen on |
| `--max-players=N` | Player limit |
| `--password=TEXT` | Require a password |
| `--lan` | Same network only, no friend or browser codes |
| `--no-browser` | Skip browser joining |
| `--terminal` | Run without a window |

On macOS, the first time you open it: right-click → Open.

`cloudflared` is made by Cloudflare and included under the Apache 2.0 license (`cloudflared-LICENSE.txt`).
