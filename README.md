# Let's Play with Terraform

Ensure that your system is up to date and you have installed the `gnupg`, `software-properties-common`, and `curl` packages installed.

```text
sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl
```

```text
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
```

```text
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
```

```text
sudo apt-get update && sudo apt-get install terraform
```

Verify that the installation:

```text
terraform -help
```
