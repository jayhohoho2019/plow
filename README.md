Replow 
For replotting, which involves removing old plots.

Based on the Plow below. 
Added functions to check available free space on remote destination, and remove a certain number of c0 plots to free up space in destination (local and remote). 


# 🚜 The Plow

An efficient Chia Plot mover.

Uses `inotify` to watch for new Chia plots and then fires off `rsync` to move
them to their final destination.

It can do many in parallel, one at a time, one per source, or one per destination.
