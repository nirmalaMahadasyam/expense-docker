Create EC2 instance---docker,t3.micro,no key-pair,allow_everything. loginto @public ip
To execute perticular script file (docker installations cmd's): curl <raw url of expense-docker> |sudo bash
Resize the disk storage(logical volume allocation)--issue(if we build more images, then space issue are comming so we do these steps manually)
ref:conceptsa--->resizedisk.MD
to build the mysql,backend and frontend.
To push the images into ECR(Elastic container registry)
In ECR it self enable the image scan. their it will shows vulnarabilities dev should resolve the issues then it will move to forthere.
