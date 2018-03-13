### Import DO Order Proposal Headers:

This program imports DO Order Proposal Headers files into local server from Linux server 172.17.0.19 and stores data of sgh1 file into mdoheader table.

The program also downloads DO Order Proposal Lines and DO Order Proposal History from DO API to PF new Linux server 172.17.0.19 with .sgl1and .sgh2 extensions respectively.

The sgl1 and sgh2 files which are received from DMD are stored in "/work/edi/\[dbname\]/STARGATE.OUT/" in the new Linux server. The old sgh2 file is moved to subfolder "/old".

The sgl1 \(Order Proposal Line\) file contains JSON data with information about line number, supplier code, factory code, transport, quantity, available date and comment.

The sgh2 \(Order Proposal History\) file contains JSON data with information about past changes in the Order Proposal lines.

