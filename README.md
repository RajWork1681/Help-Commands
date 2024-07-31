Commands 📜
Before you continue 🧐

Commands denoted by 🐱‍👤 are privileged meaning the user must have a role named bBot to be able to use that command.

Commands denoted by 😸 can be used by everyone.

General
register 🐱‍👤
Usage -> .register

Registers your discord server with bBot. This is the first command you should be using after the bot is invited to your discord server.

setpugchannel 🐱‍👤
Usage -> .setpugchannel

Typing this command in a channel will mark that channel to be used for pug commands.

setquerychannel 🐱‍👤
Usage -> .setquerychannel

Typing this command in a channel will mark that channel to be used for query commands.

ignorecommandgroup, igc 🐱‍👤
Usage -> .ignorecommandgroup group

All ignorable commands are classified into 2 groups, namely, pugs and queries. If for instance you do not want query commands from the bot and only care about the rest of it then you can ignore the queries group.

unignorecommandgroup, uigc 🐱‍👤
Usage -> .unignorecommandgroup group

To unignore a command group which was previously ignored.

warn 🐱‍👤
Usage -> .warn @mention#0000 reason

Warns an user. Simultaneously, creates a log entry for auditing purposes.

logs 🐱‍👤
Usage -> .logs @mention#0000

Shows the last 10 logs of the mentioned user.

invite 😸
Usage -> .invite

Generates an invite for your server with no expiry and unlimited uses. If such an invite already exists, it re-uses that.

Pugs
addgametype, agm 🐱‍👤
Usage -> .addgametype name totalPlayers totalTeams

Creates a new gametype which can be now pugged.

Note that totalTeams must be less than 4 due to UT99 supporting 4 team colors only OR mix if it's a mix gamemode

deletegametype, dgm 🐱‍👤
Usage -> .deletegametype name

Deletes an already present gametype.

Note that if there is atleast 1 user joined for the gametype then this command will not work until the list is cleared.

defaultjoin 😸
Usage -> .defaultjoin gametype1 gametype2 etc

Stores your default preference for joining pugs

list, ls 😸
Usage -> .list gametype or .list

There are 2 versions of this command, with gametype and without.

If gametype is mentioned then it will show all the users who have currently joined the gametype
If gametype is not mentioned then it will summarise all the gametypes with their names and a count of number of players joined / max players
liast 😸
Usage -> .liast

Combination of list and last.

lsa 😸
Usage -> .lsa

Shows the list of all gametypes with users who present.

join, j 😸
Usage -> .join gametype or .j

There are 2 versions of this command, with gametype and without.

If gametype is mentioned then it will join that particular gametype.
If gametype is not mentioned then it will join all gametypes saved in your default join preferences.
leave, lv, l 😸
Usage -> .leave gametype

Removes yourself from the gametype.

lva 😸
Usage -> .lva

Removes yourself from all gametypes that you've joined.

promote, p 😸
Usage -> .promote gametype or .promote

There are 2 versions of this command, with gametype and without.

If gametype is mentioned then it will promote that particular gametype.
If gametype is not mentioned then it will promote all gametypes with atleast 1 user joined sorted by the least number of users required to fill that pug.
Since this command makes use discord's @here usage, then in order to counter spam, users can be given a COOLDOWN role which will prevent them from using the command once every 120 seconds.

captain, capt 😸
Usage -> .captain

Adds you to the list of captains of the filled pug. Team color is RNG.

picking 😸
Usage -> .picking

Shows the current picking states of filled pug(s).

pick, p 😸
Usage -> .pick index index2(?)

Picks at the user at the mentioned index and add them to your team. index2 can be specified if bot asks you to pick 2 players.

💲 Bonus Usage 💲 You can do a random pick by typing random instead of the index.

tag 😸
Usage -> .tag info

Adds meta information about yourself in all the pugs you've joined.

For example if you have no microphone then you can tag yourself .tag nomic. This will help the captains later while picking and making a decision.

stats 😸
Usage -> .stats or .stats @mention#0000

There are 2 versions of this command, with mentioned user and without.

If user is mentioned, then it will show the stats of the mentioned user.
If user is not mentioned, then it will show your own stats.
last 😸
Usage -> .last gametype or .last

There are 2 versions of this command, with gametype and without.

