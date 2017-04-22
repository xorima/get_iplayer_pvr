# get_iplayer_pvr
get_iplayer running the pvr by default with output to /data/output/(tv,radio)/name/series
Works well with get_iplayer_web

Example Run commands:
docker run --name iplayer_pvr -v /data/iplayer/:/data -v /data/mount/media/test/:/data/output -d jasonfield/get_iplayer_pvr
docker run --name iplayer_web -v /data/iplayer/:/data -p 1935:1935 -d jasonfield/get_iplayer_web
