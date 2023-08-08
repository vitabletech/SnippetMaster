# Release Notes - All-in-One Snippet Master Extension (Version 1.3.0)

## What's New

### Added Docker Snippets
We've added a new set of Docker-related snippets to help you manage your Docker containers more efficiently. These snippets cover various common Docker commands for container management, creating Docker images, pushing them to AWS ECR, sharing Docker images, and more.
Sure! Here are all the added shell snippets with their prefixes:

#### Docker Commands (_docker)
Description: Docker commands for container management.

Snippet:
```
docker ps -a | grep geoms
docker logs <containerid>
docker exec -it <containerid> /bin/bash
```

#### Create Docker Image from Container (_create docker image)
Description: Create a new Docker image from a running container.

Snippet:
```
docker ps
docker commit <container_id_or_name> <image_name>:<tag>
```

#### Push Docker Image to AWS ECR (_push docker image to aws ECR)
Description: Push your Docker container to AWS Container Registry (ECR).

Snippet:
```
docker tag <image_name> <aws_account_id>.dkr.ecr.<region>.amazonaws.com/<repository_name>:<tag>
docker push <aws_account_id>.dkr.ecr.<region>.amazonaws.com/<repository_name>:<tag>
```

#### Share Docker Image Locally (_share image)
Description: Share the Docker image without pushing to AWS ECR.

Snippet:
```
docker save -o <output_file.tar> <image_name>:<tag>
```

#### Load Docker Image from Local File (_load image)
Description: Import or pull the Docker image from the local system.

Snippet:
```
docker load -i <input_file.tar>
```

#### Docker Run with Your Project Name and Image (_docker_run_project)
Description: Run a Docker container with your project name and image.

Snippet:
```
docker run -it --name REPLACE_WITH_YOUR_PROJECT_NAME PASTE_YOUR_IMAGE_NAME
```

#### Docker Pull CentOS Image (_docker_pull_centos)
Description: Pull the latest CentOS image from Docker Hub.

Snippet:
```
docker pull centos
```

#### Docker Run CentOS Container (_docker_run_centos)
Description: Run an interactive CentOS container named 'mycentos'.

Snippet:
```
docker run -it --name mycentos centos
```

#### Update SSH Config (_update_ssh_config)
Description: If you are facing issues connecting via SSH in the command-line due to compatibility with older systems, you can update SSH configuration with ssh-rsa algorithms.

Snippet:
```
sudo vi /etc/ssh/ssh_config
# Add these two lines at the end
HostkeyAlgorithms +ssh-rsa
PubkeyAcceptedAlgorithms +ssh-rsa
```

#### Tail Logs (_tail logs)
Description: Tail multiple log files. This command will run `sudo tail -f` for the four specified log files, allowing you to monitor them in real-time.

Snippet:
```
sudo tail -f /var/log/messages /var/log/pictometry-logger.log /var/log/httpd/error_log /var/log/httpd/ssl_error_log
```

#### Fix SSL Certificates Issue (_fix ssl)
Description: If you are facing SSL certificates issues, this snippet will help you resolve them.

Snippet:
```
cd /etc/pki/tls/certs
sudo curl https://curl.se/ca/cacert.pem -o ca-bundle.crt -k
```

#### Enable Apache Module (_enable apache module)
Description: Enable an Apache module on your Ubuntu system using the `a2enmod` command.

Snippet:
```
sudo a2enmod TYPE_YOUR_MOUDLE_NAME
```

#### Create Symbolic Link for Apache (_apache symlink)
Description: Create a symbolic link between /etc/apache2/conf.d and /etc/apache2/sites-enabled.

Snippet:
```
sudo ln -s /etc/apache2/conf.d /etc/apache2/sites-enabled/
```

#### Mount Remote Directory in Linux (_mount_remote_directory)
Description: Mount a remote directory from a server to a local mount point in Linux.

Snippet:
```
sudo mount serverIP_OR_DOMAIN_NAME:/share/path/ /mnt/local/directory/path/
```

#### Yum List (First 10 Packages) (_yum_list)
Description: Display the first 10 packages available in the Yum package manager.

Snippet:
```
yum list | head -n 10
```

#### Disk Space Usage (_disk_space_usage)
Description: Display disk space usage of all mounted filesystems in a human-readable format.

Snippet:
```
df -h
```

#### List Block Devices (_lsblk)
Description: List information about all available block devices (disks) connected to the system.

Snippet:
```
lsblk
```

#### Resize Filesystem (_resize_filesystem)
Description: Resize the filesystem on the specified device (/dev/xvda1 in this example) after resizing the underlying partition.

Snippet:
```
sudo resize2fs /dev/xvda1
```

#### Replace Text in File with sed (_sed_replace_text)
Description: Replace 'old_text' with 'new_text' in the specified 'your_file_name' using sed.

Snippet:
```
sed -i 's/old_text/new_text/g' your_file_name
```

#### Yum Search for Python27-pip Package (_yum_search_python27-pip)
Description: Search for the 'python27-pip' package using Yum package manager.

Snippet:
```
yum search python27-pip
```

#### Install VSCE (_install_vsce)
Description: Install VS Code Extension Manager (VSCE) globally using Node.js package manager (npm).

Snippet:
```
npm install -g @vscode/vsce
```

#### Package VS Code Extension (_package_extension)
Description: Package the VS Code extension into a .vsix file for publishing.

Snippet:
```
vsce package
```

#### Publish VS Code Extension with Token (_publish_extension_token)
Description: Publish the VS Code extension to the VS Code Marketplace using a Personal Access Token (VSCE_TOKEN).

Snippet:
```
vsce publish -p VSCE_TOKEN
```
Note: Replace `VSCE_TOKEN`, `<your_file_name>`, `<image_name>:<tag>`, and `<type username>` with the appropriate values when using the snippets.


Note: Replace `TYPE_YOUR_MOUDLE_NAME`, `<container_id_or_name>`, `<image_name>`, `<aws_account_id>`, `<region>`, `<repository_name>`, `<tag>`, `<output_file.tar>`, `<input_file.tar>`, `<containerid>`, `<image_name>:<tag>`, `<source>`, `<destination>`, `<output_file.tar>`, `<input_file.tar>`, `<aws_account_id>.dkr.ecr.<region>.amazonaws.com/<repository_name>:<tag>`, `<aws_account_id>.dkr.ecr.<region>.amazonaws.com/<repository_name>:<tag>`, `<output_file.tar>`, `<input_file.tar>`, `<type username>`, `<image_name>:<tag>`, VSCE_TOKEN, <your_file_name>, <image_name>:<tag>, <type username> and `<your_file_name>` with the appropriate values when using the snippets.