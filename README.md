# EC2 based Snowplow deployment

To deploy and run Snowplow on AWS do the following:

1. Configure group_vars/all for your deployment
2. Run ./create_certs.yml to create certificates required SSL termination. After this step you will recive a mail from Amazon Certificate Manager, to confirm you are the domain owner.
3. Run ./site.yml to install provision EC2 instances, loadbalancers and install snowplow.
