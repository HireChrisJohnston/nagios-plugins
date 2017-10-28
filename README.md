# nagios-plugins
Nagios plugins that are good for general purpose or are for 3rd party providers

# [check_adrive_usage.php](check_adrive_usage.php)
Nagios plugin for checking ADrive disk usage using the API.  Refer to API reference regarding API access restrictions based on account type. Outputs Nagios performance data and alerts based on the thresholds defined(optional) as a whole number represneting a percentage,  without using the '%'. 

## Example:
* Username and password are required
* Warning and Critical varibles are optional 

By default 90% warning and 97% is critical
PS C:\foo>.\check_adrive_usage.php  user@email.com UserPasword

PS C:\foo>.\check_adrive_usage.php  user@email.com UserPasword -warn 90 -crit 97
