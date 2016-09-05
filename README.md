# RID_ENUM - A simple open source method for performing null session brute forces

Copyright 2016 TrustedSec

+ Written by: David Kennedy (ReL1K)
+ Twitter: @HackingDave and @TrustedSec
+ Website: https://www.trustedsec.com

```
.______       __   _______         _______ .__   __.  __    __  .___  ___.
|   _  \     |  | |       \       |   ____||  \ |  | |  |  |  | |   \/   |
|  |_)  |    |  | |  .--.  |      |  |__   |   \|  | |  |  |  | |  \  /  |
|      /     |  | |  |  |  |      |   __|  |  . `  | |  |  |  | |  |\/|  |
|  |\  \----.|  | |  '--'  |      |  |____ |  |\   | |  `--'  | |  |  |  |
| _| `._____||__| |_______/  _____|_______||__| \__|  \______/  |__|  |__|
                            |______|

Written by: David Kennedy (ReL1K)
Company: https://www.trustedsec.com
Twitter: @TrustedSec
Twitter: @HackingDave

Rid Enum is a RID cycling attack that attempts to enumerate user accounts through
null sessions and the SID to RID enum. If you specify a password file, it will
automatically attempt to brute force the user accounts when its finished enumerating.

- RIDENUM is open source and uses all standard python libraries minus python-pexpect. -

You can also specify an already dumped username file, it needs to be in the DOMAINNAME\USERNAME
format.

Example: ./ridenum.py 192.168.1.50 500 50000 /root/dict.txt

Usage: ./ridenum.py <server_ip> <start_rid> <end_rid> <optional_password_file> <optional_username_filename>
