# Installation with EasyWP
For generating a CSR, private key and installing it to an EasyWP account.


1. On the Namecheap website, navigate to the `Apps` tab and select the `EasyWP` application.
![1 - easywp](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/a59ca4c7-cc1c-4333-9b6f-fd828f135d13)

<br>

2. Click the `Manage` button on the website for which you'd like to replace the certificate.
![2 - list of sites](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/f0da228b-a906-41aa-b662-8a617ac146fb)

<br>

3. Click the `Manage` button nex to the `SSL Certificate` row.
![3 - manage site](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/76dcb18d-1f39-472d-8190-42716748049c)

<br>

4. Select `Change` to replace the certificate.
![4 - change ssl](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/a5af7957-7b01-46be-8109-fe855ffaca9c)

<br>

1. You will need a CSR and private key to continue. You can use the [Namecheap CSR Generator](https://decoder.link/csr_generator) to generate this information.
![msedge_EGdeH2MyQN](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/89a21e59-15b2-4aa6-a2f6-993a002e20a7)

<br>

6. Add the `www` subdomain as an alternate name for good measure.<br>
![image](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/19786d0a-5726-4202-b635-2d1c0cddd1e1) 

<br>

7. Generate the CSR and private key.

<br>

🟨 Make a note of the RSA private key. This is required for installation, and you will not be able to retrieve this later.

<br>

8. 🛑 Do not use the self-signed certificate provided by this tool for installation. Follow steps 5-11 of the [Manual SSL Installation](manual.md) guide to properly issue the certificate. 

<br>

9. Copy and paste the Private Key, Certificate and CA Bundle. Click `Change` to install the certificate.
![5 add in cert](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/59bd6984-04c1-43d3-bf0d-a6fbc727b568)

<br>

10. Click the toggle switch to activate the certificate.
![6 - make active](https://github.com/zchristianl/namecheap-ssl-install/assets/6568643/d31c3b8e-ecc9-408a-b177-149c719fbea5)