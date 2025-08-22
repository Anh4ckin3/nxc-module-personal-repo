## Module - restrictedadmin.py 

A small module for SMB. This module is designed to perform three main actions on a registry key: "DisableRestrictedAdmin".

This key manages Windows "Restricted Admin" protection. If this protection is enabled, it is possible to perform Pass-The-Hash (PTH) on the RDP protocol, particularly with xfreerdp, as Windows uses the NTLM hash for authentication.

This idea comes from my tool [pyRestrictedAdmin](https://github.com/Anh4ckin3/pyRestrictedAdmin)

**modes:**

- read : See the value of the registry key and deduce if PTH is is possible or not
![Module preview](/images/picture2.png)

- disable : Set value to 1, PTH will be no longer possible
![Module preview](/images/picture4.png)

- enable : Set value to 0, that will enable the security option "RestricedAdmin" and allow PTH on RDP
![Module preview](/images/picture3.png)


