# MINEformation

## About
MINEformation is a learning exercise that leverages the beloved and familiar Minecraft to 
demonstrate the power of AWS.

## Usage
Simply load the cloudformation template from your AWS account by a user with administrative access
and you are good to go! Once your EC2 instance has passed health check, you should be able to 
use Minecrafts online mode to connect to the server's public IP address.

## Planned features.
- To the greatest extent possible the project will be managed via a single
cloudformation template. There will be some limitations here like the creation of SSH keys.
- Fully functional Minecraft server on a Linux based AMI to keep costs low.
- Regular backups of the Minecraft world to S3.
- S3 bucket lifecycle policies to keep costs low.
- Route 53 integration so the server can be resolved at parameter.domain.com
- Autoscaling to rebuild the server in the case of a server crash. 