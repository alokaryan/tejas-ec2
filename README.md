# tejas-ec2

this module will create a ec2 instance on aws

##USAGE

provider "aws" {
   region = "ap-south-1"
   }
   
   module "tejas-ec2" {
      source = "github.com/alokaryan/tejas-ec2"
      ami_id = "ami-id-of-your-choice"
      instance_type = "instance-type"
      vpc_id = "your-vpc-id"
      port = "your-port"
      cidr_block = "0.0.0.0/0"
      }
      