If gametype is mentioned, then it will show the last pug played for that specific gametype.
If gametype is not mentioned, then it will show the last pug played irrespective of any gametype.
💲 Bonus Usage 💲 You can go beyond last by specifying a number after last like last3 or add that many t characters like .lasttt

top10played 😸
Usage -> .top10played gametype

Generates an image of top 10 puggers for the gametype (sorted by most number of pugs played for the gametype).

pugstats 😸
Usage -> .pugstats

Outputs a summary of total number of pugs played, individual pug count(s) and a timestamp when the first pug was played

autoremove, ar 😸
Usage -> .autoremove expiry(?)

Automatically removes the user from all the pugs they have joined after expiry. Note that If no expiry is provided, it clears your autoremoval request (if any).

⏲ Expiry Parameters ⏲ m for minutes or h for hours or d for days.

For example, .autoremove 30m will automatically remove the user from all the pugs after 30 minutes. .autoremove will clear your autoremoval request.

add 🐱‍👤
Usage -> .add @mention#0000 gametype1 gametype2 etc

Adds the mentioned user to the list of specified gametypes.

remove 🐱‍👤
Usage -> .remove @mention#0000 gametype1 gametype2 etc

Removes the mentioned user from the list of specified gametypes.

forcepick 🐱‍👤
Usage -> .forcepick @mention#0000 index

Picks the player at the specified index for mentioned user's team.

reset 🐱‍👤
Usage -> .reset pugname

Resets the pug back into picking mode if it was filled.

block 🐱‍👤
Usage -> .block @mention#0000 duration reason

Blocks the mentioned user from joining pugs for a certain period of time.

⏲ Duration Parameters ⏲ m for minutes or h for hours or d for days. For example, .block @mention#0000 1d xyz reason will block the mentioned user for 1 day.

unblock 🐱‍👤
Usage -> .unblock @mention#0000

Unblocks the mentioned user.

showblocked 🐱‍👤
Usage -> .showblocked

Shows the list of blocked users.

blockcaptain/blockcapt 🐱‍👤
Usage -> .blockcaptain @mention#0000 reason

Blocks the mentioned user from becoming a captain in pugs.

unblockcaptain/unblockcapt 🐱‍👤
Usage -> .unblockcaptain @mention#0000

Unblocks the mentioned user from becoming a captain in pugs.

showblockedcaptain/showblockedcapt 🐱‍👤
Usage -> .showblocked

Shows the list of blocked captains.

enablecoinflip 🐱‍👤
Usage -> .enablecoinflip gametype

Enables coin flip feature for the specified gametype (for mapvote purposes).

When the picking finishes, it will randomly decide which team won mapvote.

disablecoinflip 🐱‍👤
Usage -> .disablecoinflip gametype

Disabled coin flip feature for the specified gametype.

teamemojis 🐱‍👤
Usage -> .teameojis emoji gametype

Sets the preferred teamemoji for the gametype. emoji can be one of agonies, cores or logos.

Note that if gametype is omitted then the default is change it for ALL gametypes.

setpickingorder 🐱‍👤
Usage -> .setpickingorder gametype pickingOrder

Enforces a custom picking order for the gametype. An example of a picking order for a gametype with 2 teams is 1 2 2 1 1 2 2 1. It goes like Red picks first, then blue picks 2 times then red picks 2 times then blue picks 2 times and finally last pick goes to red

Red - 1
Blue - 2
Green - 3
Gold - 4
Note that this command does not work for DUEL/MIX/DM gametypes.

Queries
addqueryserver, aqs 🐱‍👤
Usage -> .addqueryserver address name

Adds a query server to the list of query servers.

deletequeryserver, dqs 🐱‍👤
Usage -> .deletequeryserver index

Deletes the query server at the specified index from the list.

editqueryserver, eqs 🐱‍👤
Usage -> .editqueryserver index attribute newValue

Edits the query server at the specified index in the list.

📑 Attributes 📑 name for editing name, address for editing address.

servers, server 😸
Usage -> .servers

Shows the list of query servers.

query, q 😸
Usage -> .query index or .query customAddress

There are 2 versions of this command, with index and with custom address.

If index is specified, it will query the query server's address at the specified index.
If custom address is specified, it will query that specific address.
ip 😸
Usage -> .ip index

Prints the address of the query server at the specified index in the list.
