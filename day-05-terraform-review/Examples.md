You are a Senior Cloud Infrastructure Engineer.

Review this Terraform configuration.
resource "aws_instance" "web" {
  ami           = "ami-123456"
  instance_type = "t2.micro"
}
 

Analyze:

1. Security Risks
2. Cost Risks
3. Reliability Concerns
4. Observability Gaps
5. Best Practice Improvements

Provide:
- Severity
- Recommendation
- Verification Method



Improved Example:

resource "aws_instance" "web" {
  ami           = var.ami_id
  instance_type = "t3.micro"

  iam_instance_profile = aws_iam_instance_profile.ec2_profile.name

  vpc_security_group_ids = [
    aws_security_group.web.id
  ]

  monitoring = true

  metadata_options {
    http_tokens = "required"
  }

  root_block_device {
    encrypted = true
  }

  tags = {
    Name        = "web-server"
    Environment = "dev"
    Owner       = "platform-team"
    ManagedBy   = "Terraform"
  }
}
