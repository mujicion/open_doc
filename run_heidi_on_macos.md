    socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\" &
    docker run -ti --rm -e DISPLAY=docker.for.mac.host.internal:0 tsari/heidisql
