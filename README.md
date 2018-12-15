#webgrabUpdateChannels

Updating channels indices (siteini.pack) for webgrab++

# Example

The dummy WebGrab++.config.xml file must be located into the config folder

```bash
docker run -it --rm -e PAT="GitHub_Personal_Access_Token" \
-v "$(pwd)/config:/config" \
-v "$(pwd)/data:/data" \
--entrypoint="/defaults/updateChannels.sh" \
synker/webgraboneshot:latest
```
