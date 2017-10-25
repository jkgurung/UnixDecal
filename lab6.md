### Lab 6 - Processes and Services

### Overview

At any given time, there are dozens of processes running on a Unix server. Most of these processes run in the background. Today we’ll explore these background processes and how we can control them.

Make sure you are doing all of these exercises on your VM.

#### Which processes are running on my system?

Open up a terminal and run the __ps__ command. You should see something like this:
```
  PID TTY          TIME CMD
14195 pts/1    00:00:00 bash
15289 pts/1    00:00:00 ps
```
As you can see, ps displays itself in the list. This is because ps displays the processes which are running at the time it runs, which includes itself.

Now run sleep 100 in the background and then run ps. Now you should see something like:
