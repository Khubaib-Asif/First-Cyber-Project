\# Lab setup (Quick)



This file documents how I created the DVWA lab used for testing.



1\. Install Oracle VM VirtualBox: https://www.virtualbox.org/  

2\. Download Metasploitable2 (or DVWA appliance). If you get a VMware package (.vmdk/.vmx), extract and attach the `.vmdk` as an existing disk in VirtualBox.  

3\. Create a new VM:

&nbsp;  - Type: Linux

&nbsp;  - Version: Ubuntu (32-bit) or Other Linux (32-bit)

&nbsp;  - Memory: 512 MB

&nbsp;  - Hard disk: use existing `.vmdk` (Metasploitable)

4\. Network: use \*\*Bridged Adapter\*\* (or Host-only if available) so the host can reach the VM.  

5\. Boot the VM and login: `msfadmin` / `msfadmin`.  

6\. From host browser open `http://<VM-IP>` (replace `<VM-IP>` with the VM address).  

7\. If DVWA shows setup: go to `/dvwa/setup.php` and click \*\*Create / Reset Database\*\*; then login (admin/password) and set security to \*\*low\*\*.





