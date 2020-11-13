Supported tags and respective `Dockerfile` links
================================================

  * [`latest`](https://github.com/coolfeather2/docker-youtube-dlc/blob/master/Dockerfile) [![](https://images.microbadger.com/badges/image/coolfeather2/youtube-dlc.svg)](http://microbadger.com/images/coolfeather2/youtube-dlc "Get your own image badge on microbadger.com")


What is youtube-dlc?
==================

[youtube-dlc](https://github.com/blackjack4494/yt-dlc) is a command-line program to download videos from YouTube.com and other video sites.


How to use this image
=====================

    $ docker run --rm --user $UID:$GID -v $PWD:/downloads coolfeather2/youtube-dlc \
          <video_url>

  * `--user $UID:$GID` is to run as your current user, and not `root`.
  * `-v $PWD:/downloads` is to store downloaded files in the current working directory.
  * `<video_url>` is the ID of a YouTube video or other arguments to pass to `youtube-dlc`.

Note: The entrypoint is set to `youtube-dlc`, so do *not* put `youtube-dlc` again as argument.

Features of this image
----------------------

  * **Small**: Built based on official [Alpine Linux](https://registry.hub.docker.com/_/alpine/).
  * **Simple**: One command and you should be ready to go. All documented here.
  * **Secure**: Runs as any user.


User Feedback
=============

Having more issues? [Report a bug on GitHub](https://github.com/coolfeather2/docker-youtube-dlc/issues).
