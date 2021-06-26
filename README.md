# YAGPDB counter
A set of custom commands to create a Discord counting channel with YAGPDB

## Installation
In case you need a refresher, or don't know how to add a custom command, please read [this tutorial](https://learn.yagpdb.xyz/the-custom-command-interface).

Copy each `.go.tmpl` file to a new custom command.

Details about the commands are located at the top of each file, as well as below.

## Components
| Command/trigger                    | Trigger type | Restrictions                 | Description                                           |
| ---------------------------------- | ------------ | ---------------------------- | ----------------------------------------------------- |
| [`\A`](main.go.tmpl)               | Regex        | Only run in counting channel | Main trigger, verifies the number                     |
| [`count`](count.go.tmpl)           | Command      | None                         | Shows the next number                                 |
| [`count top`](count_top.go.tmpl)   | Command      | None                         | Shows the leaderboard of users who counted the most   |
| [`count set`](count_set.go.tmpl)   | Command      | Moderators only              | Sets the last counted number                          |
| [`count user`](count_user.go.tmpl) | Command      | Moderators only              | Sets number of times a user counted (for leaderboard) |
