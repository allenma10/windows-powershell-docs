---
ms.mktglfcycl: manage
ms.sitesec: library
ms.author: brianlic
author: brianlic-msft
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.IdentityServer.Management.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 12/20/2016
ms.prod: w10
ms.technology: powershell-windows
ms.topic: reference
online version: 
schema: 2.0.0
title: Disable-AdfsLocalClaimsProviderTrust
ms.assetid: 37F17A5A-0C10-4021-A8F8-C5D7CC6DBB5D
---

# Disable-AdfsLocalClaimsProviderTrust

## SYNOPSIS
Disables a local claims provider trust.

## SYNTAX

### IdentifierObject
```
Disable-AdfsLocalClaimsProviderTrust -TargetClaimsProviderTrust <LocalClaimsProviderTrust> [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Identifier
```
Disable-AdfsLocalClaimsProviderTrust -TargetIdentifier <String> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### IdentifierName
```
Disable-AdfsLocalClaimsProviderTrust -TargetName <String> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Disable-AdfsLocalClaimsProviderTrust** cmdlet disables a local claims provider trust.

## EXAMPLES

### Example 1: Disable a local claims provider trust
```
PS C:\> Disable-AdfsLocalClaimsProviderTrust -TargetName "testldap"
```

This command disables a local claims provider trust named testldap.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetClaimsProviderTrust
Specifies the local claims provider trust to disable.
To obtain a **LocalClaimsProviderTrust** object, use the **Get-AdfsLocalClaimsProviderTrust** cmdlet.

```yaml
Type: LocalClaimsProviderTrust
Parameter Sets: IdentifierObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TargetIdentifier
Specifies the ID of the local claims provider trust to disable.

```yaml
Type: String
Parameter Sets: Identifier
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TargetName
Specifies the name of the local claims provider trust to disable.

```yaml
Type: String
Parameter Sets: IdentifierName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AdfsLocalClaimsProviderTrust](./Add-AdfsLocalClaimsProviderTrust.md)

[Enable-AdfsLocalClaimsProviderTrust](./Enable-AdfsLocalClaimsProviderTrust.md)

[Get-AdfsLocalClaimsProviderTrust](./Get-AdfsLocalClaimsProviderTrust.md)

[Remove-AdfsLocalClaimsProviderTrust](./Remove-AdfsLocalClaimsProviderTrust.md)

[Set-AdfsLocalClaimsProviderTrust](./Set-AdfsLocalClaimsProviderTrust.md)
