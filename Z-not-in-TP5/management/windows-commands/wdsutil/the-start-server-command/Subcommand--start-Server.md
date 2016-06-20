---
title: Subcommand: start-Server
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 1e4343e2-0a16-4e65-8769-c09adaef5680
---
# Subcommand: start-Server
Starts all services for a Windows Deployment Services server.

## Syntax

```
WDSUTIL [Options] /Start-Server [/Server:<Server name>]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|\[\/Server:<Server name>\]|Specifies the name of the server to be started. This can be either the NetBIOS name or the fully qualified domain name \(FQDN\). If no server name is specified, the local server will be used.|

## <a name="BKMK_examples"></a>Examples
To start the server, type one of the following:

```
WDSUTIL /Start-Server
WDSUTIL /Verbose /Start-Server /Server:MyWDSServer
```

#### Additional references
[Command-Line Syntax Key](../../Command-Line-Syntax-Key.md)

[Using the disable-Server Command](Using-the-disable-Server-Command.md)

[Using the enable-Server Command](../using-the-enable-command/Using-the-enable-Server-Command.md)

[Using the get-Server Command](../using-the-get-command/Using-the-get-Server-Command.md)

[Using the Initialize-Server Command](../Using-the-Initialize-Server-Command.md)

[Subcommand: set-Server](../the-set-command/Subcommand--set-Server.md)

[Subcommand: stop-Server](../the-stop-server-command/Subcommand--stop-Server.md)

[The uninitialize-Server Option](../The-uninitialize-Server-Option.md)

