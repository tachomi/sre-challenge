# Site Reliability Engineering Challenge

Hi! :wave:

Welcome to Remote's SRE Interview challenge. If you've reached this step of the interview process, we have deemed you a as a good candidate for the job, let's see if you've got the technical chops to do it.

This challenge should take you less than 4 hours to complete. If you go over the 4 hours, please stop immediately and deliver as is. Your personal time is **yours** and we have no rights over it.

There is no strict set of objective criteria to evaluate this challenge, we just want to see what you are capable of. Feedback will be provided over e-mail before advancing you to the next stage.

## Expectations

1. This is a Git repository: we're expecting you to commit your changes appropriately.
    1. Smaller commits with good commit messages are always a plus.
    2. Behave as if you were going to open a Merge Request to a shared team-managed repository.

2. Write good and meaningful comments for your code. Don't comment on what is self-explanatory.

3. Don't repeat yourself. Where applicable, re-use your code.

4. A lot of the code written as part of this challenge cannot be tested adequately because that would make you incur costs. We can't possible ask you that, so for any code that interfaces with cloud APIs, write it to the best of your ability, but don't actually apply it. Your code will be reviewed for itself.

## Problem 1
Start by creating a `terraform/` subdirectory.

There, write enough Terraform code to implement the following:

- 1 Isolated VPC
- 3 Subnets, spread across 3 Availability Zones
- 1 EKS cluster
- 1 EKS Node group with 1 node

## Problem 2
Look at the `app/` subdirectory. There, you'll find a Phoenix application.

Create a Dockerfile for the application: install dependencies, compile the application and add enough configuration to be able to run the application with a `docker run app` after a `docker build -t app .`

Create a `gitlab-ci.yml` file to automate building this Dockerfile in the context of GitLab CI.

## Submission
Once you're done, tarball and gzip this Git repository into a `tar.gz` file, making sure to include the `.git` folder as well. Send the resulting file over e-mail to your recruitment contact. 
