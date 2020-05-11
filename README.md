# sol2
# ubuntu@u1:~$ set 
TF_VAR_AWS_ACCESS_KEY=AKIAS4UJ5OSA3Y4RA3QL 
TF_VAR_AWS_REGION=eu-west-1 
TF_VAR_AWS_SECRET_KEY=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

# ubuntu@u1:/mnt/hgfs/Desktop/sol3$ cp -r ../terraform-course/.terraform ./
# ubuntu@u1:/mnt/hgfs/Desktop/sol3$ ta
```
terraform destroy -auto-approve
terraform init
terraform apply -auto-approve
cat terraform.tfstate|grep public_ip|grep -v associate


Destroy complete! Resources: 0 destroyed.

Initializing the backend...

Initializing provider plugins...

The following providers do not have any version constraints in configuration,
so the latest version was installed.

To prevent automatic upgrades to new major versions that may contain breaking
changes, it is recommended to add version = "..." constraints to the
corresponding provider blocks in configuration, with the constraint strings
suggested below.

* provider.aws: version = "~> 2.60"

Terraform has been successfully initialized!

You may now begin working with Terraform. Try running "terraform plan" to see
any changes that are required for your infrastructure. All Terraform commands
should now work.

If you ever set or change modules or backend configuration for Terraform,
rerun this command to reinitialize your working directory. If you forget, other
commands will detect it and remind you to do so if necessary.
aws_key_pair.mykey: Creating...
aws_key_pair.mykey: Creation complete after 1s [id=mykey]
aws_instance.example[2]: Creating...
aws_instance.example[0]: Creating...
aws_instance.example[1]: Creating...
aws_instance.example[3]: Creating...
aws_instance.example[2]: Still creating... [10s elapsed]
aws_instance.example[0]: Still creating... [10s elapsed]
aws_instance.example[1]: Still creating... [10s elapsed]
aws_instance.example[3]: Still creating... [10s elapsed]
aws_instance.example[1]: Still creating... [20s elapsed]
aws_instance.example[3]: Still creating... [20s elapsed]
aws_instance.example[2]: Still creating... [20s elapsed]
aws_instance.example[0]: Still creating... [20s elapsed]
aws_instance.example[2]: Provisioning with 'file'...
aws_instance.example[3]: Provisioning with 'file'...
aws_instance.example[0]: Provisioning with 'file'...
aws_instance.example[1]: Provisioning with 'file'...
aws_instance.example[2]: Still creating... [30s elapsed]
aws_instance.example[1]: Still creating... [30s elapsed]
aws_instance.example[0]: Still creating... [30s elapsed]
aws_instance.example[3]: Still creating... [30s elapsed]
aws_instance.example[3]: Provisioning with 'remote-exec'...
aws_instance.example[3] (remote-exec): Connecting to remote host via SSH...
aws_instance.example[3] (remote-exec):   Host: 13.209.21.21
aws_instance.example[3] (remote-exec):   User: ubuntu
aws_instance.example[3] (remote-exec):   Password: false
aws_instance.example[3] (remote-exec):   Private key: true
aws_instance.example[3] (remote-exec):   Certificate: false
aws_instance.example[3] (remote-exec):   SSH Agent: false
aws_instance.example[3] (remote-exec):   Checking Host Key: false
aws_instance.example[3] (remote-exec): Connected!
aws_instance.example[1]: Provisioning with 'remote-exec'...
aws_instance.example[1] (remote-exec): Connecting to remote host via SSH...
aws_instance.example[1] (remote-exec):   Host: 3.34.90.51
aws_instance.example[1] (remote-exec):   User: ubuntu
aws_instance.example[1] (remote-exec):   Password: false
aws_instance.example[1] (remote-exec):   Private key: true
aws_instance.example[1] (remote-exec):   Certificate: false
aws_instance.example[1] (remote-exec):   SSH Agent: false
aws_instance.example[1] (remote-exec):   Checking Host Key: false
aws_instance.example[1] (remote-exec): Connected!
aws_instance.example[0]: Provisioning with 'remote-exec'...
aws_instance.example[0] (remote-exec): Connecting to remote host via SSH...
aws_instance.example[0] (remote-exec):   Host: 13.125.190.89
aws_instance.example[0] (remote-exec):   User: ubuntu
aws_instance.example[0] (remote-exec):   Password: false
aws_instance.example[0] (remote-exec):   Private key: true
aws_instance.example[0] (remote-exec):   Certificate: false
aws_instance.example[0] (remote-exec):   SSH Agent: false
aws_instance.example[0] (remote-exec):   Checking Host Key: false
aws_instance.example[0] (remote-exec): Connected!
aws_instance.example[1]: Still creating... [40s elapsed]
aws_instance.example[2]: Still creating... [40s elapsed]
aws_instance.example[0]: Still creating... [40s elapsed]
aws_instance.example[3]: Still creating... [40s elapsed]
aws_instance.example[3] (remote-exec): 0% [Working]
aws_instance.example[3] (remote-exec): Hit:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic InRelease
aws_instance.example[3] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[3] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
aws_instance.example[3] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB]
aws_instance.example[3] (remote-exec): 0% [3 InRelease 74.6 kB/74.6 kB 100%] [
aws_instance.example[3] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[3] (remote-exec): 0% [1 InRelease gpgv 242 kB] [Connectin
aws_instance.example[3] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[3] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[3] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe amd64 Packages [8570 kB]
aws_instance.example[3] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [4 Packag
aws_instance.example[3] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[3] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe Translation-en [4941 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [5 Translatio
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse amd64 Packages [151 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse Translation-en [108 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 Packages [932 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:9 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main Translation-en [318 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted amd64 Packages [50.1 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted Translation-en [12.6 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 Packages [1068 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe Translation-en [332 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse amd64 Packages [15.5 kB]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse Translation-en [6352 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[3] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main amd64 Packages [7516 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[3] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main Translation-en [4764 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[3] (remote-exec): Get:19 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe amd64 Packages [7484 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[3] (remote-exec): Get:20 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe Translation-en [4436 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B]
aws_instance.example[3] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[3] (remote-exec): 86% [4 Packages store 0 B]
aws_instance.example[3] (remote-exec): Get:21 http://security.ubuntu.com/ubuntu bionic-security/main amd64 Packages [707 kB]
aws_instance.example[3] (remote-exec): 86% [4 Packages store 0 B] [21 Packages
aws_instance.example[3] (remote-exec): 87% [21 Packages 71.0 kB/707 kB 10%]
aws_instance.example[3] (remote-exec): 87% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[3] (remote-exec): 88% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[3] (remote-exec): 89% [21 Packages 549 kB/707 kB 78%]
aws_instance.example[3] (remote-exec): 89% [6 Packages store 0 B] [21 Packages
aws_instance.example[3] (remote-exec): 89% [21 Packages 586 kB/707 kB 83%]
aws_instance.example[3] (remote-exec): 89% [7 Translation-en store 0 B] [21 Pa
aws_instance.example[3] (remote-exec): 90% [21 Packages 614 kB/707 kB 87%]
aws_instance.example[3] (remote-exec): 90% [8 Packages store 0 B] [21 Packages
aws_instance.example[3] (remote-exec): 90% [8 Packages store 0 B]
aws_instance.example[3] (remote-exec): 90% [Waiting for headers]
aws_instance.example[3] (remote-exec): 90% [10 Translation-en store 0 B] [Wait
aws_instance.example[3] (remote-exec): 91% [Waiting for headers]
aws_instance.example[3] (remote-exec): 91% [11 Packages store 0 B] [Waiting fo
aws_instance.example[3] (remote-exec): 91% [Waiting for headers]
aws_instance.example[3] (remote-exec): 91% [12 Translation-en store 0 B] [Wait
aws_instance.example[3] (remote-exec): 91% [Waiting for headers]
aws_instance.example[3] (remote-exec): 91% [13 Packages store 0 B] [Waiting fo
aws_instance.example[3] (remote-exec): Get:22 http://security.ubuntu.com/ubuntu bionic-security/main Translation-en [224 kB]
aws_instance.example[3] (remote-exec): 91% [13 Packages store 0 B] [22 Transla
aws_instance.example[3] (remote-exec): 92% [13 Packages store 0 B] [Waiting fo
aws_instance.example[3] (remote-exec): Get:23 http://security.ubuntu.com/ubuntu bionic-security/restricted amd64 Packages [40.3 kB]
aws_instance.example[3] (remote-exec): 92% [13 Packages store 0 B] [23 Package
aws_instance.example[3] (remote-exec): 92% [13 Packages store 0 B] [Waiting fo
aws_instance.example[3] (remote-exec): Get:24 http://security.ubuntu.com/ubuntu bionic-security/restricted Translation-en [10.2 kB]
aws_instance.example[3] (remote-exec): 92% [13 Packages store 0 B] [24 Transla
aws_instance.example[3] (remote-exec): Get:25 http://security.ubuntu.com/ubuntu bionic-security/universe amd64 Packages [660 kB]
aws_instance.example[3] (remote-exec): 92% [13 Packages store 0 B] [25 Package
aws_instance.example[3] (remote-exec): 95% [25 Packages 473 kB/660 kB 72%]
aws_instance.example[3] (remote-exec): 95% [14 Translation-en store 0 B] [25 P
aws_instance.example[3] (remote-exec): Get:26 http://security.ubuntu.com/ubuntu bionic-security/universe Translation-en [219 kB]
aws_instance.example[3] (remote-exec): 95% [14 Translation-en store 0 B] [26 T
aws_instance.example[3] (remote-exec): 96% [26 Translation-en 13.9 kB/219 kB 6
aws_instance.example[3] (remote-exec): 96% [15 Packages store 0 B] [26 Transla
aws_instance.example[3] (remote-exec): 96% [26 Translation-en 31.3 kB/219 kB 1
aws_instance.example[3] (remote-exec): 96% [16 Translation-en store 0 B] [26 T
aws_instance.example[3] (remote-exec): 96% [26 Translation-en 40.0 kB/219 kB 1
aws_instance.example[3] (remote-exec): 96% [17 Packages store 0 B] [26 Transla
aws_instance.example[3] (remote-exec): 97% [26 Translation-en 50.1 kB/219 kB 2
aws_instance.example[3] (remote-exec): 97% [18 Translation-en store 0 B] [26 T
aws_instance.example[3] (remote-exec): 97% [26 Translation-en 53.0 kB/219 kB 2
aws_instance.example[3] (remote-exec): 97% [19 Packages store 0 B] [26 Transla
aws_instance.example[3] (remote-exec): 97% [26 Translation-en 64.6 kB/219 kB 2
aws_instance.example[3] (remote-exec): 97% [20 Translation-en store 0 B] [26 T
aws_instance.example[3] (remote-exec): 97% [26 Translation-en 67.5 kB/219 kB 3
aws_instance.example[3] (remote-exec): 97% [21 Packages store 0 B] [26 Transla
aws_instance.example[3] (remote-exec): Get:27 http://security.ubuntu.com/ubuntu bionic-security/multiverse amd64 Packages [7392 B]
aws_instance.example[3] (remote-exec): 98% [21 Packages store 0 B] [27 Package
aws_instance.example[3] (remote-exec): 98% [21 Packages store 0 B] [Waiting fo
aws_instance.example[3] (remote-exec): Get:28 http://security.ubuntu.com/ubuntu bionic-security/multiverse Translation-en [2788 B]
aws_instance.example[3] (remote-exec): 98% [21 Packages store 0 B] [28 Transla
aws_instance.example[3] (remote-exec): 98% [21 Packages store 0 B]
aws_instance.example[3] (remote-exec): 98% [Working]
aws_instance.example[3] (remote-exec): 98% [22 Translation-en store 0 B]
aws_instance.example[3] (remote-exec): 99% [Working]
aws_instance.example[3] (remote-exec): 99% [23 Packages store 0 B]
aws_instance.example[3] (remote-exec): 99% [Working]
aws_instance.example[3] (remote-exec): 99% [24 Translation-en store 0 B]
aws_instance.example[3] (remote-exec): 99% [Working]
aws_instance.example[3] (remote-exec): 99% [25 Packages store 0 B]
aws_instance.example[3] (remote-exec): 99% [Working]
aws_instance.example[3] (remote-exec): 99% [26 Translation-en store 0 B]
aws_instance.example[3] (remote-exec): 100% [Working]
aws_instance.example[3] (remote-exec): 100% [27 Packages store 0 B]
aws_instance.example[3] (remote-exec): 100% [Working]
aws_instance.example[3] (remote-exec): 100% [28 Translation-en store 0 B]
aws_instance.example[3] (remote-exec): 100% [Working]
aws_instance.example[3] (remote-exec): Fetched 18.7 MB in 4s (4889 kB/s)
aws_instance.example[1] (remote-exec): 0% [Working]
aws_instance.example[1] (remote-exec): Hit:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic InRelease
aws_instance.example[1] (remote-exec): 0% [Connecting to security.ubuntu.com]
aws_instance.example[1] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
aws_instance.example[1] (remote-exec): 0% [Waiting for headers] [Connecting to
aws_instance.example[1] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB]
aws_instance.example[1] (remote-exec): 0% [Connecting to security.ubuntu.com]
aws_instance.example[1] (remote-exec): 0% [1 InRelease gpgv 242 kB] [Connectin
aws_instance.example[1] (remote-exec): 0% [Connecting to security.ubuntu.com]
aws_instance.example[1] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[1] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe amd64 Packages [8570 kB]
aws_instance.example[1] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [4 Packag
aws_instance.example[1] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Connecti
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[1] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe Translation-en [4941 kB]
aws_instance.example[0]: Still creating... [50s elapsed]
aws_instance.example[1]: Still creating... [50s elapsed]
aws_instance.example[2]: Still creating... [50s elapsed]
aws_instance.example[3]: Still creating... [50s elapsed]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [5 Translatio
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse amd64 Packages [151 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse Translation-en [108 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 Packages [932 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main Translation-en [318 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted amd64 Packages [50.1 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted Translation-en [12.6 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 Packages [1068 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe Translation-en [332 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse amd64 Packages [15.5 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse Translation-en [6352 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): Get:16 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [16 InRelease
aws_instance.example[1] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main amd64 Packages [7516 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [16 InRelease
aws_instance.example[1] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main Translation-en [4764 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[1] (remote-exec): Get:19 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe amd64 Packages [7484 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [19 Packages
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[1] (remote-exec): Get:20 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe Translation-en [4436 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [16 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [16 InRelease
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B]
aws_instance.example[1] (remote-exec): 0% [4 Packages store 0 B] [16 InRelease
aws_instance.example[1] (remote-exec): 86% [4 Packages store 0 B]
aws_instance.example[1] (remote-exec): Get:21 http://security.ubuntu.com/ubuntu bionic-security/main amd64 Packages [707 kB]
aws_instance.example[1] (remote-exec): 86% [4 Packages store 0 B] [21 Packages
aws_instance.example[1] (remote-exec): 87% [21 Packages 56.3 kB/707 kB 8%]
aws_instance.example[1] (remote-exec): 87% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[1] (remote-exec): 87% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[3] (remote-exec): Reading package lists... 0%
aws_instance.example[3] (remote-exec): Reading package lists... 0%
aws_instance.example[3] (remote-exec): Reading package lists... 0%
aws_instance.example[3] (remote-exec): Reading package lists... 4%
aws_instance.example[3] (remote-exec): Reading package lists... 4%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): 88% [21 Packages 346 kB/707 kB 49%]
aws_instance.example[1] (remote-exec): 88% [6 Packages store 0 B] [21 Packages
aws_instance.example[1] (remote-exec): 89% [21 Packages 370 kB/707 kB 52%]
aws_instance.example[1] (remote-exec): 89% [7 Translation-en store 0 B] [21 Pa
aws_instance.example[1] (remote-exec): 89% [21 Packages 388 kB/707 kB 55%]
aws_instance.example[1] (remote-exec): 89% [8 Packages store 0 B] [21 Packages
aws_instance.example[1] (remote-exec): 90% [21 Packages 653 kB/707 kB 92%]
aws_instance.example[1] (remote-exec): 90% [9 Translation-en store 0 B] [21 Pa
aws_instance.example[1] (remote-exec): 90% [9 Translation-en store 0 B]
aws_instance.example[1] (remote-exec): 91% [Waiting for headers]
aws_instance.example[1] (remote-exec): 91% [10 Packages store 0 B] [Waiting fo
aws_instance.example[1] (remote-exec): 91% [Waiting for headers]
aws_instance.example[1] (remote-exec): 91% [11 Translation-en store 0 B] [Wait
aws_instance.example[1] (remote-exec): 91% [Waiting for headers]
aws_instance.example[1] (remote-exec): 91% [12 Packages store 0 B] [Waiting fo
aws_instance.example[1] (remote-exec): Get:22 http://security.ubuntu.com/ubuntu bionic-security/main Translation-en [224 kB]
aws_instance.example[1] (remote-exec): 91% [12 Packages store 0 B] [22 Transla
aws_instance.example[1] (remote-exec): 92% [22 Translation-en 194 kB/224 kB 86
aws_instance.example[1] (remote-exec): 92% [13 Translation-en store 0 B] [22 T
aws_instance.example[1] (remote-exec): 92% [13 Translation-en store 0 B] [Wait
aws_instance.example[1] (remote-exec): Get:23 http://security.ubuntu.com/ubuntu bionic-security/restricted amd64 Packages [40.3 kB]
aws_instance.example[1] (remote-exec): 92% [13 Translation-en store 0 B] [23 P
aws_instance.example[1] (remote-exec): Get:24 http://security.ubuntu.com/ubuntu bionic-security/restricted Translation-en [10.2 kB]
aws_instance.example[1] (remote-exec): 93% [13 Translation-en store 0 B] [24 T
aws_instance.example[1] (remote-exec): Get:25 http://security.ubuntu.com/ubuntu bionic-security/universe amd64 Packages [660 kB]
aws_instance.example[1] (remote-exec): 93% [13 Translation-en store 0 B] [25 P
aws_instance.example[1] (remote-exec): 94% [25 Packages 286 kB/660 kB 43%]
aws_instance.example[1] (remote-exec): 94% [14 Packages store 0 B] [25 Package
aws_instance.example[1] (remote-exec): 94% [25 Packages 304 kB/660 kB 46%]
aws_instance.example[1] (remote-exec): 94% [15 Translation-en store 0 B] [25 P
aws_instance.example[1] (remote-exec): 95% [25 Packages 312 kB/660 kB 47%]
aws_instance.example[1] (remote-exec): 95% [17 Packages store 0 B] [25 Package
aws_instance.example[1] (remote-exec): 95% [25 Packages 323 kB/660 kB 49%]
aws_instance.example[1] (remote-exec): 95% [18 Translation-en store 0 B] [25 P
aws_instance.example[1] (remote-exec): 95% [25 Packages 328 kB/660 kB 50%]
aws_instance.example[1] (remote-exec): 95% [19 Packages store 0 B] [25 Package
aws_instance.example[1] (remote-exec): 95% [25 Packages 337 kB/660 kB 51%]
aws_instance.example[1] (remote-exec): 95% [20 Translation-en store 0 B] [25 P
aws_instance.example[1] (remote-exec): 96% [25 Packages 343 kB/660 kB 52%]
aws_instance.example[1] (remote-exec): 96% [21 Packages store 0 B] [25 Package
aws_instance.example[1] (remote-exec): 97% [25 Packages 660 kB/660 kB 100%]
aws_instance.example[1] (remote-exec): Get:26 http://security.ubuntu.com/ubuntu bionic-security/universe Translation-en [219 kB]
aws_instance.example[3] (remote-exec): Reading package lists... 46%
aws_instance.example[3] (remote-exec): Reading package lists... 46%
aws_instance.example[3] (remote-exec): Reading package lists... 66%
aws_instance.example[3] (remote-exec): Reading package lists... 66%
aws_instance.example[3] (remote-exec): Reading package lists... 67%
aws_instance.example[3] (remote-exec): Reading package lists... 67%
aws_instance.example[3] (remote-exec): Reading package lists... 67%
aws_instance.example[3] (remote-exec): Reading package lists... 67%
aws_instance.example[3] (remote-exec): Reading package lists... 70%
aws_instance.example[3] (remote-exec): Reading package lists... 73%
aws_instance.example[3] (remote-exec): Reading package lists... 73%
aws_instance.example[3] (remote-exec): Reading package lists... 76%
aws_instance.example[3] (remote-exec): Reading package lists... 76%
aws_instance.example[3] (remote-exec): Reading package lists... 77%
aws_instance.example[3] (remote-exec): Reading package lists... 77%
aws_instance.example[3] (remote-exec): Reading package lists... 77%
aws_instance.example[3] (remote-exec): Reading package lists... 77%
aws_instance.example[3] (remote-exec): Reading package lists... 83%
aws_instance.example[3] (remote-exec): Reading package lists... 83%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 86%
aws_instance.example[3] (remote-exec): Reading package lists... 90%
aws_instance.example[3] (remote-exec): Reading package lists... 90%
aws_instance.example[3] (remote-exec): Reading package lists... 93%
aws_instance.example[3] (remote-exec): Reading package lists... 93%
aws_instance.example[3] (remote-exec): Reading package lists... 93%
aws_instance.example[3] (remote-exec): Reading package lists... 93%
aws_instance.example[3] (remote-exec): Reading package lists... 94%
aws_instance.example[3] (remote-exec): Reading package lists... 94%
aws_instance.example[3] (remote-exec): Reading package lists... 97%
aws_instance.example[3] (remote-exec): Reading package lists... 97%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... 99%
aws_instance.example[3] (remote-exec): Reading package lists... Done
aws_instance.example[1] (remote-exec): 97% [26 Translation-en 5243 B/219 kB 2%
aws_instance.example[1] (remote-exec): 97% [22 Translation-en store 0 B] [26 T
aws_instance.example[1] (remote-exec): Get:27 http://security.ubuntu.com/ubuntu bionic-security/multiverse amd64 Packages [7392 B]
aws_instance.example[1] (remote-exec): 98% [22 Translation-en store 0 B] [27 P
aws_instance.example[1] (remote-exec): 98% [22 Translation-en store 0 B] [Wait
aws_instance.example[1] (remote-exec): Get:28 http://security.ubuntu.com/ubuntu bionic-security/multiverse Translation-en [2788 B]
aws_instance.example[3] (remote-exec): Reading package lists... 0%
aws_instance.example[3] (remote-exec): Reading package lists... 100%
aws_instance.example[3] (remote-exec): Reading package lists... Done
aws_instance.example[1] (remote-exec): 98% [22 Translation-en store 0 B] [28 T
aws_instance.example[1] (remote-exec): 98% [22 Translation-en store 0 B]
aws_instance.example[1] (remote-exec): 99% [Working]
aws_instance.example[1] (remote-exec): 99% [23 Packages store 0 B]
aws_instance.example[1] (remote-exec): 99% [Working]
aws_instance.example[1] (remote-exec): 99% [24 Translation-en store 0 B]
aws_instance.example[1] (remote-exec): 99% [Working]
aws_instance.example[1] (remote-exec): 99% [25 Packages store 0 B]
aws_instance.example[3] (remote-exec): Building dependency tree... 0%
aws_instance.example[3] (remote-exec): Building dependency tree... 0%
aws_instance.example[3] (remote-exec): Building dependency tree... 50%
aws_instance.example[3] (remote-exec): Building dependency tree... 50%
aws_instance.example[1] (remote-exec): 99% [Working]
aws_instance.example[1] (remote-exec): 99% [26 Translation-en store 0 B]
aws_instance.example[1] (remote-exec): 100% [Working]
aws_instance.example[1] (remote-exec): 100% [27 Packages store 0 B]
aws_instance.example[1] (remote-exec): 100% [Working]
aws_instance.example[1] (remote-exec): 100% [28 Translation-en store 0 B]
aws_instance.example[1] (remote-exec): 100% [Working]
aws_instance.example[1] (remote-exec): Fetched 18.7 MB in 4s (4857 kB/s)
aws_instance.example[3] (remote-exec): Building dependency tree
aws_instance.example[3] (remote-exec): Reading state information... 0%
aws_instance.example[3] (remote-exec): Reading state information... 0%
aws_instance.example[3] (remote-exec): Reading state information... Done
aws_instance.example[3] (remote-exec): The following additional packages will be installed:
aws_instance.example[3] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[3] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[3] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[3] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[3] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[3] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[3] (remote-exec):   libnginx-mod-mail
aws_instance.example[3] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[3] (remote-exec):   libwebp6 libxpm4 nginx-common
aws_instance.example[3] (remote-exec):   nginx-core
aws_instance.example[3] (remote-exec): Suggested packages:
aws_instance.example[3] (remote-exec):   libgd-tools fcgiwrap nginx-doc
aws_instance.example[3] (remote-exec):   ssl-cert
aws_instance.example[3] (remote-exec): The following NEW packages will be installed:
aws_instance.example[3] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[3] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[3] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[3] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[3] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[3] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[3] (remote-exec):   libnginx-mod-mail
aws_instance.example[3] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[3] (remote-exec):   libwebp6 libxpm4 nginx nginx-common
aws_instance.example[3] (remote-exec):   nginx-core
aws_instance.example[3] (remote-exec): 0 upgraded, 18 newly installed, 0 to remove and 20 not upgraded.
aws_instance.example[3] (remote-exec): Need to get 2462 kB of archives.
aws_instance.example[3] (remote-exec): After this operation, 8210 kB of additional disk space will be used.
aws_instance.example[3] (remote-exec): 0% [Working]
aws_instance.example[3] (remote-exec): Get:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libjpeg-turbo8 amd64 1.5.2-0ubuntu5.18.04.3 [110 kB]
aws_instance.example[3] (remote-exec): 0% [1 libjpeg-turbo8 0 B/110 kB 0%]
aws_instance.example[3] (remote-exec): 5% [Working]
aws_instance.example[3] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fonts-dejavu-core all 2.37-1 [1041 kB]
aws_instance.example[3] (remote-exec): 5% [2 fonts-dejavu-core 0 B/1041 kB 0%]
aws_instance.example[3] (remote-exec): 40% [Working]
aws_instance.example[3] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fontconfig-config all 2.12.6-0ubuntu2 [55.8 kB]
aws_instance.example[3] (remote-exec): 40% [3 fontconfig-config 0 B/55.8 kB 0%
aws_instance.example[3] (remote-exec): 43% [Working]
aws_instance.example[3] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libfontconfig1 amd64 2.12.6-0ubuntu2 [137 kB]
aws_instance.example[3] (remote-exec): 43% [4 libfontconfig1 0 B/137 kB 0%]
aws_instance.example[3] (remote-exec): 48% [Working]
aws_instance.example[3] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjpeg8 amd64 8c-2ubuntu8 [2194 B]
aws_instance.example[3] (remote-exec): 48% [5 libjpeg8 0 B/2194 B 0%]
aws_instance.example[3] (remote-exec): 49% [Working]
aws_instance.example[3] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjbig0 amd64 2.1-3.1build1 [26.7 kB]
aws_instance.example[3] (remote-exec): 49% [6 libjbig0 0 B/26.7 kB 0%]
aws_instance.example[3] (remote-exec): 51% [Working]
aws_instance.example[3] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libtiff5 amd64 4.0.9-5ubuntu0.3 [153 kB]
aws_instance.example[3] (remote-exec): 51% [7 libtiff5 0 B/153 kB 0%]
aws_instance.example[3] (remote-exec): 57% [Working]
aws_instance.example[3] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libwebp6 amd64 0.6.1-2 [185 kB]
aws_instance.example[3] (remote-exec): 57% [8 libwebp6 0 B/185 kB 0%]
aws_instance.example[3] (remote-exec): 64% [Working]
aws_instance.example[3] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libxpm4 amd64 1:3.5.12-1 [34.0 kB]
aws_instance.example[3] (remote-exec): 64% [9 libxpm4 0 B/34.0 kB 0%]
aws_instance.example[3] (remote-exec): 67% [Working]
aws_instance.example[3] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libgd3 amd64 2.2.5-4ubuntu0.4 [119 kB]
aws_instance.example[3] (remote-exec): 67% [10 libgd3 0 B/119 kB 0%]
aws_instance.example[3] (remote-exec): 72% [Working]
aws_instance.example[3] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-common all 1.14.0-0ubuntu1.7 [37.4 kB]
aws_instance.example[3] (remote-exec): 72% [11 nginx-common 0 B/37.4 kB 0%]
aws_instance.example[3] (remote-exec): 74% [Working]
aws_instance.example[3] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-geoip amd64 1.14.0-0ubuntu1.7 [11.2 kB]
aws_instance.example[3] (remote-exec): 74% [12 libnginx-mod-http-geoip 0 B/11.
aws_instance.example[3] (remote-exec): 75% [Working]
aws_instance.example[3] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-image-filter amd64 1.14.0-0ubuntu1.7 [14.6 kB]
aws_instance.example[3] (remote-exec): 75% [13 libnginx-mod-http-image-filter
aws_instance.example[3] (remote-exec): 77% [Working]
aws_instance.example[3] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.14.0-0ubuntu1.7 [13.0 kB]
aws_instance.example[3] (remote-exec): 77% [14 libnginx-mod-http-xslt-filter 0
aws_instance.example[3] (remote-exec): 79% [Working]
aws_instance.example[3] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-mail amd64 1.14.0-0ubuntu1.7 [41.8 kB]
aws_instance.example[0] (remote-exec): 0% [Working]
aws_instance.example[0] (remote-exec): Hit:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic InRelease
aws_instance.example[0] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[0] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
aws_instance.example[3] (remote-exec): 79% [15 libnginx-mod-mail 0 B/41.8 kB 0
aws_instance.example[3] (remote-exec): 81% [Working]
aws_instance.example[3] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-stream amd64 1.14.0-0ubuntu1.7 [63.7 kB]
aws_instance.example[0] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB]
aws_instance.example[3] (remote-exec): 81% [16 libnginx-mod-stream 0 B/63.7 kB
aws_instance.example[3] (remote-exec): 84% [Working]
aws_instance.example[3] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-core amd64 1.14.0-0ubuntu1.7 [413 kB]
aws_instance.example[3] (remote-exec): 84% [17 nginx-core 0 B/413 kB 0%]
aws_instance.example[3] (remote-exec): 99% [Working]
aws_instance.example[3] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx all 1.14.0-0ubuntu1.7 [3596 B]
aws_instance.example[3] (remote-exec): 99% [18 nginx 0 B/3596 B 0%]
aws_instance.example[3] (remote-exec): 100% [Working]
aws_instance.example[3] (remote-exec): Fetched 2462 kB in 0s (29.8 MB/s)
aws_instance.example[0] (remote-exec): 0% [3 InRelease 74.6 kB/74.6 kB 100%] [
aws_instance.example[0] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[0] (remote-exec): 0% [1 InRelease gpgv 242 kB] [Connectin
aws_instance.example[0] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[0] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[0] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe amd64 Packages [8570 kB]
aws_instance.example[0] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [4 Packag
aws_instance.example[0] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[0] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe Translation-en [4941 kB]
aws_instance.example[3] (remote-exec): Preconfiguring packages ...
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [5 Translatio
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:6 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse amd64 Packages [151 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse Translation-en [108 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 Packages [932 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main Translation-en [318 kB]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libjpeg-turbo8:amd64.
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted amd64 Packages [50.1 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted Translation-en [12.6 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 Packages [1068 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe Translation-en [332 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse amd64 Packages [15.5 kB]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse Translation-en [6352 B]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [6 InRelease
aws_instance.example[0] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main amd64 Packages [7516 B]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [6 InRelease
aws_instance.example[0] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main Translation-en [4764 B]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[0] (remote-exec): Get:19 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe amd64 Packages [7484 B]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [19 Packages
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[0] (remote-exec): Get:20 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe Translation-en [4436 B]
aws_instance.example[3] (remote-exec): (Reading database ...
aws_instance.example[3] (remote-exec): (Reading database ... 5%
aws_instance.example[3] (remote-exec): (Reading database ... 10%
aws_instance.example[3] (remote-exec): (Reading database ... 15%
aws_instance.example[3] (remote-exec): (Reading database ... 20%
aws_instance.example[3] (remote-exec): (Reading database ... 25%
aws_instance.example[3] (remote-exec): (Reading database ... 30%
aws_instance.example[3] (remote-exec): (Reading database ... 35%
aws_instance.example[3] (remote-exec): (Reading database ... 40%
aws_instance.example[3] (remote-exec): (Reading database ... 45%
aws_instance.example[3] (remote-exec): (Reading database ... 50%
aws_instance.example[3] (remote-exec): (Reading database ... 55%
aws_instance.example[3] (remote-exec): (Reading database ... 60%
aws_instance.example[3] (remote-exec): (Reading database ... 65%
aws_instance.example[3] (remote-exec): (Reading database ... 70%
aws_instance.example[3] (remote-exec): (Reading database ... 75%
aws_instance.example[3] (remote-exec): (Reading database ... 80%
aws_instance.example[3] (remote-exec): (Reading database ... 85%
aws_instance.example[3] (remote-exec): (Reading database ... 90%
aws_instance.example[3] (remote-exec): (Reading database ... 95%
aws_instance.example[3] (remote-exec): (Reading database ... 100%
aws_instance.example[3] (remote-exec): (Reading database ... 56588 files and directories currently installed.)
aws_instance.example[3] (remote-exec): Preparing to unpack .../00-libjpeg-turbo8_1.5.2-0ubuntu5.18.04.3_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [20 Translati
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [6 InRelease
aws_instance.example[3] (remote-exec): Selecting previously unselected package fonts-dejavu-core.
aws_instance.example[3] (remote-exec): Preparing to unpack .../01-fonts-dejavu-core_2.37-1_all.deb ...
aws_instance.example[3] (remote-exec): Unpacking fonts-dejavu-core (2.37-1) ...
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B]
aws_instance.example[0] (remote-exec): 0% [4 Packages store 0 B] [6 InRelease
aws_instance.example[3] (remote-exec): Selecting previously unselected package fontconfig-config.
aws_instance.example[3] (remote-exec): Preparing to unpack .../02-fontconfig-config_2.12.6-0ubuntu2_all.deb ...
aws_instance.example[3] (remote-exec): Unpacking fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package libfontconfig1:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../03-libfontconfig1_2.12.6-0ubuntu2_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): 86% [4 Packages store 0 B]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libjpeg8:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../04-libjpeg8_8c-2ubuntu8_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[0] (remote-exec): Get:21 http://security.ubuntu.com/ubuntu bionic-security/main amd64 Packages [707 kB]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libjbig0:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../05-libjbig0_2.1-3.1build1_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[0] (remote-exec): 86% [4 Packages store 0 B] [21 Packages
aws_instance.example[3] (remote-exec): Selecting previously unselected package libtiff5:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../06-libtiff5_4.0.9-5ubuntu0.3_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package libwebp6:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../07-libwebp6_0.6.1-2_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package libxpm4:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../08-libxpm4_1%3a3.5.12-1_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package libgd3:amd64.
aws_instance.example[3] (remote-exec): Preparing to unpack .../09-libgd3_2.2.5-4ubuntu0.4_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[0] (remote-exec): 87% [4 Packages store 0 B] [21 Packages
aws_instance.example[1] (remote-exec): Reading package lists... 0%
aws_instance.example[1] (remote-exec): Reading package lists... 0%
aws_instance.example[1] (remote-exec): Reading package lists... 0%
aws_instance.example[1] (remote-exec): Reading package lists... 4%
aws_instance.example[1] (remote-exec): Reading package lists... 4%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Reading package lists... 7%
aws_instance.example[3] (remote-exec): Selecting previously unselected package nginx-common.
aws_instance.example[3] (remote-exec): Preparing to unpack .../10-nginx-common_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[3] (remote-exec): Unpacking nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package libnginx-mod-http-geoip.
aws_instance.example[3] (remote-exec): Preparing to unpack .../11-libnginx-mod-http-geoip_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): 89% [21 Packages 607 kB/707 kB 86%]
aws_instance.example[0] (remote-exec): 89% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[0] (remote-exec): 90% [5 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): Get:22 http://security.ubuntu.com/ubuntu bionic-security/main Translation-en [224 kB]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libnginx-mod-http-image-filter.
aws_instance.example[3] (remote-exec): Preparing to unpack .../12-libnginx-mod-http-image-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): 90% [5 Translation-en store 0 B] [22 Tr
aws_instance.example[0] (remote-exec): 90% [5 Translation-en store 0 B] [Waiti
aws_instance.example[0] (remote-exec): Get:23 http://security.ubuntu.com/ubuntu bionic-security/restricted amd64 Packages [40.3 kB]
aws_instance.example[0] (remote-exec): 91% [5 Translation-en store 0 B] [23 Pa
aws_instance.example[0] (remote-exec): 91% [5 Translation-en store 0 B] [Waiti
aws_instance.example[0] (remote-exec): Get:24 http://security.ubuntu.com/ubuntu bionic-security/restricted Translation-en [10.2 kB]
aws_instance.example[0] (remote-exec): 91% [5 Translation-en store 0 B] [24 Tr
aws_instance.example[0] (remote-exec): Get:25 http://security.ubuntu.com/ubuntu bionic-security/universe amd64 Packages [660 kB]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libnginx-mod-http-xslt-filter.
aws_instance.example[3] (remote-exec): Preparing to unpack .../13-libnginx-mod-http-xslt-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): 91% [5 Translation-en store 0 B] [25 Pa
aws_instance.example[0] (remote-exec): Get:26 http://security.ubuntu.com/ubuntu bionic-security/universe Translation-en [219 kB]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libnginx-mod-mail.
aws_instance.example[0] (remote-exec): 94% [5 Translation-en store 0 B] [26 Tr
aws_instance.example[0] (remote-exec): Get:27 http://security.ubuntu.com/ubuntu bionic-security/multiverse amd64 Packages [7392 B]
aws_instance.example[0] (remote-exec): 94% [5 Translation-en store 0 B] [27 Pa
aws_instance.example[0] (remote-exec): Get:28 http://security.ubuntu.com/ubuntu bionic-security/multiverse Translation-en [2788 B]
aws_instance.example[3] (remote-exec): Preparing to unpack .../14-libnginx-mod-mail_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): 95% [5 Translation-en store 0 B] [28 Tr
aws_instance.example[0] (remote-exec): 95% [5 Translation-en store 0 B]
aws_instance.example[3] (remote-exec): Selecting previously unselected package libnginx-mod-stream.
aws_instance.example[3] (remote-exec): Preparing to unpack .../15-libnginx-mod-stream_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Selecting previously unselected package nginx-core.
aws_instance.example[3] (remote-exec): Preparing to unpack .../16-nginx-core_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[3] (remote-exec): Unpacking nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Reading package lists... 46%
aws_instance.example[1] (remote-exec): Reading package lists... 46%
aws_instance.example[1] (remote-exec): Reading package lists... 66%
aws_instance.example[1] (remote-exec): Reading package lists... 66%
aws_instance.example[1] (remote-exec): Reading package lists... 67%
aws_instance.example[1] (remote-exec): Reading package lists... 67%
aws_instance.example[1] (remote-exec): Reading package lists... 67%
aws_instance.example[1] (remote-exec): Reading package lists... 67%
aws_instance.example[1] (remote-exec): Reading package lists... 71%
aws_instance.example[1] (remote-exec): Reading package lists... 73%
aws_instance.example[1] (remote-exec): Reading package lists... 73%
aws_instance.example[1] (remote-exec): Reading package lists... 76%
aws_instance.example[1] (remote-exec): Reading package lists... 76%
aws_instance.example[1] (remote-exec): Reading package lists... 77%
aws_instance.example[1] (remote-exec): Reading package lists... 77%
aws_instance.example[1] (remote-exec): Reading package lists... 77%
aws_instance.example[1] (remote-exec): Reading package lists... 77%
aws_instance.example[1] (remote-exec): Reading package lists... 83%
aws_instance.example[1] (remote-exec): Reading package lists... 83%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 86%
aws_instance.example[1] (remote-exec): Reading package lists... 90%
aws_instance.example[1] (remote-exec): Reading package lists... 90%
aws_instance.example[1] (remote-exec): Reading package lists... 93%
aws_instance.example[1] (remote-exec): Reading package lists... 93%
aws_instance.example[1] (remote-exec): Reading package lists... 93%
aws_instance.example[1] (remote-exec): Reading package lists... 93%
aws_instance.example[1] (remote-exec): Reading package lists... 94%
aws_instance.example[1] (remote-exec): Reading package lists... 94%
aws_instance.example[1] (remote-exec): Reading package lists... 97%
aws_instance.example[1] (remote-exec): Reading package lists... 97%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... 99%
aws_instance.example[1] (remote-exec): Reading package lists... Done
aws_instance.example[3] (remote-exec): Selecting previously unselected package nginx.
aws_instance.example[3] (remote-exec): Preparing to unpack .../17-nginx_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[3] (remote-exec): Unpacking nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Reading package lists... 0%
aws_instance.example[1] (remote-exec): Reading package lists... 100%
aws_instance.example[1] (remote-exec): Reading package lists... Done
aws_instance.example[3] (remote-exec): Setting up libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[0] (remote-exec): 95% [Working]
aws_instance.example[0] (remote-exec): 95% [7 Packages store 0 B]
aws_instance.example[0] (remote-exec): 95% [Working]
aws_instance.example[0] (remote-exec): 95% [8 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 95% [Working]
aws_instance.example[0] (remote-exec): 95% [9 Packages store 0 B]
aws_instance.example[3] (remote-exec): Setting up fonts-dejavu-core (2.37-1) ...
aws_instance.example[1] (remote-exec): Building dependency tree... 0%
aws_instance.example[1] (remote-exec): Building dependency tree... 0%
aws_instance.example[1] (remote-exec): Building dependency tree... 50%
aws_instance.example[1] (remote-exec): Building dependency tree... 50%
aws_instance.example[1] (remote-exec): Building dependency tree
aws_instance.example[1] (remote-exec): Reading state information... 0%
aws_instance.example[1] (remote-exec): Reading state information... 0%
aws_instance.example[1] (remote-exec): Reading state information... Done
aws_instance.example[3] (remote-exec): Setting up nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): The following additional packages will be installed:
aws_instance.example[1] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[1] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[1] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[1] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[1] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[1] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[1] (remote-exec):   libnginx-mod-mail
aws_instance.example[1] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[1] (remote-exec):   libwebp6 libxpm4 nginx-common
aws_instance.example[1] (remote-exec):   nginx-core
aws_instance.example[1] (remote-exec): Suggested packages:
aws_instance.example[1] (remote-exec):   libgd-tools fcgiwrap nginx-doc
aws_instance.example[1] (remote-exec):   ssl-cert
aws_instance.example[0] (remote-exec): 95% [Working]
aws_instance.example[0] (remote-exec): 95% [10 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 96% [Working]
aws_instance.example[0] (remote-exec): 96% [11 Packages store 0 B]
aws_instance.example[0] (remote-exec): 96% [Working]
aws_instance.example[0] (remote-exec): 96% [12 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 96% [Working]
aws_instance.example[0] (remote-exec): 96% [13 Packages store 0 B]
aws_instance.example[1] (remote-exec): The following NEW packages will be installed:
aws_instance.example[1] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[1] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[1] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[1] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[1] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[1] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[1] (remote-exec):   libnginx-mod-mail
aws_instance.example[1] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[1] (remote-exec):   libwebp6 libxpm4 nginx nginx-common
aws_instance.example[1] (remote-exec):   nginx-core
aws_instance.example[1] (remote-exec): 0 upgraded, 18 newly installed, 0 to remove and 20 not upgraded.
aws_instance.example[1] (remote-exec): Need to get 2462 kB of archives.
aws_instance.example[1] (remote-exec): After this operation, 8210 kB of additional disk space will be used.
aws_instance.example[1] (remote-exec): 0% [Working]
aws_instance.example[1] (remote-exec): Get:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libjpeg-turbo8 amd64 1.5.2-0ubuntu5.18.04.3 [110 kB]
aws_instance.example[1] (remote-exec): 0% [1 libjpeg-turbo8 0 B/110 kB 0%]
aws_instance.example[1] (remote-exec): 5% [Working]
aws_instance.example[1] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fonts-dejavu-core all 2.37-1 [1041 kB]
aws_instance.example[1] (remote-exec): 5% [2 fonts-dejavu-core 0 B/1041 kB 0%]
aws_instance.example[1] (remote-exec): 40% [Working]
aws_instance.example[1] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fontconfig-config all 2.12.6-0ubuntu2 [55.8 kB]
aws_instance.example[1] (remote-exec): 40% [3 fontconfig-config 0 B/55.8 kB 0%
aws_instance.example[1] (remote-exec): 43% [Working]
aws_instance.example[1] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libfontconfig1 amd64 2.12.6-0ubuntu2 [137 kB]
aws_instance.example[1] (remote-exec): 43% [4 libfontconfig1 0 B/137 kB 0%]
aws_instance.example[1] (remote-exec): 48% [Working]
aws_instance.example[1] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjpeg8 amd64 8c-2ubuntu8 [2194 B]
aws_instance.example[1] (remote-exec): 48% [5 libjpeg8 0 B/2194 B 0%]
aws_instance.example[1] (remote-exec): 49% [Working]
aws_instance.example[1] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjbig0 amd64 2.1-3.1build1 [26.7 kB]
aws_instance.example[1] (remote-exec): 49% [6 libjbig0 0 B/26.7 kB 0%]
aws_instance.example[1] (remote-exec): 51% [Working]
aws_instance.example[1] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libtiff5 amd64 4.0.9-5ubuntu0.3 [153 kB]
aws_instance.example[1] (remote-exec): 51% [7 libtiff5 0 B/153 kB 0%]
aws_instance.example[1] (remote-exec): 57% [Working]
aws_instance.example[1] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libwebp6 amd64 0.6.1-2 [185 kB]
aws_instance.example[1] (remote-exec): 57% [8 libwebp6 0 B/185 kB 0%]
aws_instance.example[1] (remote-exec): 64% [Working]
aws_instance.example[1] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libxpm4 amd64 1:3.5.12-1 [34.0 kB]
aws_instance.example[1] (remote-exec): 64% [9 libxpm4 0 B/34.0 kB 0%]
aws_instance.example[1] (remote-exec): 67% [Working]
aws_instance.example[1] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libgd3 amd64 2.2.5-4ubuntu0.4 [119 kB]
aws_instance.example[1] (remote-exec): 67% [10 libgd3 0 B/119 kB 0%]
aws_instance.example[1] (remote-exec): 72% [Working]
aws_instance.example[1] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-common all 1.14.0-0ubuntu1.7 [37.4 kB]
aws_instance.example[1] (remote-exec): 72% [11 nginx-common 0 B/37.4 kB 0%]
aws_instance.example[1] (remote-exec): 74% [Working]
aws_instance.example[1] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-geoip amd64 1.14.0-0ubuntu1.7 [11.2 kB]
aws_instance.example[1] (remote-exec): 74% [12 libnginx-mod-http-geoip 0 B/11.
aws_instance.example[1] (remote-exec): 75% [Working]
aws_instance.example[1] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-image-filter amd64 1.14.0-0ubuntu1.7 [14.6 kB]
aws_instance.example[1] (remote-exec): 75% [13 libnginx-mod-http-image-filter
aws_instance.example[1] (remote-exec): 77% [Working]
aws_instance.example[1] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.14.0-0ubuntu1.7 [13.0 kB]
aws_instance.example[1] (remote-exec): 77% [14 libnginx-mod-http-xslt-filter 0
aws_instance.example[1] (remote-exec): 79% [Working]
aws_instance.example[1] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-mail amd64 1.14.0-0ubuntu1.7 [41.8 kB]
aws_instance.example[1] (remote-exec): 79% [15 libnginx-mod-mail 0 B/41.8 kB 0
aws_instance.example[1] (remote-exec): 81% [Working]
aws_instance.example[1] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-stream amd64 1.14.0-0ubuntu1.7 [63.7 kB]
aws_instance.example[1] (remote-exec): 81% [16 libnginx-mod-stream 0 B/63.7 kB
aws_instance.example[1] (remote-exec): 84% [Working]
aws_instance.example[1] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-core amd64 1.14.0-0ubuntu1.7 [413 kB]
aws_instance.example[1] (remote-exec): 84% [17 nginx-core 0 B/413 kB 0%]
aws_instance.example[1] (remote-exec): 99% [Working]
aws_instance.example[1] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx all 1.14.0-0ubuntu1.7 [3596 B]
aws_instance.example[1] (remote-exec): 99% [18 nginx 0 B/3596 B 0%]
aws_instance.example[1] (remote-exec): 100% [Working]
aws_instance.example[1] (remote-exec): Fetched 2462 kB in 0s (28.0 MB/s)
aws_instance.example[0] (remote-exec): 96% [Working]
aws_instance.example[0] (remote-exec): 96% [14 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 97% [Working]
aws_instance.example[0] (remote-exec): 97% [15 Packages store 0 B]
aws_instance.example[0] (remote-exec): 97% [Working]
aws_instance.example[0] (remote-exec): 97% [16 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 97% [Working]
aws_instance.example[0] (remote-exec): 97% [17 Packages store 0 B]
aws_instance.example[0] (remote-exec): 97% [Working]
aws_instance.example[0] (remote-exec): 97% [18 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 98% [Working]
aws_instance.example[0] (remote-exec): 98% [19 Packages store 0 B]
aws_instance.example[0] (remote-exec): 98% [Working]
aws_instance.example[0] (remote-exec): 98% [20 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 98% [Working]
aws_instance.example[0] (remote-exec): 98% [21 Packages store 0 B]
aws_instance.example[3] (remote-exec): Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
aws_instance.example[1] (remote-exec): Preconfiguring packages ...
aws_instance.example[0] (remote-exec): 98% [Working]
aws_instance.example[0] (remote-exec): 98% [22 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 99% [Working]
aws_instance.example[0] (remote-exec): 99% [23 Packages store 0 B]
aws_instance.example[0] (remote-exec): 99% [Working]
aws_instance.example[0] (remote-exec): 99% [24 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 99% [Working]
aws_instance.example[0] (remote-exec): 99% [25 Packages store 0 B]
aws_instance.example[1] (remote-exec): Selecting previously unselected package libjpeg-turbo8:amd64.
aws_instance.example[0] (remote-exec): 99% [Working]
aws_instance.example[0] (remote-exec): 99% [26 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 100% [Working]
aws_instance.example[0] (remote-exec): 100% [27 Packages store 0 B]
aws_instance.example[0] (remote-exec): 100% [Working]
aws_instance.example[0] (remote-exec): 100% [28 Translation-en store 0 B]
aws_instance.example[0] (remote-exec): 100% [Working]
aws_instance.example[0] (remote-exec): Fetched 18.7 MB in 4s (4878 kB/s)
aws_instance.example[1] (remote-exec): (Reading database ...
aws_instance.example[1] (remote-exec): (Reading database ... 5%
aws_instance.example[1] (remote-exec): (Reading database ... 10%
aws_instance.example[1] (remote-exec): (Reading database ... 15%
aws_instance.example[1] (remote-exec): (Reading database ... 20%
aws_instance.example[1] (remote-exec): (Reading database ... 25%
aws_instance.example[1] (remote-exec): (Reading database ... 30%
aws_instance.example[1] (remote-exec): (Reading database ... 35%
aws_instance.example[1] (remote-exec): (Reading database ... 40%
aws_instance.example[1] (remote-exec): (Reading database ... 45%
aws_instance.example[1] (remote-exec): (Reading database ... 50%
aws_instance.example[1] (remote-exec): (Reading database ... 55%
aws_instance.example[1] (remote-exec): (Reading database ... 60%
aws_instance.example[1] (remote-exec): (Reading database ... 65%
aws_instance.example[1] (remote-exec): (Reading database ... 70%
aws_instance.example[1] (remote-exec): (Reading database ... 75%
aws_instance.example[1] (remote-exec): (Reading database ... 80%
aws_instance.example[1] (remote-exec): (Reading database ... 85%
aws_instance.example[1] (remote-exec): (Reading database ... 90%
aws_instance.example[1] (remote-exec): (Reading database ... 95%
aws_instance.example[1] (remote-exec): (Reading database ... 100%
aws_instance.example[1] (remote-exec): (Reading database ... 56588 files and directories currently installed.)
aws_instance.example[1] (remote-exec): Preparing to unpack .../00-libjpeg-turbo8_1.5.2-0ubuntu5.18.04.3_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[3] (remote-exec): Setting up libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[3] (remote-exec): Setting up libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package fonts-dejavu-core.
aws_instance.example[1] (remote-exec): Preparing to unpack .../01-fonts-dejavu-core_2.37-1_all.deb ...
aws_instance.example[1] (remote-exec): Unpacking fonts-dejavu-core (2.37-1) ...
aws_instance.example[3] (remote-exec): Setting up libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[3] (remote-exec): Setting up libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Setting up libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Setting up libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[3] (remote-exec): Setting up libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package fontconfig-config.
aws_instance.example[1] (remote-exec): Preparing to unpack .../02-fontconfig-config_2.12.6-0ubuntu2_all.deb ...
aws_instance.example[1] (remote-exec): Unpacking fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[3] (remote-exec): Setting up fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libfontconfig1:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../03-libfontconfig1_2.12.6-0ubuntu2_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libjpeg8:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../04-libjpeg8_8c-2ubuntu8_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libjbig0:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../05-libjbig0_2.1-3.1build1_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libtiff5:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../06-libtiff5_4.0.9-5ubuntu0.3_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[3] (remote-exec): Setting up libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libwebp6:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../07-libwebp6_0.6.1-2_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[3] (remote-exec): Setting up libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[3] (remote-exec): Setting up libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[3] (remote-exec): Setting up libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libxpm4:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../08-libxpm4_1%3a3.5.12-1_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[3] (remote-exec): Setting up libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Setting up nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libgd3:amd64.
aws_instance.example[1] (remote-exec): Preparing to unpack .../09-libgd3_2.2.5-4ubuntu0.4_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package nginx-common.
aws_instance.example[1] (remote-exec): Preparing to unpack .../10-nginx-common_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[1] (remote-exec): Unpacking nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Setting up nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libnginx-mod-http-geoip.
aws_instance.example[3] (remote-exec): Processing triggers for systemd (237-3ubuntu10.39) ...
aws_instance.example[1] (remote-exec): Preparing to unpack .../11-libnginx-mod-http-geoip_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libnginx-mod-http-image-filter.
aws_instance.example[1] (remote-exec): Preparing to unpack .../12-libnginx-mod-http-image-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[3] (remote-exec): Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libnginx-mod-http-xslt-filter.
aws_instance.example[1] (remote-exec): Preparing to unpack .../13-libnginx-mod-http-xslt-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libnginx-mod-mail.
aws_instance.example[1] (remote-exec): Preparing to unpack .../14-libnginx-mod-mail_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package libnginx-mod-stream.
aws_instance.example[1] (remote-exec): Preparing to unpack .../15-libnginx-mod-stream_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package nginx-core.
aws_instance.example[1] (remote-exec): Preparing to unpack .../16-nginx-core_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[1] (remote-exec): Unpacking nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Selecting previously unselected package nginx.
aws_instance.example[1] (remote-exec): Preparing to unpack .../17-nginx_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[1] (remote-exec): Unpacking nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Setting up libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[1]: Still creating... [1m0s elapsed]
aws_instance.example[0]: Still creating... [1m0s elapsed]
aws_instance.example[3]: Still creating... [1m0s elapsed]
aws_instance.example[2]: Still creating... [1m0s elapsed]
aws_instance.example[1] (remote-exec): Setting up fonts-dejavu-core (2.37-1) ...
aws_instance.example[3] (remote-exec): Processing triggers for ufw (0.36-0ubuntu0.18.04.1) ...
aws_instance.example[3] (remote-exec): Processing triggers for ureadahead (0.100.0-21) ...
aws_instance.example[3] (remote-exec): Processing triggers for libc-bin (2.27-3ubuntu1) ...
aws_instance.example[1] (remote-exec): Setting up nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Reading package lists... 0%
aws_instance.example[0] (remote-exec): Reading package lists... 0%
aws_instance.example[0] (remote-exec): Reading package lists... 0%
aws_instance.example[0] (remote-exec): Reading package lists... 4%
aws_instance.example[0] (remote-exec): Reading package lists... 4%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[0] (remote-exec): Reading package lists... 7%
aws_instance.example[1] (remote-exec): Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
aws_instance.example[1] (remote-exec): Setting up libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[1] (remote-exec): Setting up libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Setting up libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[1] (remote-exec): Setting up libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Setting up libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Setting up libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[1] (remote-exec): Setting up libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[1] (remote-exec): Setting up fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): Reading package lists... 46%
aws_instance.example[0] (remote-exec): Reading package lists... 46%
aws_instance.example[0] (remote-exec): Reading package lists... 66%
aws_instance.example[0] (remote-exec): Reading package lists... 66%
aws_instance.example[0] (remote-exec): Reading package lists... 67%
aws_instance.example[0] (remote-exec): Reading package lists... 67%
aws_instance.example[0] (remote-exec): Reading package lists... 67%
aws_instance.example[0] (remote-exec): Reading package lists... 67%
aws_instance.example[0] (remote-exec): Reading package lists... 70%
aws_instance.example[0] (remote-exec): Reading package lists... 73%
aws_instance.example[0] (remote-exec): Reading package lists... 73%
aws_instance.example[0] (remote-exec): Reading package lists... 76%
aws_instance.example[0] (remote-exec): Reading package lists... 76%
aws_instance.example[0] (remote-exec): Reading package lists... 77%
aws_instance.example[0] (remote-exec): Reading package lists... 77%
aws_instance.example[0] (remote-exec): Reading package lists... 77%
aws_instance.example[0] (remote-exec): Reading package lists... 77%
aws_instance.example[0] (remote-exec): Reading package lists... 83%
aws_instance.example[0] (remote-exec): Reading package lists... 83%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 86%
aws_instance.example[0] (remote-exec): Reading package lists... 90%
aws_instance.example[0] (remote-exec): Reading package lists... 90%
aws_instance.example[0] (remote-exec): Reading package lists... 93%
aws_instance.example[0] (remote-exec): Reading package lists... 93%
aws_instance.example[0] (remote-exec): Reading package lists... 93%
aws_instance.example[0] (remote-exec): Reading package lists... 93%
aws_instance.example[0] (remote-exec): Reading package lists... 94%
aws_instance.example[0] (remote-exec): Reading package lists... 94%
aws_instance.example[0] (remote-exec): Reading package lists... 97%
aws_instance.example[0] (remote-exec): Reading package lists... 97%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... 99%
aws_instance.example[0] (remote-exec): Reading package lists... Done
aws_instance.example[0] (remote-exec): Reading package lists... 0%
aws_instance.example[0] (remote-exec): Reading package lists... 100%
aws_instance.example[0] (remote-exec): Reading package lists... Done
aws_instance.example[0] (remote-exec): Building dependency tree... 0%
aws_instance.example[0] (remote-exec): Building dependency tree... 0%
aws_instance.example[0] (remote-exec): Building dependency tree... 50%
aws_instance.example[0] (remote-exec): Building dependency tree... 50%
aws_instance.example[0] (remote-exec): Building dependency tree
aws_instance.example[0] (remote-exec): Reading state information... 0%
aws_instance.example[0] (remote-exec): Reading state information... 0%
aws_instance.example[0] (remote-exec): Reading state information... Done
aws_instance.example[0] (remote-exec): The following additional packages will be installed:
aws_instance.example[0] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[0] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[0] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[0] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[0] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[0] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[0] (remote-exec):   libnginx-mod-mail
aws_instance.example[0] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[0] (remote-exec):   libwebp6 libxpm4 nginx-common
aws_instance.example[0] (remote-exec):   nginx-core
aws_instance.example[0] (remote-exec): Suggested packages:
aws_instance.example[0] (remote-exec):   libgd-tools fcgiwrap nginx-doc
aws_instance.example[0] (remote-exec):   ssl-cert
aws_instance.example[0] (remote-exec): The following NEW packages will be installed:
aws_instance.example[0] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[0] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[0] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[0] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[0] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[0] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[0] (remote-exec):   libnginx-mod-mail
aws_instance.example[0] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[0] (remote-exec):   libwebp6 libxpm4 nginx nginx-common
aws_instance.example[0] (remote-exec):   nginx-core
aws_instance.example[0] (remote-exec): 0 upgraded, 18 newly installed, 0 to remove and 20 not upgraded.
aws_instance.example[0] (remote-exec): Need to get 2462 kB of archives.
aws_instance.example[0] (remote-exec): After this operation, 8210 kB of additional disk space will be used.
aws_instance.example[0] (remote-exec): 0% [Working]
aws_instance.example[0] (remote-exec): Get:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libjpeg-turbo8 amd64 1.5.2-0ubuntu5.18.04.3 [110 kB]
aws_instance.example[0] (remote-exec): 0% [1 libjpeg-turbo8 0 B/110 kB 0%]
aws_instance.example[0] (remote-exec): 5% [Working]
aws_instance.example[0] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fonts-dejavu-core all 2.37-1 [1041 kB]
aws_instance.example[0] (remote-exec): 5% [2 fonts-dejavu-core 0 B/1041 kB 0%]
aws_instance.example[0] (remote-exec): 40% [Working]
aws_instance.example[0] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fontconfig-config all 2.12.6-0ubuntu2 [55.8 kB]
aws_instance.example[0] (remote-exec): 40% [3 fontconfig-config 0 B/55.8 kB 0%
aws_instance.example[0] (remote-exec): 43% [Working]
aws_instance.example[0] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libfontconfig1 amd64 2.12.6-0ubuntu2 [137 kB]
aws_instance.example[0] (remote-exec): 43% [4 libfontconfig1 0 B/137 kB 0%]
aws_instance.example[0] (remote-exec): 48% [Working]
aws_instance.example[0] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjpeg8 amd64 8c-2ubuntu8 [2194 B]
aws_instance.example[0] (remote-exec): 48% [5 libjpeg8 0 B/2194 B 0%]
aws_instance.example[0] (remote-exec): 49% [Working]
aws_instance.example[0] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjbig0 amd64 2.1-3.1build1 [26.7 kB]
aws_instance.example[0] (remote-exec): 49% [6 libjbig0 0 B/26.7 kB 0%]
aws_instance.example[0] (remote-exec): 51% [Working]
aws_instance.example[0] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libtiff5 amd64 4.0.9-5ubuntu0.3 [153 kB]
aws_instance.example[0] (remote-exec): 51% [7 libtiff5 0 B/153 kB 0%]
aws_instance.example[0] (remote-exec): 57% [Working]
aws_instance.example[0] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libwebp6 amd64 0.6.1-2 [185 kB]
aws_instance.example[0] (remote-exec): 57% [8 libwebp6 0 B/185 kB 0%]
aws_instance.example[0] (remote-exec): 64% [Working]
aws_instance.example[0] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libxpm4 amd64 1:3.5.12-1 [34.0 kB]
aws_instance.example[0] (remote-exec): 64% [9 libxpm4 0 B/34.0 kB 0%]
aws_instance.example[0] (remote-exec): 67% [Working]
aws_instance.example[0] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libgd3 amd64 2.2.5-4ubuntu0.4 [119 kB]
aws_instance.example[0] (remote-exec): 67% [10 libgd3 0 B/119 kB 0%]
aws_instance.example[0] (remote-exec): 72% [Working]
aws_instance.example[0] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-common all 1.14.0-0ubuntu1.7 [37.4 kB]
aws_instance.example[0] (remote-exec): 72% [11 nginx-common 0 B/37.4 kB 0%]
aws_instance.example[0] (remote-exec): 74% [Working]
aws_instance.example[0] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-geoip amd64 1.14.0-0ubuntu1.7 [11.2 kB]
aws_instance.example[0] (remote-exec): 74% [12 libnginx-mod-http-geoip 0 B/11.
aws_instance.example[0] (remote-exec): 75% [Working]
aws_instance.example[0] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-image-filter amd64 1.14.0-0ubuntu1.7 [14.6 kB]
aws_instance.example[0] (remote-exec): 75% [13 libnginx-mod-http-image-filter
aws_instance.example[0] (remote-exec): 77% [Working]
aws_instance.example[0] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.14.0-0ubuntu1.7 [13.0 kB]
aws_instance.example[0] (remote-exec): 77% [14 libnginx-mod-http-xslt-filter 0
aws_instance.example[0] (remote-exec): 79% [Working]
aws_instance.example[0] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-mail amd64 1.14.0-0ubuntu1.7 [41.8 kB]
aws_instance.example[0] (remote-exec): 79% [15 libnginx-mod-mail 0 B/41.8 kB 0
aws_instance.example[0] (remote-exec): 81% [Working]
aws_instance.example[0] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-stream amd64 1.14.0-0ubuntu1.7 [63.7 kB]
aws_instance.example[1] (remote-exec): Setting up libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): 81% [16 libnginx-mod-stream 0 B/63.7 kB
aws_instance.example[0] (remote-exec): 84% [Working]
aws_instance.example[0] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-core amd64 1.14.0-0ubuntu1.7 [413 kB]
aws_instance.example[0] (remote-exec): 84% [17 nginx-core 0 B/413 kB 0%]
aws_instance.example[0] (remote-exec): 99% [Working]
aws_instance.example[0] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx all 1.14.0-0ubuntu1.7 [3596 B]
aws_instance.example[0] (remote-exec): 99% [18 nginx 0 B/3596 B 0%]
aws_instance.example[0] (remote-exec): 100% [Working]
aws_instance.example[0] (remote-exec): Fetched 2462 kB in 0s (28.6 MB/s)
aws_instance.example[1] (remote-exec): Setting up libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[1] (remote-exec): Setting up libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[1] (remote-exec): Setting up libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[1] (remote-exec): Setting up libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Setting up nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[3]: Creation complete after 1m2s [id=i-0229f2bbc685c206b]
aws_instance.example[0] (remote-exec): Preconfiguring packages ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libjpeg-turbo8:amd64.
aws_instance.example[1] (remote-exec): Setting up nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[1] (remote-exec): Processing triggers for systemd (237-3ubuntu10.39) ...
aws_instance.example[0] (remote-exec): (Reading database ...
aws_instance.example[0] (remote-exec): (Reading database ... 5%
aws_instance.example[0] (remote-exec): (Reading database ... 10%
aws_instance.example[0] (remote-exec): (Reading database ... 15%
aws_instance.example[0] (remote-exec): (Reading database ... 20%
aws_instance.example[0] (remote-exec): (Reading database ... 25%
aws_instance.example[0] (remote-exec): (Reading database ... 30%
aws_instance.example[0] (remote-exec): (Reading database ... 35%
aws_instance.example[0] (remote-exec): (Reading database ... 40%
aws_instance.example[0] (remote-exec): (Reading database ... 45%
aws_instance.example[0] (remote-exec): (Reading database ... 50%
aws_instance.example[0] (remote-exec): (Reading database ... 55%
aws_instance.example[0] (remote-exec): (Reading database ... 60%
aws_instance.example[0] (remote-exec): (Reading database ... 65%
aws_instance.example[0] (remote-exec): (Reading database ... 70%
aws_instance.example[0] (remote-exec): (Reading database ... 75%
aws_instance.example[0] (remote-exec): (Reading database ... 80%
aws_instance.example[0] (remote-exec): (Reading database ... 85%
aws_instance.example[0] (remote-exec): (Reading database ... 90%
aws_instance.example[0] (remote-exec): (Reading database ... 95%
aws_instance.example[0] (remote-exec): (Reading database ... 100%
aws_instance.example[0] (remote-exec): (Reading database ... 56588 files and directories currently installed.)
aws_instance.example[0] (remote-exec): Preparing to unpack .../00-libjpeg-turbo8_1.5.2-0ubuntu5.18.04.3_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[1] (remote-exec): Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package fonts-dejavu-core.
aws_instance.example[0] (remote-exec): Preparing to unpack .../01-fonts-dejavu-core_2.37-1_all.deb ...
aws_instance.example[0] (remote-exec): Unpacking fonts-dejavu-core (2.37-1) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package fontconfig-config.
aws_instance.example[0] (remote-exec): Preparing to unpack .../02-fontconfig-config_2.12.6-0ubuntu2_all.deb ...
aws_instance.example[0] (remote-exec): Unpacking fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libfontconfig1:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../03-libfontconfig1_2.12.6-0ubuntu2_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libjpeg8:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../04-libjpeg8_8c-2ubuntu8_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libjbig0:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../05-libjbig0_2.1-3.1build1_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[1] (remote-exec): Processing triggers for ufw (0.36-0ubuntu0.18.04.1) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libtiff5:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../06-libtiff5_4.0.9-5ubuntu0.3_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[1] (remote-exec): Processing triggers for ureadahead (0.100.0-21) ...
aws_instance.example[1] (remote-exec): Processing triggers for libc-bin (2.27-3ubuntu1) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libwebp6:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../07-libwebp6_0.6.1-2_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libxpm4:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../08-libxpm4_1%3a3.5.12-1_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libgd3:amd64.
aws_instance.example[0] (remote-exec): Preparing to unpack .../09-libgd3_2.2.5-4ubuntu0.4_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package nginx-common.
aws_instance.example[0] (remote-exec): Preparing to unpack .../10-nginx-common_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[0] (remote-exec): Unpacking nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libnginx-mod-http-geoip.
aws_instance.example[0] (remote-exec): Preparing to unpack .../11-libnginx-mod-http-geoip_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libnginx-mod-http-image-filter.
aws_instance.example[0] (remote-exec): Preparing to unpack .../12-libnginx-mod-http-image-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libnginx-mod-http-xslt-filter.
aws_instance.example[0] (remote-exec): Preparing to unpack .../13-libnginx-mod-http-xslt-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libnginx-mod-mail.
aws_instance.example[0] (remote-exec): Preparing to unpack .../14-libnginx-mod-mail_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package libnginx-mod-stream.
aws_instance.example[0] (remote-exec): Preparing to unpack .../15-libnginx-mod-stream_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package nginx-core.
aws_instance.example[0] (remote-exec): Preparing to unpack .../16-nginx-core_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[0] (remote-exec): Unpacking nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Selecting previously unselected package nginx.
aws_instance.example[0] (remote-exec): Preparing to unpack .../17-nginx_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[0] (remote-exec): Unpacking nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[0] (remote-exec): Setting up fonts-dejavu-core (2.37-1) ...
aws_instance.example[0] (remote-exec): Setting up nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[1]: Creation complete after 1m5s [id=i-01e05057eea04afaf]
aws_instance.example[0] (remote-exec): Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
aws_instance.example[0] (remote-exec): Setting up libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[0] (remote-exec): Setting up libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[0] (remote-exec): Setting up libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[0] (remote-exec): Setting up libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[0] (remote-exec): Setting up fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): Setting up libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[0] (remote-exec): Setting up libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[0] (remote-exec): Setting up libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[0] (remote-exec): Setting up libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Setting up nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[0] (remote-exec): Processing triggers for systemd (237-3ubuntu10.39) ...
aws_instance.example[0] (remote-exec): Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
aws_instance.example[0] (remote-exec): Processing triggers for ufw (0.36-0ubuntu0.18.04.1) ...
aws_instance.example[0] (remote-exec): Processing triggers for ureadahead (0.100.0-21) ...
aws_instance.example[0] (remote-exec): Processing triggers for libc-bin (2.27-3ubuntu1) ...
aws_instance.example[2]: Still creating... [1m10s elapsed]
aws_instance.example[0]: Still creating... [1m10s elapsed]
aws_instance.example[0]: Creation complete after 1m10s [id=i-05278ab5d3acd60a0]
aws_instance.example[2]: Provisioning with 'remote-exec'...
aws_instance.example[2] (remote-exec): Connecting to remote host via SSH...
aws_instance.example[2] (remote-exec):   Host: 52.79.94.144
aws_instance.example[2] (remote-exec):   User: ubuntu
aws_instance.example[2] (remote-exec):   Password: false
aws_instance.example[2] (remote-exec):   Private key: true
aws_instance.example[2] (remote-exec):   Certificate: false
aws_instance.example[2] (remote-exec):   SSH Agent: false
aws_instance.example[2] (remote-exec):   Checking Host Key: false
aws_instance.example[2] (remote-exec): Connected!
aws_instance.example[2]: Still creating... [1m20s elapsed]
aws_instance.example[2] (remote-exec): 0% [Working]
aws_instance.example[2] (remote-exec): Hit:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic InRelease
aws_instance.example[2] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[2] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
aws_instance.example[2] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB]
aws_instance.example[2] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[2] (remote-exec): 0% [1 InRelease gpgv 242 kB] [Connectin
aws_instance.example[2] (remote-exec): 0% [Connecting to security.ubuntu.com (
aws_instance.example[2] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[2] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe amd64 Packages [8570 kB]
aws_instance.example[2] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [4 Packag
aws_instance.example[2] (remote-exec): 0% [2 InRelease gpgv 88.7 kB] [Waiting
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[2] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/universe Translation-en [4941 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [2 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [5 Translatio
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse amd64 Packages [151 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/multiverse Translation-en [108 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 Packages [932 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:9 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main Translation-en [318 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted amd64 Packages [50.1 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/restricted Translation-en [12.6 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 Packages [1068 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/universe Translation-en [332 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse amd64 Packages [15.5 kB]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/multiverse Translation-en [6352 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [3 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[2] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main amd64 Packages [7516 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[2] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/main Translation-en [4764 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[2] (remote-exec): Get:19 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe amd64 Packages [7484 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [19 Packages
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [Waiting for
aws_instance.example[2] (remote-exec): Get:20 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-backports/universe Translation-en [4436 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B]
aws_instance.example[2] (remote-exec): 0% [4 Packages store 0 B] [9 InRelease
aws_instance.example[2] (remote-exec): 86% [4 Packages store 0 B]
aws_instance.example[2] (remote-exec): Get:21 http://security.ubuntu.com/ubuntu bionic-security/main amd64 Packages [707 kB]
aws_instance.example[2] (remote-exec): 86% [4 Packages store 0 B] [21 Packages
aws_instance.example[2] (remote-exec): 87% [21 Packages 82.6 kB/707 kB 12%]
aws_instance.example[2] (remote-exec): 87% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[2] (remote-exec): 88% [5 Translation-en store 0 B] [21 Pa
aws_instance.example[2] (remote-exec): 89% [21 Packages 586 kB/707 kB 83%]
aws_instance.example[2] (remote-exec): 89% [6 Packages store 0 B] [21 Packages
aws_instance.example[2] (remote-exec): 90% [21 Packages 628 kB/707 kB 89%]
aws_instance.example[2] (remote-exec): 90% [7 Translation-en store 0 B] [21 Pa
aws_instance.example[2] (remote-exec): 90% [21 Packages 659 kB/707 kB 93%]
aws_instance.example[2] (remote-exec): 90% [8 Packages store 0 B] [21 Packages
aws_instance.example[2] (remote-exec): 90% [8 Packages store 0 B]
aws_instance.example[2]: Still creating... [1m30s elapsed]
aws_instance.example[2] (remote-exec): 90% [Waiting for headers]
aws_instance.example[2] (remote-exec): 90% [10 Translation-en store 0 B] [Wait
aws_instance.example[2] (remote-exec): 91% [Waiting for headers]
aws_instance.example[2] (remote-exec): 91% [11 Packages store 0 B] [Waiting fo
aws_instance.example[2] (remote-exec): Get:22 http://security.ubuntu.com/ubuntu bionic-security/main Translation-en [224 kB]
aws_instance.example[2] (remote-exec): 91% [11 Packages store 0 B] [22 Transla
aws_instance.example[2] (remote-exec): 91% [22 Translation-en 14.3 kB/224 kB 6
aws_instance.example[2] (remote-exec): 91% [12 Translation-en store 0 B] [22 T
aws_instance.example[2] (remote-exec): 91% [22 Translation-en 34.5 kB/224 kB 1
aws_instance.example[2] (remote-exec): 91% [13 Packages store 0 B] [22 Transla
aws_instance.example[2] (remote-exec): 92% [13 Packages store 0 B] [Waiting fo
aws_instance.example[2] (remote-exec): Get:23 http://security.ubuntu.com/ubuntu bionic-security/restricted amd64 Packages [40.3 kB]
aws_instance.example[2] (remote-exec): 92% [13 Packages store 0 B] [23 Package
aws_instance.example[2] (remote-exec): Get:24 http://security.ubuntu.com/ubuntu bionic-security/restricted Translation-en [10.2 kB]
aws_instance.example[2] (remote-exec): 92% [13 Packages store 0 B] [24 Transla
aws_instance.example[2] (remote-exec): Get:25 http://security.ubuntu.com/ubuntu bionic-security/universe amd64 Packages [660 kB]
aws_instance.example[2] (remote-exec): 92% [13 Packages store 0 B] [25 Package
aws_instance.example[2] (remote-exec): 95% [25 Packages 473 kB/660 kB 72%]
aws_instance.example[2] (remote-exec): 95% [14 Translation-en store 0 B] [25 P
aws_instance.example[2] (remote-exec): Get:26 http://security.ubuntu.com/ubuntu bionic-security/universe Translation-en [219 kB]
aws_instance.example[2] (remote-exec): 95% [14 Translation-en store 0 B] [26 T
aws_instance.example[2] (remote-exec): 96% [26 Translation-en 130 kB/219 kB 59
aws_instance.example[2] (remote-exec): 96% [15 Packages store 0 B] [26 Transla
aws_instance.example[2] (remote-exec): 97% [26 Translation-en 147 kB/219 kB 67
aws_instance.example[2] (remote-exec): 97% [16 Translation-en store 0 B] [26 T
aws_instance.example[2] (remote-exec): 97% [26 Translation-en 156 kB/219 kB 71
aws_instance.example[2] (remote-exec): 97% [17 Packages store 0 B] [26 Transla
aws_instance.example[2] (remote-exec): 97% [26 Translation-en 165 kB/219 kB 75
aws_instance.example[2] (remote-exec): 97% [18 Translation-en store 0 B] [26 T
aws_instance.example[2] (remote-exec): 97% [26 Translation-en 170 kB/219 kB 78
aws_instance.example[2] (remote-exec): 97% [19 Packages store 0 B] [26 Transla
aws_instance.example[2] (remote-exec): 98% [26 Translation-en 178 kB/219 kB 81
aws_instance.example[2] (remote-exec): 98% [20 Translation-en store 0 B] [26 T
aws_instance.example[2] (remote-exec): 98% [26 Translation-en 183 kB/219 kB 84
aws_instance.example[2] (remote-exec): 98% [21 Packages store 0 B] [26 Transla
aws_instance.example[2] (remote-exec): Get:27 http://security.ubuntu.com/ubuntu bionic-security/multiverse amd64 Packages [7392 B]
aws_instance.example[2] (remote-exec): 98% [21 Packages store 0 B] [27 Package
aws_instance.example[2] (remote-exec): 98% [21 Packages store 0 B] [Waiting fo
aws_instance.example[2] (remote-exec): Get:28 http://security.ubuntu.com/ubuntu bionic-security/multiverse Translation-en [2788 B]
aws_instance.example[2] (remote-exec): 98% [21 Packages store 0 B] [28 Transla
aws_instance.example[2] (remote-exec): 98% [21 Packages store 0 B]
aws_instance.example[2] (remote-exec): 98% [Working]
aws_instance.example[2] (remote-exec): 98% [22 Translation-en store 0 B]
aws_instance.example[2] (remote-exec): 99% [Working]
aws_instance.example[2] (remote-exec): 99% [23 Packages store 0 B]
aws_instance.example[2] (remote-exec): 99% [Working]
aws_instance.example[2] (remote-exec): 99% [24 Translation-en store 0 B]
aws_instance.example[2] (remote-exec): 99% [Working]
aws_instance.example[2] (remote-exec): 99% [25 Packages store 0 B]
aws_instance.example[2] (remote-exec): 99% [Working]
aws_instance.example[2] (remote-exec): 99% [26 Translation-en store 0 B]
aws_instance.example[2] (remote-exec): 100% [Working]
aws_instance.example[2] (remote-exec): 100% [27 Packages store 0 B]
aws_instance.example[2] (remote-exec): 100% [Working]
aws_instance.example[2] (remote-exec): 100% [28 Translation-en store 0 B]
aws_instance.example[2] (remote-exec): 100% [Working]
aws_instance.example[2] (remote-exec): Fetched 18.7 MB in 4s (4890 kB/s)
aws_instance.example[2] (remote-exec): Reading package lists... 0%
aws_instance.example[2] (remote-exec): Reading package lists... 0%
aws_instance.example[2] (remote-exec): Reading package lists... 0%
aws_instance.example[2] (remote-exec): Reading package lists... 4%
aws_instance.example[2] (remote-exec): Reading package lists... 4%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 7%
aws_instance.example[2] (remote-exec): Reading package lists... 46%
aws_instance.example[2] (remote-exec): Reading package lists... 46%
aws_instance.example[2] (remote-exec): Reading package lists... 66%
aws_instance.example[2] (remote-exec): Reading package lists... 66%
aws_instance.example[2] (remote-exec): Reading package lists... 67%
aws_instance.example[2] (remote-exec): Reading package lists... 67%
aws_instance.example[2] (remote-exec): Reading package lists... 67%
aws_instance.example[2] (remote-exec): Reading package lists... 67%
aws_instance.example[2] (remote-exec): Reading package lists... 70%
aws_instance.example[2] (remote-exec): Reading package lists... 73%
aws_instance.example[2] (remote-exec): Reading package lists... 73%
aws_instance.example[2] (remote-exec): Reading package lists... 76%
aws_instance.example[2] (remote-exec): Reading package lists... 76%
aws_instance.example[2] (remote-exec): Reading package lists... 77%
aws_instance.example[2] (remote-exec): Reading package lists... 77%
aws_instance.example[2] (remote-exec): Reading package lists... 77%
aws_instance.example[2] (remote-exec): Reading package lists... 77%
aws_instance.example[2] (remote-exec): Reading package lists... 83%
aws_instance.example[2] (remote-exec): Reading package lists... 83%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 86%
aws_instance.example[2] (remote-exec): Reading package lists... 90%
aws_instance.example[2] (remote-exec): Reading package lists... 90%
aws_instance.example[2] (remote-exec): Reading package lists... 93%
aws_instance.example[2] (remote-exec): Reading package lists... 93%
aws_instance.example[2] (remote-exec): Reading package lists... 93%
aws_instance.example[2] (remote-exec): Reading package lists... 93%
aws_instance.example[2] (remote-exec): Reading package lists... 94%
aws_instance.example[2] (remote-exec): Reading package lists... 94%
aws_instance.example[2] (remote-exec): Reading package lists... 97%
aws_instance.example[2] (remote-exec): Reading package lists... 97%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... 99%
aws_instance.example[2] (remote-exec): Reading package lists... Done
aws_instance.example[2] (remote-exec): Reading package lists... 0%
aws_instance.example[2] (remote-exec): Reading package lists... 100%
aws_instance.example[2] (remote-exec): Reading package lists... Done
aws_instance.example[2] (remote-exec): Building dependency tree... 0%
aws_instance.example[2] (remote-exec): Building dependency tree... 0%
aws_instance.example[2] (remote-exec): Building dependency tree... 50%
aws_instance.example[2] (remote-exec): Building dependency tree... 50%
aws_instance.example[2] (remote-exec): Building dependency tree
aws_instance.example[2] (remote-exec): Reading state information... 0%
aws_instance.example[2] (remote-exec): Reading state information... 0%
aws_instance.example[2] (remote-exec): Reading state information... Done
aws_instance.example[2] (remote-exec): The following additional packages will be installed:
aws_instance.example[2] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[2] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[2] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[2] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[2] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[2] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[2] (remote-exec):   libnginx-mod-mail
aws_instance.example[2] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[2] (remote-exec):   libwebp6 libxpm4 nginx-common
aws_instance.example[2] (remote-exec):   nginx-core
aws_instance.example[2] (remote-exec): Suggested packages:
aws_instance.example[2] (remote-exec):   libgd-tools fcgiwrap nginx-doc
aws_instance.example[2] (remote-exec):   ssl-cert
aws_instance.example[2] (remote-exec): The following NEW packages will be installed:
aws_instance.example[2] (remote-exec):   fontconfig-config fonts-dejavu-core
aws_instance.example[2] (remote-exec):   libfontconfig1 libgd3 libjbig0
aws_instance.example[2] (remote-exec):   libjpeg-turbo8 libjpeg8
aws_instance.example[2] (remote-exec):   libnginx-mod-http-geoip
aws_instance.example[2] (remote-exec):   libnginx-mod-http-image-filter
aws_instance.example[2] (remote-exec):   libnginx-mod-http-xslt-filter
aws_instance.example[2] (remote-exec):   libnginx-mod-mail
aws_instance.example[2] (remote-exec):   libnginx-mod-stream libtiff5
aws_instance.example[2] (remote-exec):   libwebp6 libxpm4 nginx nginx-common
aws_instance.example[2] (remote-exec):   nginx-core
aws_instance.example[2] (remote-exec): 0 upgraded, 18 newly installed, 0 to remove and 20 not upgraded.
aws_instance.example[2] (remote-exec): Need to get 2462 kB of archives.
aws_instance.example[2] (remote-exec): After this operation, 8210 kB of additional disk space will be used.
aws_instance.example[2] (remote-exec): 0% [Working]
aws_instance.example[2] (remote-exec): Get:1 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libjpeg-turbo8 amd64 1.5.2-0ubuntu5.18.04.3 [110 kB]
aws_instance.example[2] (remote-exec): 0% [1 libjpeg-turbo8 0 B/110 kB 0%]
aws_instance.example[2] (remote-exec): 5% [Working]
aws_instance.example[2] (remote-exec): Get:2 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fonts-dejavu-core all 2.37-1 [1041 kB]
aws_instance.example[2] (remote-exec): 5% [2 fonts-dejavu-core 0 B/1041 kB 0%]
aws_instance.example[2] (remote-exec): 40% [Working]
aws_instance.example[2] (remote-exec): Get:3 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 fontconfig-config all 2.12.6-0ubuntu2 [55.8 kB]
aws_instance.example[2] (remote-exec): 40% [3 fontconfig-config 0 B/55.8 kB 0%
aws_instance.example[2] (remote-exec): 43% [Working]
aws_instance.example[2] (remote-exec): Get:4 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libfontconfig1 amd64 2.12.6-0ubuntu2 [137 kB]
aws_instance.example[2] (remote-exec): 43% [4 libfontconfig1 0 B/137 kB 0%]
aws_instance.example[2] (remote-exec): 48% [Working]
aws_instance.example[2] (remote-exec): Get:5 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjpeg8 amd64 8c-2ubuntu8 [2194 B]
aws_instance.example[2] (remote-exec): 48% [5 libjpeg8 0 B/2194 B 0%]
aws_instance.example[2] (remote-exec): 49% [Working]
aws_instance.example[2] (remote-exec): Get:6 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libjbig0 amd64 2.1-3.1build1 [26.7 kB]
aws_instance.example[2] (remote-exec): 49% [6 libjbig0 0 B/26.7 kB 0%]
aws_instance.example[2] (remote-exec): 51% [Working]
aws_instance.example[2] (remote-exec): Get:7 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libtiff5 amd64 4.0.9-5ubuntu0.3 [153 kB]
aws_instance.example[2] (remote-exec): 51% [7 libtiff5 0 B/153 kB 0%]
aws_instance.example[2] (remote-exec): 57% [Working]
aws_instance.example[2] (remote-exec): Get:8 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libwebp6 amd64 0.6.1-2 [185 kB]
aws_instance.example[2] (remote-exec): 57% [8 libwebp6 0 B/185 kB 0%]
aws_instance.example[2] (remote-exec): 64% [Working]
aws_instance.example[2] (remote-exec): Get:9 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic/main amd64 libxpm4 amd64 1:3.5.12-1 [34.0 kB]
aws_instance.example[2] (remote-exec): 64% [9 libxpm4 0 B/34.0 kB 0%]
aws_instance.example[2] (remote-exec): 67% [Working]
aws_instance.example[2] (remote-exec): Get:10 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libgd3 amd64 2.2.5-4ubuntu0.4 [119 kB]
aws_instance.example[2] (remote-exec): 67% [10 libgd3 0 B/119 kB 0%]
aws_instance.example[2] (remote-exec): 72% [Working]
aws_instance.example[2] (remote-exec): Get:11 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-common all 1.14.0-0ubuntu1.7 [37.4 kB]
aws_instance.example[2] (remote-exec): 72% [11 nginx-common 0 B/37.4 kB 0%]
aws_instance.example[2] (remote-exec): 74% [Working]
aws_instance.example[2] (remote-exec): Get:12 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-geoip amd64 1.14.0-0ubuntu1.7 [11.2 kB]
aws_instance.example[2] (remote-exec): 74% [12 libnginx-mod-http-geoip 0 B/11.
aws_instance.example[2] (remote-exec): 75% [Working]
aws_instance.example[2] (remote-exec): Get:13 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-image-filter amd64 1.14.0-0ubuntu1.7 [14.6 kB]
aws_instance.example[2] (remote-exec): 75% [13 libnginx-mod-http-image-filter
aws_instance.example[2] (remote-exec): 77% [Working]
aws_instance.example[2] (remote-exec): Get:14 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.14.0-0ubuntu1.7 [13.0 kB]
aws_instance.example[2] (remote-exec): 77% [14 libnginx-mod-http-xslt-filter 0
aws_instance.example[2] (remote-exec): 79% [Working]
aws_instance.example[2] (remote-exec): Get:15 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-mail amd64 1.14.0-0ubuntu1.7 [41.8 kB]
aws_instance.example[2] (remote-exec): 79% [15 libnginx-mod-mail 0 B/41.8 kB 0
aws_instance.example[2] (remote-exec): 81% [Working]
aws_instance.example[2] (remote-exec): Get:16 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libnginx-mod-stream amd64 1.14.0-0ubuntu1.7 [63.7 kB]
aws_instance.example[2] (remote-exec): 81% [16 libnginx-mod-stream 0 B/63.7 kB
aws_instance.example[2] (remote-exec): 84% [Working]
aws_instance.example[2] (remote-exec): Get:17 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx-core amd64 1.14.0-0ubuntu1.7 [413 kB]
aws_instance.example[2] (remote-exec): 84% [17 nginx-core 0 B/413 kB 0%]
aws_instance.example[2] (remote-exec): 99% [Working]
aws_instance.example[2] (remote-exec): Get:18 http://ap-northeast-2.ec2.archive.ubuntu.com/ubuntu bionic-updates/main amd64 nginx all 1.14.0-0ubuntu1.7 [3596 B]
aws_instance.example[2] (remote-exec): 99% [18 nginx 0 B/3596 B 0%]
aws_instance.example[2] (remote-exec): 100% [Working]
aws_instance.example[2] (remote-exec): Fetched 2462 kB in 0s (30.6 MB/s)
aws_instance.example[2] (remote-exec): Preconfiguring packages ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libjpeg-turbo8:amd64.
aws_instance.example[2] (remote-exec): (Reading database ...
aws_instance.example[2] (remote-exec): (Reading database ... 5%
aws_instance.example[2] (remote-exec): (Reading database ... 10%
aws_instance.example[2] (remote-exec): (Reading database ... 15%
aws_instance.example[2] (remote-exec): (Reading database ... 20%
aws_instance.example[2] (remote-exec): (Reading database ... 25%
aws_instance.example[2] (remote-exec): (Reading database ... 30%
aws_instance.example[2] (remote-exec): (Reading database ... 35%
aws_instance.example[2] (remote-exec): (Reading database ... 40%
aws_instance.example[2] (remote-exec): (Reading database ... 45%
aws_instance.example[2] (remote-exec): (Reading database ... 50%
aws_instance.example[2] (remote-exec): (Reading database ... 55%
aws_instance.example[2] (remote-exec): (Reading database ... 60%
aws_instance.example[2] (remote-exec): (Reading database ... 65%
aws_instance.example[2] (remote-exec): (Reading database ... 70%
aws_instance.example[2] (remote-exec): (Reading database ... 75%
aws_instance.example[2] (remote-exec): (Reading database ... 80%
aws_instance.example[2] (remote-exec): (Reading database ... 85%
aws_instance.example[2] (remote-exec): (Reading database ... 90%
aws_instance.example[2] (remote-exec): (Reading database ... 95%
aws_instance.example[2] (remote-exec): (Reading database ... 100%
aws_instance.example[2] (remote-exec): (Reading database ... 56588 files and directories currently installed.)
aws_instance.example[2] (remote-exec): Preparing to unpack .../00-libjpeg-turbo8_1.5.2-0ubuntu5.18.04.3_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package fonts-dejavu-core.
aws_instance.example[2] (remote-exec): Preparing to unpack .../01-fonts-dejavu-core_2.37-1_all.deb ...
aws_instance.example[2] (remote-exec): Unpacking fonts-dejavu-core (2.37-1) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package fontconfig-config.
aws_instance.example[2] (remote-exec): Preparing to unpack .../02-fontconfig-config_2.12.6-0ubuntu2_all.deb ...
aws_instance.example[2] (remote-exec): Unpacking fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libfontconfig1:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../03-libfontconfig1_2.12.6-0ubuntu2_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libjpeg8:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../04-libjpeg8_8c-2ubuntu8_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libjbig0:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../05-libjbig0_2.1-3.1build1_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libtiff5:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../06-libtiff5_4.0.9-5ubuntu0.3_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libwebp6:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../07-libwebp6_0.6.1-2_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libxpm4:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../08-libxpm4_1%3a3.5.12-1_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libgd3:amd64.
aws_instance.example[2] (remote-exec): Preparing to unpack .../09-libgd3_2.2.5-4ubuntu0.4_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package nginx-common.
aws_instance.example[2] (remote-exec): Preparing to unpack .../10-nginx-common_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[2] (remote-exec): Unpacking nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libnginx-mod-http-geoip.
aws_instance.example[2] (remote-exec): Preparing to unpack .../11-libnginx-mod-http-geoip_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libnginx-mod-http-image-filter.
aws_instance.example[2] (remote-exec): Preparing to unpack .../12-libnginx-mod-http-image-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libnginx-mod-http-xslt-filter.
aws_instance.example[2] (remote-exec): Preparing to unpack .../13-libnginx-mod-http-xslt-filter_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libnginx-mod-mail.
aws_instance.example[2] (remote-exec): Preparing to unpack .../14-libnginx-mod-mail_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package libnginx-mod-stream.
aws_instance.example[2] (remote-exec): Preparing to unpack .../15-libnginx-mod-stream_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package nginx-core.
aws_instance.example[2] (remote-exec): Preparing to unpack .../16-nginx-core_1.14.0-0ubuntu1.7_amd64.deb ...
aws_instance.example[2] (remote-exec): Unpacking nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Selecting previously unselected package nginx.
aws_instance.example[2] (remote-exec): Preparing to unpack .../17-nginx_1.14.0-0ubuntu1.7_all.deb ...
aws_instance.example[2] (remote-exec): Unpacking nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up libjbig0:amd64 (2.1-3.1build1) ...
aws_instance.example[2] (remote-exec): Setting up fonts-dejavu-core (2.37-1) ...
aws_instance.example[2] (remote-exec): Setting up nginx-common (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
aws_instance.example[2] (remote-exec): Setting up libjpeg-turbo8:amd64 (1.5.2-0ubuntu5.18.04.3) ...
aws_instance.example[2] (remote-exec): Setting up libnginx-mod-mail (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up libxpm4:amd64 (1:3.5.12-1) ...
aws_instance.example[2] (remote-exec): Setting up libnginx-mod-http-xslt-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up libnginx-mod-http-geoip (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up libwebp6:amd64 (0.6.1-2) ...
aws_instance.example[2] (remote-exec): Setting up libjpeg8:amd64 (8c-2ubuntu8) ...
aws_instance.example[2] (remote-exec): Setting up fontconfig-config (2.12.6-0ubuntu2) ...
aws_instance.example[2] (remote-exec): Setting up libnginx-mod-stream (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up libtiff5:amd64 (4.0.9-5ubuntu0.3) ...
aws_instance.example[2] (remote-exec): Setting up libfontconfig1:amd64 (2.12.6-0ubuntu2) ...
aws_instance.example[2] (remote-exec): Setting up libgd3:amd64 (2.2.5-4ubuntu0.4) ...
aws_instance.example[2] (remote-exec): Setting up libnginx-mod-http-image-filter (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Setting up nginx-core (1.14.0-0ubuntu1.7) ...
aws_instance.example[2]: Still creating... [1m40s elapsed]
aws_instance.example[2] (remote-exec): Setting up nginx (1.14.0-0ubuntu1.7) ...
aws_instance.example[2] (remote-exec): Processing triggers for systemd (237-3ubuntu10.39) ...
aws_instance.example[2] (remote-exec): Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
aws_instance.example[2] (remote-exec): Processing triggers for ufw (0.36-0ubuntu0.18.04.1) ...
aws_instance.example[2] (remote-exec): Processing triggers for ureadahead (0.100.0-21) ...
aws_instance.example[2] (remote-exec): Processing triggers for libc-bin (2.27-3ubuntu1) ...
aws_instance.example[2]: Creation complete after 1m43s [id=i-036ec9767770dc993]

Apply complete! Resources: 5 added, 0 changed, 0 destroyed.
            "public_ip": "13.125.190.89",
            "public_ip": "3.34.90.51",
            "public_ip": "52.79.94.144",
            "public_ip": "13.209.21.21",
```
# ubuntu@u1:/mnt/hgfs/Desktop/sol3$ td
```
terraform destroy -auto-approve

aws_key_pair.mykey: Refreshing state... [id=mykey]
aws_instance.example[2]: Refreshing state... [id=i-036ec9767770dc993]
aws_instance.example[1]: Refreshing state... [id=i-01e05057eea04afaf]
aws_instance.example[3]: Refreshing state... [id=i-0229f2bbc685c206b]
aws_instance.example[0]: Refreshing state... [id=i-05278ab5d3acd60a0]
aws_instance.example[1]: Destroying... [id=i-01e05057eea04afaf]
aws_instance.example[2]: Destroying... [id=i-036ec9767770dc993]
aws_instance.example[0]: Destroying... [id=i-05278ab5d3acd60a0]
aws_instance.example[3]: Destroying... [id=i-0229f2bbc685c206b]
aws_instance.example[1]: Still destroying... [id=i-01e05057eea04afaf, 10s elapsed]
aws_instance.example[2]: Still destroying... [id=i-036ec9767770dc993, 10s elapsed]
aws_instance.example[0]: Still destroying... [id=i-05278ab5d3acd60a0, 10s elapsed]
aws_instance.example[3]: Still destroying... [id=i-0229f2bbc685c206b, 10s elapsed]
aws_instance.example[1]: Destruction complete after 20s
aws_instance.example[2]: Still destroying... [id=i-036ec9767770dc993, 20s elapsed]
aws_instance.example[0]: Still destroying... [id=i-05278ab5d3acd60a0, 20s elapsed]
aws_instance.example[3]: Still destroying... [id=i-0229f2bbc685c206b, 20s elapsed]
aws_instance.example[0]: Still destroying... [id=i-05278ab5d3acd60a0, 30s elapsed]
aws_instance.example[2]: Still destroying... [id=i-036ec9767770dc993, 30s elapsed]
aws_instance.example[3]: Still destroying... [id=i-0229f2bbc685c206b, 30s elapsed]
aws_instance.example[2]: Destruction complete after 30s
aws_instance.example[0]: Destruction complete after 30s
aws_instance.example[3]: Destruction complete after 30s
aws_key_pair.mykey: Destroying... [id=mykey]
aws_key_pair.mykey: Destruction complete after 0s

Destroy complete! Resources: 5 destroyed.
```
