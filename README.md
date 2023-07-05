# Discorsa
`Placeholder repo for Discorsa` 
___
Now this isn't just one app, it's a collection. There's a bot, there's a webserver, there's a mod, there will probably be a better website in the future...\
Because of this, I've split them into multiple repositories to make it easier to collaborate and deploy those apps. None of the actual repositories will be made public, instead this "frontpage" repo will be used for [new releases](https://github.com/Hypurrnating/Discorsa/tags), [tracking issues](https://github.com/Hypurrnating/Discorsa/issues), and [hosting the page](https://hypurrnating.github.io/Discorsa/) obviously, in addition to making some of the apps readable to the public, such as the mod clients.

If you have any questions, or need help, there's a [discord server](https://discord.gg/DPTCrxawBx) just for that.

\
At the moment, the mod doesn't do a lot. Mainly relays your lap times to a server, where they are saved and sent to discord.\
I plan on expanding it to include more detailed data about each lap. This is a tricky thing to do since:
- Processing data from [AC Python Doc](https://docs.google.com/document/d/13trBp6K1TjWbToUQs_nfFsB291-zVJzRZCNaTYt4Dzc/pub), and Shared Memory Reference is a *little* tricky
- Assetto Corsa is using python version 3.3 (and don't get me started on importing modules)
- Worst: Assetto Corsa is a client sided game, and I am writing a client sided mod. This is notoriously horrible for security.

## To do:
- [ ] Fix Lap Invalidation https://github.com/Hypurrnating/Discorsa/issues/1
- [ ] Include feedback about connection with server from transmitter to user in game
  - [ ] on_start event to check for a working connection: `(On hold: Requires rewriting the the transmitter)` 
  - [x] Retry sending data in case it fails
  - [x] Save data it couldn't send and retry on next startup
- [ ] Move from using webhooks to using the bot.
  - [ ] Configure private networking between bot and server
  - [ ] Add command for managing the channels to send messages to
    - [ ] Also include a `try except` that removes a channel from settings it can not access (preferrably done when the message actually has to be sent)
    - [ ] ofc enable sending to multiple channels
  - [ ] Command to flip sending calls on and off
- [ ] Various security features

### Planned for the future:
- [ ] **Duels**: A feature that allows users to set a car, track, and time for time attack like sessions. Players would not need to join a server for this, and can set laps at their own schedule, at their own pace.
  - [ ] Spinoff modes that include teams/ffa
- [ ] **Link**: Share a code with somebody to have a session without joining a server. Players who join will have live information about others shared in game 
