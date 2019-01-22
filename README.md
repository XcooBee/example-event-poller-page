# XcooBee API Event Poller App

You can use the poller page to retrieve events and post them to your development instance.
This is useful when your development instance cannot receive HTTP webhook posts directly.

Please be aware that if you should exceed poll limits for the poller you will receive HTTP error 429.


## Encryption 

Event payloads may be encrypted with PGP Key based on sensitivity of payload. If you need plain text you will need to decrypt using OpengPGP tools before posting event data. If you are using PHP or JavaScript we recommend the use of XcooBee SDK for this purpose. 


## Usage

You supply your API access credentials and target Urls in the form fields and the poller page will poll in the interval specified. If events are found they will be download and reposted to internal website that will process them.

It can do one time manual poll or a scheduled poll in the background as long as the page is active.

