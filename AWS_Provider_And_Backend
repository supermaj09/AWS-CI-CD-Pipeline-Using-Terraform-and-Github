terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 3.0"
    }
  }
}

# Configure the AWS Provider
provider "aws" {
  region = "us-east-1"
  access_key = ""
  secret_key = ""
}

terraform {
    backend "s3" {
        enrcypt = false
        bucket = "tf-bucket-v2"
        dynamodb_table = "tf-state-lock-dynamodb"
        key = "path/path/terraform-tfstate"
        region = "us-east-1"
        
    }
}
