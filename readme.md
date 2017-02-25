# MINEformation

## About
MINEformation is a learning exercise that leverages the beloved and familiar Minecraft to 
demonstrate the power of AWS.

## Assumptions
- User has created an EC2 keypair named mineformationKP.
- User has a registered hosted zone with AWS.

## Usage
This cloudformation template assumes you have registered at least one hosted zone with AWS.

Simply load the cloudformation template from your AWS account by a user with administrative access
and you are good to go! Once your EC2 instance has passed health check, you should be able to 
use Minecrafts online mode to connect to the server's public IP address.

## Implemented features
- EC2 instance installs minecraft server at boot time using UserData.
- Auto scaling group maintains 1 running server at all times, even after system termination.
- ELB DNS name registers itself to your domain.

## Planned features
- To the greatest extent possible the project will be managed via a single
cloudformation template. There will be some limitations here like the creation of SSH keys.
- Fully functional Minecraft server on a Linux based AMI to keep costs low.
- Deployable to a configurable region passed through cloudformation parameter.
- Demonstrated usage of pseudo parameters.
- CloudWatch and SNS integration.