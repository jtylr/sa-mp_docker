# Docker for sa-mp

**Note**: Although SACNR still uses this for now, it's not being maintained and there are more than definitely better options out there. We'll be moving over to [sampctl](https://github.com/Southclaws/sampctl) by [Southclaws](https://github.com/Southclaws/) whenever is convenient and after testing has been completed.

<hr>

Tested with 0.3.7 R2-2

## Instructions

1. Check out this project
2. Place your sa-mp files into the `samp03` directory
3. To build the image run `docker build -t sa-mp .`
4. Start the container with `docker run --net=host -v samp03:/samp sa-mp`

Your server should now be running within the docker container.

## Caveats

- This isn't a very well optimised image, it just shares the sa-mp volume with the container. This can be particularly slow on OS X hosts.
- Nothing is back in the docker registry. Maybe one day.
