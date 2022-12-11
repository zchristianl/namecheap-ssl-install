# Manual SSL Installation
For generating a CSR, issuing a certificate and installing it via the SSL module in cPanel. 

🟨 Note: This method is less convenient. Use the [Automatic SSL Installation](automatic.md) whenever possible.

1. In cPanel, open the `SSL/TLS` app.
![0 - native ssl app](https://user-images.githubusercontent.com/6568643/206796385-e6974fb7-15e1-444c-8bf0-c53669353620.png)    
<br>

2. Click on the link for Certificate Signing Requests.
![1 5 - CSR](https://user-images.githubusercontent.com/6568643/206796606-4afdd066-3f6b-44d1-b88c-f972377e9252.png)  
<br>

3. Complete the required information to generate a CSR.
![1 - generate csr](https://user-images.githubusercontent.com/6568643/206796387-fa40d5d6-1069-4d71-9423-12d6b0c9365a.png)  
🔵 Some certificates allow you to protect the `www` subdomain at no additional cost. Be sure to use the base domain as your primary domain, and the `www` subdomain as secondary.  
<br>

4. The CSR will be generated. 
![2 - generated](https://user-images.githubusercontent.com/6568643/206796390-fa9be33c-caea-4a22-aec8-3d57997e45dd.png)  
🟨 Make a note of the RSA private key. This is required for installation, and you will not be able to retrieve this later.  
<br>

5. Locate the SSL certificate in Namecheap and select `Activate` or `Renew`, whichever is applicable.
![2 5 - start activate](https://user-images.githubusercontent.com/6568643/206797208-161e7e53-187d-4682-a845-a27c753cff42.png)  
<br>

6. Paste the newly-generated CSR into the box. The primary domain should autopopulate.
![3 - start process](https://user-images.githubusercontent.com/6568643/206796391-438f5b0b-e610-4e83-bd41-bb686cb7a24b.png)  
<br>

7. Select a validation method of your choice. Refer to Namecheap's documentation for [Domain Control Validation](https://www.namecheap.com/support/knowledgebase/article.aspx/9637/68/how-can-i-complete-the-domain-control-validation-dcv-for-my-ssl-certificate/).
![4 - validation method](https://user-images.githubusercontent.com/6568643/206796392-57925b20-35e4-4c52-813c-92c95e62cf68.png)  
<br>

8. Review your selections for accuracy and click submit.
![5- review](https://user-images.githubusercontent.com/6568643/206796394-9f641890-324e-42c1-a391-04897a5ef684.png)  
<br>

9. Complete the Domain Control Validation for the certificate. Again, refer to Namecheap's documentation to validate the domain using the method of your choosing.
![6 - Validation](https://user-images.githubusercontent.com/6568643/206796395-205011ee-63f2-469d-ab0e-10fb4893d585.png)  
<br>

10.   One validation is successful, download the certificate.
![7 - success](https://user-images.githubusercontent.com/6568643/206797523-7ab465f4-72a2-49a9-981a-0b61ca632809.png)  
<br>

11.   The `.zip` file will contain a certificate and a CA bundle. Open these two files in your preferred text editor.
![8 - download](https://user-images.githubusercontent.com/6568643/206796398-f04822db-f57f-4be6-815c-20e94a9fceb0.png)  
<br>

12.   Return to the cPanel SSL/TLS app. Select the link for managing SSL sites.
![go to ssl](https://user-images.githubusercontent.com/6568643/206797720-9fb327cf-9522-4cee-9192-1f9224d5650a.png)  
<br>

13.    Locate the appropriate domain and select the `Update Certificate` link.
![9 - SSL Hosts](https://user-images.githubusercontent.com/6568643/206921831-8a5747be-50b7-4d68-a6f3-f958ff00ec5b.png)
<br>

14.    Paste the certificate, private key and CA bundle into their respective boxes and click `Install Certificate`.
![10 - paste in values](https://user-images.githubusercontent.com/6568643/206921285-e3429448-177d-4c6c-8cd2-1756f5f73070.png)  
<br>

15.   If installation was successful, a success message will appear.
![11 - success](https://user-images.githubusercontent.com/6568643/206921293-5b0b2d9b-c26a-49e1-894b-fef048691e9c.png)