frwl
===

From Russia With Love Content
---

https://hub.docker.com/r/danuke/frwl

Contents of this repository are my contributions to the From Russia With Love project.

https://github.com/LogoiLab/frwl
https://www.reddit.com/r/DataHoarder/comments/apsd7v/with_russia_going_offline_for_a_test_some_time/

I have included my dockerfile and modified ping_russia_docker.sh script for anyone to modify to their tastes as it current running off the debian base image, or to build and run for themselves to help in contributing.


Command
---

docker run -d \
  --name frwl \
  -v "localvolume":/from_russia_with_love_comp \
  -e ServerIP="IP/Host" \
  danukefl/frwl


-v "localvolume":/from_russia_with_love_comp
Creates a persistent container on your host so that completed tarballs can be saved.

-e ServerIP="IP/Host"
Pass server IP or hostname to ping in the script.


The ping_russia_docker.sh script has added the arguement variable to the server declaration so that it is passed and not hard set.
SERVER="" #insert any server IP here > SERVER="$1" #insert any server IP here
