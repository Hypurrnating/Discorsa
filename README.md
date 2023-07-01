# Discorsa
`Placeholder repo for Discorsa` 
___
Now this isn't just one app, it's a collection. There's a bot, there's a webserver, there's a mod, there will probably be a better website in the future...\
Because of this, I've split them into multiple repositories to make it easier to collaborate and deploy those apps. None of the actual repositories will be made public, instead this "frontpage" repo will be used for [new releases](https://github.com/Hypurrnating/Discorsa/tags), [tracking issues](https://github.com/Hypurrnating/Discorsa/issues), and [hosting the page](https://hypurrnating.github.io/Discorsa/) obviously, in addition to making some of the apps readable to the public, such as the mod clients.\

If you have any questions, or need help, there's a [discord server](https://discord.gg/DPTCrxawBx) just for that.

\
At the moment, the mod doesn't do a lot. Mainly relays your lap times to a server, where they are saved and sent to discord.\
I plan on expanding it to include more detailed data about each lap. This is a tricky thing to do since:
- Processing data from [AC Python Doc](https://docs.google.com/document/d/13trBp6K1TjWbToUQs_nfFsB291-zVJzRZCNaTYt4Dzc/pub), and [Shared Memory Reference](file:///C:/Users/imady/Downloads/ACSharedMemoryDocumentation.pdf) if a *little* tricky
- Assetto Corsa is using python version 3.3 (and don't get me started on importing modules)
- Worst: Assetto Corsa is a client sided game, and I am writing a client sided mod. This is notoriously horrible for security. 