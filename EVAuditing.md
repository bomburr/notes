### Archive Permission Add/Remove Activities Raw SQL Result

```sql

AuditID	Status	AuditDate	UserName	CategoryName	SubCategoryName	ObjectID	Vault	info	MachineName
3644056	SUCCESS	2020-11-05 11:41:25.373	testdom\EVSA	Archive Permissions	Archive	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Archive ArchiveID="15184A893E76D5442BC3CAB95EB0519131110000evserver1" ArchiveName="AGILIS Test"><OldManualSD>D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)</OldManualSD><NewManualSD></NewManualSD></Archive>	EVSRV01
3644055	SUCCESS	2020-11-05 11:41:25.370	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Delete ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="AGILIS Test"><Property Name="RawSid"><Current Value="S-1-5-21-742064545-3663393136-722983120-1175"/></Property><Property Name="SidType"><Current Value="User"/></Property><Property Name="DomainAndAccountName"><Current Value="testdom\EVSA"/></Property><Property Name="Allow:AccessMask"><Current Value="9"/></Property><Property Name="Allow:AccessMaskText"><Current Value="ReadItem|ReadFolder"/></Property><Property Name="Allow:EffectivePermissions"><Current Value="Read"/></Property><Property Name="Deny:AccessMask"><Current Value=""/></Property><Property Name="Deny:AccessMaskText"><Current Value=""/></Property><Property Name="Deny:EffectivePermissions"><Current Value=""/></Property></Delete>	EVSRV01
3644054	SUCCESS	2020-11-05 11:41:25.367	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Update ObjectType="ArchiveView" ObjectName="AGILIS Test"><Property Name="ManualSecurityDesc"><Previous Value="D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)"/><Current Value=""/></Property></Update>	EVSRV01
3644053	SUCCESS	2020-11-05 11:27:01.863	testdom\EVSA	Archive Permissions	Archive	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Archive ArchiveID="15184A893E76D5442BC3CAB95EB0519131110000evserver1" ArchiveName="AGILIS Test"><OldManualSD></OldManualSD><NewManualSD>D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)</NewManualSD></Archive>	EVSRV01
3644052	SUCCESS	2020-11-05 11:27:01.860	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="AGILIS Test"><Property Name="RawSid"><Current Value="S-1-5-21-742064545-3663393136-722983120-1175"/></Property><Property Name="SidType"><Current Value="User"/></Property><Property Name="DomainAndAccountName"><Current Value="testdom\EVSA"/></Property><Property Name="Allow:AccessMask"><Current Value="9"/></Property><Property Name="Allow:AccessMaskText"><Current Value="ReadItem|ReadFolder"/></Property><Property Name="Allow:EffectivePermissions"><Current Value="Read"/></Property><Property Name="Deny:AccessMask"><Current Value=""/></Property><Property Name="Deny:AccessMaskText"><Current Value=""/></Property><Property Name="Deny:EffectivePermissions"><Current Value=""/></Property></Create>	EVSRV01
3644051	SUCCESS	2020-11-05 11:27:01.860	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Update ObjectType="ArchiveView" ObjectName="AGILIS Test"><Property Name="ManualSecurityDesc"><Previous Value=""/><Current Value="D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)"/></Property></Update>	EVSRV01

```


##### Read Permission add activity log 


Bir arşiv üzerinde yapılan değişikliği ilişkin log **Info  Cloumn**'ununda bulunan **XML** satırının içerisinde bulunmaktadır.

Yapılan eyleme ilişkin parametereler aşağıda listelenmiştir.

**RAW XML**
```xml

<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="AGILIS Test">
	<Property Name="RawSid">
		<Current Value="S-1-5-21-742064545-3663393136-722983120-1175"/>
	</Property>
	<Property Name="SidType">
		<Current Value="User"/>
	</Property>
	<Property Name="DomainAndAccountName">
		<Current Value="testdom\EVSA"/>
	</Property>
	<Property Name="Allow:AccessMask">
		<Current Value="9"/>
	</Property>
	<Property Name="Allow:AccessMaskText">
		<Current Value="ReadItem|ReadFolder"/>
	</Property>
	<Property Name="Allow:EffectivePermissions">
		<Current Value="Read"/>
	</Property>
	<Property Name="Deny:AccessMask">
		<Current Value=""/>
	</Property>
	<Property Name="Deny:AccessMaskText">
		<Current Value=""/>
	</Property>
	<Property Name="Deny:EffectivePermissions">
		<Current Value=""/>
	</Property>
</Create>

```




###### Action Type and Affected Object 

Herhangi bir Arşiv üzerinde değişiklik yapıldığında aşağıdaki değerler üretilecektir, **ObjectName** işlemin yapıldığı arşiv'i belirtir. 

- **Create** 
    - **ObjectType**
        -   **ArchiveView:ManualSecurityDesc**
    
    - **ObjectName**
        -   "AGILIS Test" 



```xml
<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="AGILIS Test">

```

###### Properties


Eylimi yapan kullanıcıyı tespit etmek için yakalanması gereken parametreler.
- **Property**
    - **Name**=**DomainAndAccountName**
         - **Current**
            - **Value**="testdom\EVSA"

```xml

<Property Name="DomainAndAccountName">
    <Current Value="testdom\EVSA"/>
</Property>

```

**Allow:EffectivePermissions** ne tür bir allow yetkisi verildiğine dair bilgi'yi **Current Value**'da içerir.

- **Property**
    - **Name**=**Allow:EffectivePermissions**
         - **Current**
            - **Value**="Read"

```xml

<Property Name="Allow:EffectivePermissions">
    <Current Value="Read"/>

```