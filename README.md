# test-repo
this is test



VPC - 10.0.0.0/16  
public subnet -> 10.0.0.0/24  
private subnet -> 10.0.1.0/24  

ohio route -> 10.0.0.0/16  
 virginia route -> 20.0.0.0/16  



Question 5 s3 bucket connection  
step 1 -> go to aws and search S3 and and then create S3 bucktet  
step 2 -> remove block all public access, allow versioning  
step 3- >now creating IAM user in aws  
step 4 -> create a user -> attach exiting policy -> srearch for Amazon S3 full   
step 5-> select Amazon S3 full access  
step -5 -> create user  
step 7 -> again click user and create access key -> CLI -> and save file  
step -> got s3 bucket -> permission -> object ownwership ->enable ACL -> in ACL enable everyone  read and write   
step 8 -> setup EC2 machine  
Installing Mountpoint - Amazon Simple Storage Service  
    1  yum install -y awscli  
    2  aws --version  
    3  rpmquery wget  
    4  wget https://s3.amazonaws.com/mountpoint-s3-release/latest/x86_64/mount-s3.rpm  
    5  yum install ./mount-s3.rpm  
    6  aws configure  
step 10 -> give id -> cpoied form file  
step 11 ->give passowrd -> coped form file  
step 12 -> default region name -> us-east-1  
step 13 -> default output -> enter  

    7  mkdir /data  
    8  mount-s3 s3-buk-2003 /data  
    9  df -h  
   10  cd /  
   11  ls  
   12  cd data  
   13  ls  
   14  history  
