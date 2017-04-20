---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
---

# New-AzureADPolicy

## SYNOPSIS
Creates a policy.

## SYNTAX

```
New-AzureADPolicy [-AlternativeIdentifier <String>]
 -Definition <System.Collections.Generic.List`1[System.String]> -DisplayName <String>
 [-IsOrganizationDefault <Boolean>]
 [-KeyCredentials <System.Collections.Generic.List`1[Microsoft.Open.MSGraph.Model.KeyCredential]>]
 -Type <String>
```

## DESCRIPTION
The New-AzureADPolicy cmdlet creates a policy in Azure Active Directory (AD).

## EXAMPLES

### Example 1: Create a policy
```
PS C:\>New-AzureADPolicy -Definition <Array of Rules> -DisplayName <Name of Policy> -IsTenantDefault
```

This command creates a new policy.

## PARAMETERS

### -AlternativeIdentifier
Specifies an alternative ID.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Definition
Specifies an array of JSON that contains all the rules of the policy, for example: -Definition @("{"TokenLifetimePolicy":{"Version":1,"MaxInactiveTime":"20:00:00"}}")

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
String of the policy name

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsOrganizationDefault
True if this policy is the organisational default

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeyCredentials
@{Text=}

```yaml
Type: System.Collections.Generic.List`1[Microsoft.Open.MSGraph.Model.KeyCredential]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
Specifies the type of policy.
For token lifetimes, specify "TokenLifetimePolicy".

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureADPolicy]()

[Remove-AzureADPolicy]()

[Set-AzureADPolicy]()
