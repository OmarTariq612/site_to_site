`FOO_PRIVATE_KEY` -> The private key of `foo`.

`VPS_PUBLIC_KEY` -> The public key of the VPS.

`VPS_PUBLIC_IP` -> The public IP address of the VPS.

**Replace `192.168.1.0/24` with `site b` network address in your situation.**

**If `foo` is a windows machine then comment out `PreUp` and  `PostDown` lines, those lines enable IP forwarding on linux machines, on windows you can enable `RemoteAccess` service and start it using this command on powershell (with administrator privileges):**

```
Set-Service -Name RemoteAccess -StartupType Manual -Status Running
```