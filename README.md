# Create a static website and host it on s3 bucket but with public read policy assigned, using cloudfront for CDN.

## My Solution

#### 1. Create an AWS account

#### 2. Search for s3 and choose "Create bucket" to create s3 bucket.
![alt text](images/a.png)

#### 3. Give bucket a unique name, leave every other settings as default and upload.
<!-- add image -->

#### 4. Upload objects (static website files) to the bucket created above
![alt text](images/c.png)

#### 5. Search for cloudfront
![alt text](images/d.png)

#### 6. Then create a distribution
![alt text](images/e.png)

#### 7. Setup the distribution as follows:

- Set the origin domain to the s3 bucket to be deployed
![alt text](images/f.png)

- The Origin access is set to Public by default but we'll be changing it to Origin access control settings (recommended)

- Then select the s3 bucket we intend to deloy
![alt text](images/g.png)

- Enable security protections
![alt text](images/h.png)

- Set default root object to the landing page and create distribution
![alt text](images/i.png)

#### 8. Copy the policy by clicking the "Copy policy" button
![alt text](images/k.png)

#### 9. Go to the permission of the s3 bucket
![alt text](images/l.png)

#### 10. Edit the bucket policy
![alt text](images/m.png)

#### 11. Paste the policy and click on "save changes"
![alt text](images/n.png)

#### 12. Go back to the cloudfront distribution and copy the domain name generated.
![alt text](images/j.png)

Static website hosted succesffully
![alt text](images/p.png)