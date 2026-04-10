# Ticket 002 - Network Connectivity Failure

# Scenario
The user is connected to WiFi but unable to access the internet.

# System Context
Windows 10, wireless connection

# Investigation
- Verified WiFi connection status
- Attempted to access multiple websites
- Ran `ipconfig` to check IP configuration
- Used `ping google.com` to test connectivity

# Diagnosis
The network adapter was disabled, preventing proper connectivity.

# Action Taken
Re-enabled the network adapter and renewed IP configuration:
- ipconfig /release
- ipconfig /renew

# Result
Internet access restored successfully.

# Reflection
Effective network troubleshooting starts with checking adapter status before moving to command-line diagnostics.

# Validation
- Verified internet access by loading multiple websites
- Successful response received from `ping google.com`
