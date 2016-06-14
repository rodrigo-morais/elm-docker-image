elm
==================

Docker image with the Elm's 0.17.0 version installed.

Docker hub: https://hub.docker.com/r/morais/elm/

Usage
------------
First, is necessary to run a container based on this image:

docker run -it -rm -p 8000:8000 morais/elm

This container will run as default with the command `elm-reactor`. The code could be accessed in port `8000`. Is possible send another Elm command to the container as `repl`.

docker run -it -rm -p 8000:8000 morais/elm elm-repl

This image is expecting the file `elm-package.json` on the root and the code in `src` directory.