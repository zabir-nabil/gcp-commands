# gcp-commands
commands for sshing into gcp, cheatsheet

### Create a compute instance

Create an instance with the required configurations

### Generate SSH keys

In client computer, go to git bash (Git bash because it's available easily on windows, linux, & mac so the steps are same/similar)

> command

`ssh-keygen -t rsa -C "zabiralnabil@gmail.com"`

> out

```

Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/USER/.ssh/id_rsa):
Enter passphrase (empty for no passphrase): [Only press Enter]
Enter same passphrase again: [PASSWORD]
Your identification has been saved in /c/Users/USER/.ssh/id_rsa.
Your public key has been saved in /c/Users/USER/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:xvi27oSNwwFEyOUf************* zabiral**@gmail.com
The key's randomart image is:
+---[RSA 3072]----+
| . *O== =.       |
|  o*** = o       |
|    x.+ o .      |
| .   o.= .       |
|  +...E.S        |
| +.aa+.O         |
|. o.  * =        |
|.o .. .+ .       |
|=   .o o+        |
+----[SHA256]-----+

```

Now, go to your * /c/Users/USER/.ssh/id_rsa * (Or whatever path the keys are saved in), copy the contents of your id_rsa.pub (public key) and copy it to GCP SSH keys section.

> command

`ssh-add ~/.ssh/id_rsa`

> command

`ssh username@IP`


### SSH File Transfer Protocol

#### Windows (WinSCP)

> New Session

> File Protocol: SFTP

> Credentials

> Go to Advanced > Authentication > Load Provate Key

> Login


#### Mac (Cyberduck)