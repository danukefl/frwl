# frwl
From Russia With Love Content

Contents of this repository are my contributions to the From Russia With Love project.

https://github.com/LogoiLab/frwl
https://www.reddit.com/r/DataHoarder/comments/apsd7v/with_russia_going_offline_for_a_test_some_time/

I have included my dockerfile for anyone to modify to their tastes as it current running off the debian base iamge, or to build and run for themselves to help in contributing.


docker run -d \
  --name frwl \
  -v <local volume>:/from_russia_with_love_comp \
  -e ServerIP=<Ru Server IP/Host> \
  danukefl/frwl
