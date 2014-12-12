ServeCS
=======

Windows Service Template, easy to debug

## V 0.1

Template base projects created; a single file _Servo.cs_, which is the Windows Service scaffold.

Currently, for using this we just need add:

```
  <appSettings>
    <add key="WinSvc/Conf/ServiceName" value="SampleService" />
    <add key="WinSvc/Conf/DisplayName" value="Sample Service" />
    <!-- System.ServiceProcess.ServiceStartMode -->
    <add key="WinSvc/Conf/ServiceStartMode" value="Automatic" />
    <add key="WinSvc/Conf/Description" value="Sample Service" />
    <!-- csv -->
    <add key="WinSvc/Conf/ServicesDependedOn" value=",," />
    <!-- bool -->
    <add key="WinSvc/Conf/DelayedAutoStart" value="true" />
  </appSettings>
```

To _App.Config_ and necessary assemblies.

_NLog_ is used for logging as a NuGet.
### TODO:

Create Visual Studio Project Template