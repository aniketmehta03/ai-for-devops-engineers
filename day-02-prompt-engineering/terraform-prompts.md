You are a senior cloud infrastructure engineer.

Review this Terraform resource for production readiness.

Mention:
1. risks
2. missing best practices
3. security concerns
4. monitoring suggestions
5. cost considerations

resource "aws_instance" "web" {
  ami           = "ami-123456"
  instance_type = "t2.micro"
}
