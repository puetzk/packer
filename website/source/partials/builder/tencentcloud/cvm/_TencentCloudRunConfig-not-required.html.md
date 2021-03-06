<!-- Code generated from the comments of the TencentCloudRunConfig struct in builder/tencentcloud/cvm/run_config.go; DO NOT EDIT MANUALLY -->

-   `associate_public_ip_address` (bool) - Whether allocate public ip to your cvm.
    Default value is false.
    
-   `instance_name` (string) - Instance name.
    
-   `disk_type` (string) - Root disk type your cvm will be launched by. you could
    reference Disk Type
    for parameter taking.
    
-   `disk_size` (int64) - Root disk size your cvm will be launched by. values range(in GB):
    
-   `data_disks` ([]tencentCloudDataDisk) - Add one or more data disks to the instance before creating the image.
    Note that if the source image has data disk snapshots, this argument
    will be ignored, and the running instance will use source image data
    disk settings, in such case, `disk_type` argument will be used as disk
    type for all data disks, and each data disk size will use the origin
    value in source image.
    The data disks allow for the following argument:
    -  `disk_type` - Type of the data disk. Valid choices: `CLOUD_BASIC`, `CLOUD_PREMIUM` and `CLOUD_SSD`.
    -  `disk_size` - Size of the data disk.
    -  `disk_snapshot_id` - Id of the snapshot for a data disk.
    
-   `vpc_id` (string) - Specify vpc your cvm will be launched by.
    
-   `vpc_name` (string) - Specify vpc name you will create. if vpc_id is not set, packer will
    create a vpc for you named this parameter.
    
-   `vpc_ip` (string) - Vpc Ip
-   `subnet_id` (string) - Specify subnet your cvm will be launched by.
    
-   `subnet_name` (string) - Specify subnet name you will create. if subnet_id is not set, packer will
    create a subnet for you named this parameter.
    
-   `cidr_block` (string) - Specify cider block of the vpc you will create if vpc_id not set
    
-   `subnect_cidr_block` (string) - Specify cider block of the subnet you will create if
    subnet_id not set
    
-   `internet_charge_type` (string) - Internet Charge Type
-   `internet_max_bandwidth_out` (int64) - Max bandwidth out your cvm will be launched by(in MB).
    values can be set between 1 ~ 100.
    
-   `security_group_id` (string) - Specify security group your cvm will be launched by.
    
-   `security_group_name` (string) - Specify security name you will create if security_group_id not set.
    
-   `user_data` (string) - userdata.
    
-   `user_data_file` (string) - userdata file.
    
-   `host_name` (string) - host name.
    
-   `run_tags` (map[string]string) - Tags to apply to the instance that is *launched* to create the image.
    These tags are *not* applied to the resulting image.
    
-   `ssh_private_ip` (bool) - SSH Private Ip