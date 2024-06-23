# LANIFY
An unofficial Docker Image for [app.lanify.ai](https://app.lanify.ai/register?ref=kDEOfkxHgs3qVAQ)
Available on [Docker Hub](https://hub.docker.com/r/double2tbinhnv56rouble/lanify)

## What's LANIFY?
LANIFY allows you to earn passive income by sharing your network bandwidth

## How to get started?
1. Register a LANIFY Account if you don't have one already: [app.lanify.ai](https://app.lanify.ai/register?ref=kDEOfkxHgs3qVAQ)
2. Either build this image from source, or download it from Docker Hub
3. Set envriomental variables to their respective values: LANIFY_USER and LANIFY_PASS
4. You're good to go! Once started, the docker exposes your current network status and lifetime earnings on port 80

### Docker Run Command
```
docker run -d \
    --name lanify \
    -p 8080:80 \
    -e LANIFY_USER=myuser@mail.com \
    -e LANIFY_PASS=mypass \
    -e ALLOW_DEBUG=True \
    -e IMGUR_CLIENT_ID=your_client_id
    binhnv56/lanify:latest
```

Please replace 8080 with the port you want to be able to access the status with, as well as LANIFY_USER and LANIFY_PASS

## Separate thanks
I would like to mention [kgregor98](https://github.com/kgregor98/grass) and his project Grass for inspiring me to create this.


## License
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.


