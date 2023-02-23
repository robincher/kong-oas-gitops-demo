# gitops-demo

This repository provides a template for doing your own demonstration of the end to end lifecycle as depicted in the following diagram.

## Setup
1. First time only - modify the `Environment` Insomnia needs to launch the cluster since the endpoint is protected with OpenID. 
    * Modify the environment variables by pressing `COMMAND-E` to get to the environment variables screen. Follow the screenshots below to:
      1. Copy the Development Environment
      2. Create a **Private** sub environment. 
      3. Enter your Kong Okta credentials into the private sub environment kong_username and kong_password variables.

      ![Development](https://user-images.githubusercontent.com/11033758/126689412-fa6c2fc6-d82a-4127-9bbe-8d329b0e41aa.png)
      
      ![Private](https://user-images.githubusercontent.com/11033758/126690075-7d0696a0-98cb-4773-ba08-371f8c79c9e5.png)
2. **Each time you create an environment** - updated the *host* and *admin_api_host* variables in **both** the "Development" and "Private" environments.
3. **Each time you create an environment** - in the **Blog** Insomnia Design Document, click "Setup Git Sync" to configure with the URL to this git repo and your credentials
