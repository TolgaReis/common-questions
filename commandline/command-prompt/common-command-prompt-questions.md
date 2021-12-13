# Common Command Prompt Questions

## How do I kill the process currently using a port in Windows?

Open up cmd.exe as an administrator, then run the below command:

```
netstat -ano | findstr :<PORT>
```

Replace <PORT> with the port number you want.

As a result of the command executed, the rightmost column represents the PID number. Then, run the following command:

```
taskkill /PID <PID> /F
```

You can check whether the operation succeeded or not by re-running the first command. 