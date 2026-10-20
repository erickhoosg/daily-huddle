# Daily Huddle

A shared workspace for a team of up to ten, built as a Claude artifact.

## Features

- **Today:** each person posts their daily tasks and moves them through To do, In progress and Done. Unfinished tasks carry over, and a Team progress panel shows everyone's tasks.
- **Message of the day:** the team leader posts up to five messages at the top of the Today page. Teammates hear a chime when a message is added or changed, and each person can turn the sound off.
- **Calendar:** a month view of who's away. Entry types are On leave, Out of office, Working remotely, Busy, Blackout period, Propose downtime and Patching.
- **Chat:** each member has a private conversation with the team leader.
- **Team:** shows the ten seats, each person's role and today's status. The leader can remove members to free seats.

## How it runs

`daily-huddle.html` is published as an artifact on claude.ai and uses the artifact runtime's `db` and `user` capabilities, so all data syncs live between teammates.

- Each teammate signs in with their own Claude account. The artifact owner becomes the team leader.
- The leader shares the artifact with teammates as **Contributors** so they can save data.
- Access rules keep each member's chat visible only to that member and the leader. Each person can change only their own tasks and calendar entries.

Opened directly in a browser outside Claude, the page shows its sign-in screen but can't load or save data, because the data store is provided by claude.ai.
