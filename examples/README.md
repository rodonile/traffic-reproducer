# Traffic Reproducer Examples

### Examples:
```
python main.py -v --cfg examples/bmp-traffic.yml
python main.py -v --cfg examples/ipfix-traffic.yml --no-sync                           # reproduce right away (don't wait next minute)
python main.py -v --cfg examples/ipfix-bmp-scenario-segmented.yml --ask-for-input      # ask user input before reproducing each pcap file
python main.py -v --cfg examples/bgp-traffic.yml --keep-open                          # keep tcp connection open (don't exit reproducer after finishing)
```

### If root necessary (e.g. need to send through vrf interface):

```
sudo env PATH="$PATH" python main.py -v --cgf examples/nfv9-traffic.yml
```
