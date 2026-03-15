# Brute Force Login Detection

Splunk Query:

index=windows_lab EventCode=4625
| stats count by Source_Network_Address Account_Name
| where count > 5
