# geogroup
matchmaking for matchmakers 

Gotchas:
npm ENOSPC: 
execute `echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p`
(https://stackoverflow.com/a/32600959)