---
title: New sites list and syncing fixes
type: minor
---

This week's deployment focuses on usability changes to the sites list. Site names are no longer required to be unique with the exception of Dropbox connected sites. Storage provider details are displayed on the sites list to help distinguish between environments. If a site icon contains transparency it will be displayed with a padding around it. Alternatively if the site icon has no transparency the image will be shown to the edge its wrapper.

![Empty blogging interface](/img/change-log/new-sites-list.png){: .screenshot srcset="/img/change-log/new-sites-list.png 800w, /img/change-log/new-sites-list@2x.png 1600w"}

Syncing improvements ensure that sites stay synchronised when reconnected. When connecting a Git repository, all files on CloudCannon are reset to the state on the selected branch.

Features:

* New sites list design.
* Site icon pixel reading to optimise viewing.
* Videos and audio files are served from a CDN.


Fixes:

* Resetting a connection will delete files in CloudCannon. This often left sites in an intermediate state.
* Syncing with GitHub or Bitbucket no longer syncs the&nbsp;`_site`&nbsp;and `node_modules` directories.