provider "aws" {
region = "us-east-1"
}

resource "aws_instance" "one" {
count = var.instance_count
ami = "ami-0b41f7055516b991a"
instance_type = var.instance_type
}
