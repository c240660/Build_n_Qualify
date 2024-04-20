# SAP build and qualify
# Build and Qualify code  for SAP-App/Netweaver and SAPHANA

# This is the updated code for SAP_B&Q for SAP App and SAPHANA Solutions servers

Please Note - Make sure, you have "ignore-messages.conf" and "mail" fileis under the "CWD/files" 

###### CWD is the Current working Directory where you have kept this BQ.V2.yml playbook ######


####### IMPORTANT ####### IMPORTANT ####### ####### IMPORTANT ####### IMPORTANT #######

if you are in need of running this playbook  for the second time on a single server for any reason, please exclude the task of updating the GRUB parameters	
you can executethe playbook excluding GRUB task as - 

# ansible-playbook build_n_qualify.yaml --skip-tags exclude_grub_update -i <inventory> 
 
####### IMPORTANT ####### IMPORTANT ####### ####### IMPORTANT ####### IMPORTANT #######

Have added the portion for skipping the grub update task if it is done already
