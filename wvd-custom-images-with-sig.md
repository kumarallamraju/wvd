**How to provision a WVD host pool with a custom image via Shared Image Galleries?**

***Usecase:***
I was working with a customer in which they built a master image for their WVD deployments. However the image was built in 
region-1 (eastus) but wanted to deploy the hostpools in different Azure regions. The recommended practice is to use
Shared Image Galleries to replicate the custom images to the target regions (e.g westus, centralus etc..)

As of today there is no option to provision a WVD host pool for the custom images available in Shared Image Galleries. 
Our WVD Azure PG worked on an ARM template that can be used to provision the host pool in which the custom image is available
via S.I.G.

You will find ARM template at [this github repo](
https://github.com/markhooks81/RDS-Templates/tree/master/wvd-templates/Create%20and%20provision%20WVD%20host%20pool)

You can directly deploy this ARM template in to your Azure subscription. I have pasted the screenshots below.

![screen1]('/files/file1.jpg')

![screen2]('/files/file2.jpg')

![screen3]('/files/file3.jpg')


As I understamd from our product management, we plan to support Shared Image Galleries in the Azure Portal in the Spring'20 time frame.
