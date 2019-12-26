# nifi registry
Apache NiFi Registry

## deploy nifi registry
NiFi Registry can be provisioned in parallel with kafka cluster deployment as there is no overlap at this stage. Running time is about four and a half minutes on AWS for a minimal number of hosts (3):

    ec2_region=${AWS_DEFAULT_REGION} eval ./deploy ${platform_root}/${TENANT}/inventory/hostsfile-'${ec2_region}'-demo.none $platform_root/${TENANT} demo aws '$ec2_region' development none
