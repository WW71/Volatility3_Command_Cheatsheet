### Check for processes running ###
```
python vol.py -f <file> windows.psscan
```

### Grab the file in memory dump ###
```
python vol.py -f <file> -o "<dir>" windows.dumpfile --pid <pid> --virtaddr <offset>
```
*Reference the `file`, specify the `dir` you want the output dump files to go to, select the `windows.dumpfile` plugin, referencing the `ProcessID` identified via `psscan`, specifically selecting the file in memory `virtaddr` identified via `windows.handle`*

### Handy Windows plugins ###
```
windows.cmdline
```
*Check for command line executions*
```
windows.netscan
```
*Check for network activity. Haven't tested yet*

**Profile not required anymore in Volatility3. Use windows/linux/mac in the plugin command straight away**
