[![](https://raw.githubusercontent.com/sayak-brm/haos-emby-addon-repo/main/logo.png)](http://emby.media/)

# Emby

An Emby media server add-on for Home Assistant.

# What is Emby?

Emby Mediaserver automatically streams (and transcodes, if needed) your media
on-the-fly to play on any device.

# How to use this add-on

When started the emby web interface will listen on port 8096 in the container and 8096 by default on the host.

Place your media in /share or /media; or mount a CIFS share. The config files are stored in the /data folder in the addon and will be backed up with a snapshot. It is suggested to move the cache, transcode temp, and metadata to /share, /media, or NAS as well; you can do this on the Emby media server configuration page. If you do not move the cache files they will be backed up with snapshots and create very large snapshots. You can migrate an existing instance of Emby by copying the config to the add-on data folder if you have access, or you can use Emby's built-in config backup/restore feature.

Based on [emby/embyserver](https://registry.hub.docker.com/r/emby/embyserver) docker image
