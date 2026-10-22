**SSH, or Secure Shell, is a protocol which allows users to access headless[^1] computers remotely. At TRC, it is used to access certain computers in order to troubleshoot issues, as well as to send new video files to the [[VideoPi]] in the lobby. 

In order to access a computer on the network, ==you need to know the IP address for that computer==. In Nextcloud, under Staff, there is a file which should have up-to-date static IPs for all the computers[^2]. ***Only those with Staff-level access will be able to get this file.***

# Remoting into a computer using SSH

On a computer which is connected to the TRC network, open a Terminal window and type the following command:
```bash
ssh [computer's name]@[computer's ip address]
```
replacing [computer's name] with the name of the computer and [computer's ip address] with the ip address of the computer, both accessible in the previously mentioned device list.

The first time you log in to a computer from your device, it will ask you to confirm the fingerprint. This is an SSH security measure. You can type yes and hit enter to move past this.

It will then ask you for the password for the user you specified. This information is also stored in the previously mentioned device list.

You should now be in the computer, and can use terminal commands to fix issues that should arise. Each service has its own terminal commands which are needed in order to fix them if they go down.

# Sending Files Using SCP

[^1]: Headless, or a computer without a heads-up display (desktop) and, especially a connected monitor

[^2]: Need to make this file
