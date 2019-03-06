# chairmans-census
A tool to find in-game demographic data for a Final Fantasy XIV Free Company (guild) or other group

To use this tool, you'll need to provide your own [XIVAPI](https://xivapi.com) key.

Caveats for use:
* Provide the full FC name and server name; if you have a short FC name or one that returns multiple search results from The Lodestone, you may have to manually look up the FC's ID number yourself
* If any "Unknown" results appear in the final graph, run the worksheet again; whenever XIVAPI doesn't have cached character data available, it returns an empty JSON payload and adds that character to its retrieval queue
* Because of the nature of the method used, it can take a very long time to process very large FCs; a FC with 500 members takes about 20-25 minutes to run through twice
