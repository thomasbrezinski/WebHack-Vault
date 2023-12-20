> [!info] Very clear steps are documented on the developer docs, "[Build a Plugin](https://docs.obsidian.md/Plugins/Getting+started/Build+a+plugin)" page

## Basic Steps
1. Use an empty vault for development
2. Fork and clone the [sample plugin](https://github.com/obsidianmd/obsidian-sample-plugin) in your vault's `.obsidian/plugins` directory.
3. `npm run dev` in the sample plugin
4. Enable the plugin in your vault
5. Install and enable the [Hot Reload Plugin](https://github.com/pjeby/hot-reload)  which will reload your built plugin anytime it is rebuilt. 
6. Hack on the plugin
---
## Useful Tools
1. Chrome Dev Tools
	1. Obsidian is an electron app so you can use the regular chrome dev tools for debugging.
	2. The default `tsconfig.json` has `inlineSourceMap` enabled
	3. You can access the obsidian API from the tools console for exploration

---
Let's make an example change to [[Nested Daily Todos Plugin]]

---
## Testing
If your plugin depends on parts of the Obsidian API, it is best to separate those parts out from the rest because you cannot current write automated tests that depend on the any Obsidian methods unless you want to mock them all yourself.
[How to test plugin code that uses Obsidian APIs](https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/Guides/How+to+test+plugin+code+that+uses+Obsidian+APIs#How+to+test+plugin+code+that+uses+Obsidian+APIs)

---
## Publishing your plugin
There are instructions linked in the  [sample plugin](https://github.com/obsidianmd/obsidian-sample-plugin).
