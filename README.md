# Miner Search

This program is designed to find and destroy hidden miners.
It is an auxiliary tool for searching suspicious files, directories, processes, etc. and is NOT an antivirus.

## News about updates now in the Telegram!
https://t.me/MinerSearch_blog

## NET Framework 4.7.1 is required

-----------------------------------------

## How to use

Completely unzip the archive with the program into a separate folder and launch the application. Wait for the scan to complete. When using the program for the first time, you are offered to report the results of the scan to the author at your wish. After completion, a form will be shown with a brief report on the threats that have been eliminated. You can view the detailed log by clicking on the "Show log" button. Clicking on the "Quarantine" button will open the Quarantine Manager, in which you can completely delete the file or restore it.

The application also supports additional launch parameters (listed below). To use them, you should:
1) Run the command line (cmd) as administrator
2) Hold down shift and right-click on the application - select "Copy as path"
3) Paste the path into the command line and add the necessary parameters* after a space

Additional command line args (usually is not required):

| Startup params | Description |                                                                                                           
|----------------|-------------|	                                                                                                          
| -h     --help                | This help message                                                                                        |
| -nl    --no-logs             | Don't write logs in text file                                                                            |
| -nstm  --no-scantime         | Scan processes only                                                                                      |
| -nr    --no-runtime          | Static scan only (Malware dirs, files, registry keys, etc)                                               |
| -nse   --no-services         | Skip scan services                                                                                       |
| -nss   --no-signature-scan   | Skip scan files by signatures                                                                            |
| -nrc   --no-rootkit-check    | Skip checking rootkit present                                                                            |
| -p     --pause               | Pause before cleanup                                                                                     |
| -ret   --remove-empty-tasks  | Delete a task from the Task Scheduler if the application file does not exist in it                       |
| -so    --scan-only           | Display malicious or suspicious objects, but do nothing                                                  |
| -fs    --full-scan           | Add other entire local drives for signature scan                                                         |
| -ras   --run-as-system       | Start scannning with SYSTEM privilege (for advanced users)                                               |
| -s     --select              | Only selected folder will be scanned, including subfolders                                               |
| -si    --silent              | Enables silent (background) mode without any dialog forms. The app switches to background mode, messages will not be displayed, but will still be written to the log file. Incompatible with --select or --winpemode options |
| -d=    --depth=<number>      | Where <number> specify the number for maximum search depth. Usage example -d=5 (default 8)               |
| -v     --verbose             | Displays more info to the console and a log file,                                                        |
|                              | including lines about files that are not considered malicious. It may increase the size of the log file. |
| -w     --winpemode           | Start scanning in WinPE environment by specifying a different drive letter                               |
|                              | (without scanning processes, registry, firewall and task scheduler entries)                              |

* Not necessarily in strict order
--------------------------------------------------------------

Symbols in logs

| Hint | Description |
|-----------|----------|
|    [!] | Minor warning |
| [!!] | A warning worth paying attention to |
|  [!!!] | Threat detected |
| [!!!!] | A rootkit has been detected |
| [Reg] | Scan the registry key(s) |
|    [+] | Successful completion of the action (treatment, removal, etc.) |
|    [x] | Error |
| [xxx] | Critical error: for example, when running in the sandbox |
|    [#] | Status |
| [.] | Description |
|    [_] | Unblocking the directory and deleting if empty |
| [i] | Info |
|    [$] | Scan elapsed time |

----------------------------

# Demo

## Screenshots
Stop and remove malicious processes and his support components, that makes deletion malware harder
![first](https://github.com/user-attachments/assets/29828484-6d57-4e71-ad5c-641913ce34f7)

Final report form
![second](https://github.com/user-attachments/assets/309e7625-bc57-4b80-9052-4805c33f9486)


