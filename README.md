# adrien-overlay-testing

## IMPORTANT

This overlay is NOT stable. Used for me to test updates of MATE before push to calculate-linux repository.
Ebuild with sources from http://pub.mate-desktop.org/releases/

## Install

### With "simple" portage :

Make sure /etc/portage/repos.conf directory exists and git installed.

*curl https://raw.githubusercontent.com/aaaaadrien/adrien-overlay-testing/master/repo.conf -o /etc/portage/repos.conf/adrien-overlay-testing.conf*

### With Layman

*curl https://raw.githubusercontent.com/aaaaadrien/adrien-overlay-testing/master/repositories.xml -o /etc/layman/overlays/adrien-overlay-testing.xml*

*layman -S*

*layman -a adrien-overlay-testing*

## Note for Calculate Linux

To enable updates from my overlay, set to ON the cl_update_other_set with

*cl-core-variables --set update.cl_update_other_set=on*
