# AnPassX
AnPassX is the mobile version of windows store app AnPass,  you can share data between AnPassX in phone and AnPass in Windows. This is devleoped by Xamarin. Because I don't have paid apple develop account, so only andriod version is deloyed. 


### How share data between devices
* currently support only Onedrive.
* Use the sync feature in the app.

###  Password security and local encryption
* The password set by the user will encrypt the local data after 512 bits of hash, and confusion characters will be added at the same time of hash, so there is no need to worry about being cracked.
* The local backup files are encrypted with the current password, and the password at the time of backup (if it is inconsistent with the current password) will be required during recovery.

### Cloud disk data encryption
* The synchronization data of the cloud disk is encrypted and stored on the network disk based on your network disk ID and hash confusion, so even if you forget the program password, as long as you can log in to the network disk, the data is recoverable.
* It is highly recommended to synchronize datat to your onedrive disk.
* The App can't get your confidential information. The login process use the API provided by Microsoft.

### Synchronization rule
* every item has an internal unique ID, which is used to distinguish different items.
* For the same item, keep the one with the most recent modification time.

### License
* synchronization will transmit the license info.
* Must sign in Onedrive to get the license info

