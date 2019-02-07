# WebgrabUpdateChannels

[![Build Status](https://travis-ci.org/Fazzani/webgrabUpdateChannels.svg?branch=master)](https://travis-ci.org/Fazzani/webgrabUpdateChannels)

Updating channels indices (siteini.pack) for webgrab++

## Example

The dummy WebGrab++.config.xml file must be located into the config folder

```bash
docker run -it --rm \
-e PAT="GitHub_Personal_Access_Token" \
-e WEBGRAB_URL="https://gist.githubusercontent.com/Fazzani/cce67905b458bae3eb5818adeffd2510/raw/WebGrab++.config.xml" \
-v "$(pwd)/config:/config" \
-v "$(pwd)/data:/data" \
--entrypoint="/defaults/updateChannels.sh" \
synker/webgraboneshot:latest
```

```powershell
docker run -it --rm `
-e PAT="${env:PAT_PERSO}" `
-e WEBGRAB_URL="https://gist.githubusercontent.com/Fazzani/cce67905b458bae3eb5818adeffd2510/raw/WebGrab++.config.xml" `
-v "$(pwd)/config:/config" `
-v "$(pwd)/data:/data" `
--entrypoint="/defaults/updateChannels.sh" `
synker/webgraboneshot:latest
```
