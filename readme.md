# MINEformation

## About
MINEformation is a learning exercise that leverages the beloved and familiar Minecraft to
demonstrate the power of AWS.

## Assumptions
- User has created an EC2 keypair named mineformationKP.
- Optional - User has a registered hosted zone with AWS.

## Usage
This cloudformation template assumes you have registered at least one hosted zone with AWS.

Simply load the cloudformation template from your AWS account by a user with administrative access
and you are good to go! Once your EC2 instance has passed health check, you should be able to
use Minecraft's online mode to connect to the server's public IP address.

## Implemented features
- Elastic IP address connects to EC2 and optionally registers with a hosted zone.
- EC2 automatically downloads and installs minecraft.

## Planned features
- Regular Snapshots
- Cloudwatch alarms and automated responses
- SNS topic integration
