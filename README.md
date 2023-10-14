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
