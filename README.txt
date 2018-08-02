Swivel PINsafe Add-on for Splunk

#Instalation
##Standalone envirioment
Install TA using the following instructions

##Distributed envirioment
Install TA in the Search heads
Install TA in the Indexers
Install TA in the For

#Configuring Splunk
##Using GUI
Create a new index to hold PINsafe data (optional)
Configure a new UDP input to received data from PINsafe
Select pinsafe as sourcetype
Select your destination index 

##Using configuration files
Copy inputs.conf from default to local
Uncomment the udp stanza
Change <ip_address> to the ip address of you PINsafe server
Change <port> to the port listening in Splunk
Change the index name to your destination index
Restart Splunk

#Configuring PINsafe
Please refer to product documentation.
https://kb.swivelsecure.com/w/index.php/Splunk

#Support
TA-pinsafe is community supported (http://answers.splunk.com)

#Feedback
Please send your feedback to feedback+pinsafe@devbusters.com
