# Example module to build a and EC2 cluster of nodes.

```
  
provider "aws" {
  region = "eu-west-1"
}


module "Webserver" {
  source = "./modules/service/webserver-cluster"
  cluster_name = foo
  min_size     = 1
  max_size     = 5
  instance_type = "t2.micro"

}
``` 
