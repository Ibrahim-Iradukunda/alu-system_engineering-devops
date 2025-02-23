# SSH Project

## Requirements

### General

- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted on Ubuntu 20.04 LTS
- All files should end with a new line
- A `README.md` file at the root of the project folder is mandatory
- All Bash script files must be executable
- The first line of all Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all Bash scripts should be a comment explaining what the script does

### Your Servers

| Name        | Username | IP  | State |
| ----------- | -------- | --- | ----- |
| 6381-web-01 | ubuntu   | TBD | TBD   |

## Tasks

### 0. Use a private key

**File:** `0-use_a_private_key`

Write a Bash script that uses `ssh` to connect to your server using the private key `~/.ssh/school` with the user `ubuntu`.

#### Requirements:

- Only use `ssh` single-character flags
- Do not use `-l`
- Do not handle private key passphrase cases

#### Example:

```sh
sylvain@ubuntu$ ./0-use_a_private_key
ubuntu@server01:~$ exit
Connection to 8.8.8.8 closed.
sylvain@ubuntu$
```

---

### 1. Create an SSH key pair

**File:** `1-create_ssh_key_pair`

Write a Bash script that creates an RSA key pair.

#### Requirements:

- Name the private key `school`
- Create a 4096-bit key
- Protect the key with the passphrase `betty`

#### Example:

```sh
sylvain@ubuntu$ ./1-create_ssh_key_pair
Generating public/private rsa key pair.
Your identification has been saved in school.
Your public key has been saved in school.pub.
```

---

### 2. Client configuration file

**File:** `2-ssh_config`

Configure the SSH client to connect without typing a password.

#### Requirements:

- Use the private key `~/.ssh/school`
- Refuse password authentication

#### Example:

```sh
sylvain@ubuntu$ ssh -v ubuntu@98.98.98.98
...
Authentication succeeded (publickey).
Authenticated to 98.98.98.98 ([98.98.98.98]:22).
```

---

### 3. Let me in!

Add the SSH public key below to your server to allow access using the `ubuntu` user.

**Public Key:**

```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDNdtrNGtTXe5Tp1EJQop8mOSAuRGLjJ6DW4PqX4wId/Kawz35ESampIqHSOTJmbQ8UlxdJuk0gAXKk3Ncle4safGYqM/VeDK3LN5iAJxf4kcaxNtS3eVxWBE5iF3FbIjOqwxw5Lf5sRa5yXxA8HfWidhbIG5TqKL922hPgsCGABIrXRlfZYeC0FEuPWdr6smOElSVvIXthRWp9cr685KdCI+COxlj1RdVsvIo+zunmLACF9PYdjB2s96Fn0ocD3c5SGLvDOFCyvDojSAOyE70ebIElnskKsDTGwfT4P6jh9OBzTyQEIS2jOaE5RQq4IB4DsMhvbjDSQrP0MdCLgwkN
```

---

## Repository Structure

- **GitHub Repository:** `alu-system_engineering-devops`
- **Directory:** `ssh`
- **Files:**
  - `0-use_a_private_key`
  - `1-create_ssh_key_pair`
  - `2-ssh_config`

---

