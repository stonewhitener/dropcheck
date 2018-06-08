# dropcheck

For Interop Tokyo 2018


## Requirements

- macOS
- iproute2mac
- wget
- screen
- mtr


## Usage

```
# Download this script and make executable
curl -Lo dropcheck https://raw.githubusercontent.com/y-sira/dropcheck/master/dropcheck
chmod +x dropcheck

# Check the target interface (e.g. en0)
ip link | grep 'UP'

# Turn off interfaces except for the target interface
ip link set en1 down
ip link set en2 down
...

# Run tests
./dropcheck en0
```
