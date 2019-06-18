# cli-utils
cli utilities

# installation

copy the contents of the "bin" folder to /usr/local/bin

i guess it would be appropriate to set the permissions to 0555 and the owner to root:root as well.


here is a little install script: 

```git clone --depth 1 https://github.com/divinity76/cli-utils.git && sudo chown -Rv root:root cli-utils/bin/* && sudo mv -v cli-utils/bin/* /usr/local/bin/ && rm -rfv cli-utils/ && echo "OK INSTALLED"```

# documentation

pingport: pings TCP ip:port until it responds, then starts beeping. (useful when waiting for a server to restart)

countdown: counts down the specified time, for example "countdown 1 hour" -> counts down 1 hour, and prints the current number of seconds remaining

alarm: optionally prints a message, and beeps forever.


# requirements 

php-cli >= 7.0.0
