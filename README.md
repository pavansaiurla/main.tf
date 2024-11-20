provider "aws" {
region = "us-east-1"
}

resource "aws_instance" "one" {
count = "2"
ami = "ami-0b41f7055516b991a"
instance_type = "t2.micro"
}
