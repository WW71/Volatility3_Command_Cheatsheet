### Reference the `file`, specify the `dir` you want the output dump files to go to, select the `windows.dumpfile` plugin, referencing the `ProcessID` identified via `psscan`, specifically selecting the file in memory `virtaddr` identified via `windows.handle`
python vol.py -f <file> -o "<dir>" windows.dumpfile --pid <pid> --virtaddr <offset>
