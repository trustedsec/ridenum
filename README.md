# RID_ENUM - A simple open source method for performing null session brute forces
Copyright 2014 TrustedSec

Written by: David Kennedy (ReL1K)
Twitter: @dave_rel1k and @TrustedSec
Website: https://www.trustedsec.com

.______       __   _______         _______ .__   __.  __    __  .___  ___. 
|   _  \     |  | |       \       |   ____||  \ |  | |  |  |  | |   \/   | 
|  |_)  |    |  | |  .--.  |      |  |__   |   \|  | |  |  |  | |  \  /  | 
|      /     |  | |  |  |  |      |   __|  |  . `  | |  |  |  | |  |\/|  | 
|  |\  \----.|  | |  '--'  |      |  |____ |  |\   | |  `--'  | |  |  |  | 
| _| `._____||__| |_______/  _____|_______||__| \__|  \______/  |__|  |__| 
                            |______|                                       


Rid Enum is a RID cycling attack that attempts to enumerate user accounts through null sessions and the SID to RID enum. If you specify a password file, it will automatically attempt to guess the user accounts when its finished enumerating.

- RID_ENUM is open source and uses all standard python libraries minus python-pexpect. -

Example: ./rid_enum.py 192.168.1.50 500 50000 /root/dict.txt

Usage: ./rid_enum.py <server_ip> <start_rid> <end_rid> <optional_password_file>

