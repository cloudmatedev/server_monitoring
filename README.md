# Server Monitoring WHMCS Add-on
WHMCS Server Monitoring Add-on for monitoring client servers and opening a support ticket.

# Current Features
- Cron runs every X minutes and checks for successful ping then checks for defined ports.
- If a Ping or Port failure occurs, opens a ticket on behalf of the customer.
- Specify time in ms before considering a "failure" we set this to 750ms as some monitors can be slow.
- Set a minimum time between failures before opening a new ticket.

# Requirements
- PHP 7.2 (Might work on earlier versions not tested).
- WHMCS 7.5.0+ (Might work on earlier verions not tested).
- Checkiton.us Account API v1 (You need a token).

# The future
In the future we hope to see the following features implemented.

- Close the ticket with a reply if the server responds at the next cron run.
- Show failure logs on client/admin side.
- Display uptime information to customer (100% Uptime in June etc).
- Disable monitoring when Admin/Client specifies certain maintanence.
- Use own servers for monitoring (under considerations).
- Better handling of multiple failures whilst existing ticket open.







