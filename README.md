# Realtime Merge
Check for automated tool for merge conflicts.

Realtime Merge Project:

Functionalities Given:

1. Multiple Users can read and write at same time and can do changes in realtime and see conflicts with other people working on same file.
2. You also have an option to select a specific group of users with whom you want to compare.
3. I should be able to solve the conflicts by own and show all of them with their severity levels.
4. Option of real time chatting between people if they want to collaborate (Option to Select Multiple User by One)
5. Storage of all chnages in DB in case of any failures so they should not loose any changes.
6. Good Usage of websocket need to be there with session management.
7. Functions of cloud sync like we will keep on doing autosave but it will sync between cloud without any data loss.
8. Usage of Indexed DB to store all local data of users and as soon as this upload to cloud then it will clearly be deleted to maitain free space.

Very Important.

1. There should be an options to enable and disable features otherwise it may frustrate the end user.
2. There should be timer invloved at top where user can check for changes like after every 2 sec - 10 sec etc.


Tech Stack:

Websocket + Vanilla JS + Code Mirror , Monanco Code Editor + Database + CRDT + Auto running diff algorithm in background.

Limits--

Restirct number of active users working on same file i.e 15 users or 20 users per file.

Questions--

1. How to keep sync operation real and intact after introduction of time delay.
2. Time Delay is important and extensive thing to work on.
3. Usgae of database how we should store code or other code snipptes.
4. Make UI flawless without any lag.
5. Do we need authentication (yes) we will start with concept of putting name and organization ID under one hood all things should be placed.
6. Concept to add triggers to delete all caches accordingly to avoid database issue.
7. Make your payload size small so we can send data to cloud without any delay.
