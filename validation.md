# Post-Install Vaildation
To validate that the SSL installation was successful. This validation method may be used whether the certificate was installed manually or automatically.

1. In cPanel, navigate to the `SSL/TLS` app.
![1 - native ssl app](https://user-images.githubusercontent.com/6568643/206798637-2f3cd00f-6cf3-43fe-8d62-3dbff4ba42b1.png)  
<br>

2. Click the link for maintaining certificates.
![2 - certificates](https://user-images.githubusercontent.com/6568643/206798638-484a311f-0815-4e03-91b3-b5970a6a3ffa.png)  
<br>

3. Locate your domain in the list of certificates. The expiration date should reflect that of the newly-installed certificate.
![3 - cert list](https://user-images.githubusercontent.com/6568643/206798640-760dc48b-8be2-4854-8182-8d0bece2c198.png)
🔵 If the certificate was installed via the Namecheap SSL app, you may further validate by locating the number in the `Description` column of the certificates table. Compare this number with the corresponding certificate in your [list of SSL certificates](https://ap.www.namecheap.com/ProductList/SslCertificates) in Namecheap.  
<br>
