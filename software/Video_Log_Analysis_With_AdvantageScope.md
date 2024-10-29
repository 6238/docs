# Reading Robot Code Logs and Syncing With Match Video

Here's how to open an FRC match log file and sync it up with video using AdvantageScope:

1. Get a The Blue Alliance API key at https://www.thebluealliance.com/account. Sign in, scroll down to "Read API Keys", and generate a new key or copy an existing one. Paste it in AdvantageScope's preferences (Cmd/Ctrl + Comma).
1. Open AdvantageScope (it's in `[your WPILib install directory]/advantagescope`) and open the log file from the match. If you have multiple separate logs from the same match (DSLog, DSEvents, WPILog, and/or Hoot), use <kbd>Cmd/Ctrl + Shift + O</kbd> to select multiple files. 
1. Wait for AdvantageScope to load the log file - you'll see all your logged values appear in the sidebar when it's ready.
1. Open a Video tab with the + button at the top right of the window.
1. Click the blue The Blue Alliance button at the bottom of the window to automatically load the video from TBA. If TBA doesn't have the video, find it on the FRC YouTube channel, copy the URL, and click the red clipboard button to load the video. You can also use your own video with the gray file button.
1. Wait while AdvantageScope automagically loads and syncs the video. If the video has a score overlay and AdvantageScope can detect it, there should be a lock icon next to the video controls at the bottom right once all the video is loaded. If there isn't, you'll have to manually synchronize it:

    1. First, move your log playhead (at the top of the screen) to an easy-to-identify point. The arrow to the left of the scrubber will let you jump to the first point the robot was enabled (typically the start of auton).
    1. Then move the video playhead at the bottom of the window to the same point. If you used the start of auton, look for the stack lights above the driver glass turning on. You can use the arrow keys to more precisely sync.
    1. Once you're happy with how it's synced up, click the lock next to the video controls to lock the synchronization.

1. Now you can replay your logs to your heart's content. Click the play button in the top bar to start the playback. You can pop out the video by clicking the "new window" icon to the far right of the window, next to the log scrubber. 

> For example, if you'd like to compare your odometry with the robot's physical position, open an Odometry tab from the + menu at the top, then drag your Field2d into the list of poses. 