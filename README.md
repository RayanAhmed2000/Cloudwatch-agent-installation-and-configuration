# Cloudwatch-agent-installation-and-configuration
```
sudo yum install amazon-cloudwatch-agent -y
```
- alla configuartion files of cloudwatch agent
```
cd /opt/aws/amazon-cloudwatch-agent/bin/
```
- Now we to configure what metrices need to be sent using cloudwatch agent wizard
```
./amazon-cloudwatch-agent-config-wizard
```
```
./amazon-cloudwatch-agent-ctl -a fetch-config -m ec2 -s -c file:config.json
```
# Creating alarms for CUSTOM metrices
- Although clouwatch provides all the required metrices but in some cases we will have to create our own metrics
- For example for on of clients GSTN-E-Invoicing client said create a dashboard of cloudwatch in which track *Number of API calls recived and from which IRP*
- All data is saved in Log groups
- from there we will create *a metric filter*
