### Archive Permission Add/Remove Activities Raw SQL Result

```sql

AuditID	Status	AuditDate	UserName	CategoryName	SubCategoryName	ObjectID	Vault	info	MachineName
3644056	SUCCESS	2020-11-05 11:41:25.373	testdom\EVSA	Archive Permissions	Archive	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Archive ArchiveID="15184A893E76D5442BC3CAB95EB0519131110000evserver1" ArchiveName="Test Mailbox"><OldManualSD>D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)</OldManualSD><NewManualSD></NewManualSD></Archive>	EVSRV01
3644055	SUCCESS	2020-11-05 11:41:25.370	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Delete ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="Test Mailbox"><Property Name="RawSid"><Current Value="S-gi1-5-21-742064545-3663393136-722983120-1175"/></Property><Property Name="SidType"><Current Value="User"/></Property><Property Name="DomainAndAccountName"><Current Value="testdom\EVSA"/></Property><Property Name="Allow:AccessMask"><Current Value="9"/></Property><Property Name="Allow:AccessMaskText"><Current Value="ReadItem|ReadFolder"/></Property><Property Name="Allow:EffectivePermissions"><Current Value="Read"/></Property><Property Name="Deny:AccessMask"><Current Value=""/></Property><Property Name="Deny:AccessMaskText"><Current Value=""/></Property><Property Name="Deny:EffectivePermissions"><Current Value=""/></Property></Delete>	EVSRV01
3644054	SUCCESS	2020-11-05 11:41:25.367	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Update ObjectType="ArchiveView" ObjectName="Test Mailbox"><Property Name="ManualSecurityDesc"><Previous Value="D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)"/><Current Value=""/></Property></Update>	EVSRV01
3644053	SUCCESS	2020-11-05 11:27:01.863	testdom\EVSA	Archive Permissions	Archive	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Archive ArchiveID="15184A893E76D5442BC3CAB95EB0519131110000evserver1" ArchiveName="Test Mailbox"><OldManualSD></OldManualSD><NewManualSD>D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)</NewManualSD></Archive>	EVSRV01
3644052	SUCCESS	2020-11-05 11:27:01.860	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="Test Mailbox"><Property Name="RawSid"><Current Value="S-1-5-21-742064545-3663393136-722983120-1175"/></Property><Property Name="SidType"><Current Value="User"/></Property><Property Name="DomainAndAccountName"><Current Value="testdom\EVSA"/></Property><Property Name="Allow:AccessMask"><Current Value="9"/></Property><Property Name="Allow:AccessMaskText"><Current Value="ReadItem|ReadFolder"/></Property><Property Name="Allow:EffectivePermissions"><Current Value="Read"/></Property><Property Name="Deny:AccessMask"><Current Value=""/></Property><Property Name="Deny:AccessMaskText"><Current Value=""/></Property><Property Name="Deny:EffectivePermissions"><Current Value=""/></Property></Create>	EVSRV01
3644051	SUCCESS	2020-11-05 11:27:01.860	testdom\EVSA	Admin Activity	ArchiveView	15184A893E76D5442BC3CAB95EB0519131110000evserver1		<Update ObjectType="ArchiveView" ObjectName="Test Mailbox"><Property Name="ManualSecurityDesc"><Previous Value=""/><Current Value="D:(A;;CCSW;;;S-1-5-21-742064545-3663393136-722983120-1175)"/></Property></Update>	EVSRV01

```


##### Read Permission add activity log 


Bir arşiv üzerinde yapılan değişikliğe ilişkin log **Info  Cloumn**'unda bulunan **XML** satırının içerisinde yer almaktadır.

Yapılan eyleme ilişkin parametereler aşağıda listelenmiştir.

**RAW XML**
```xml

<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="Test Mailbox">
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
        -   "Test Mailbox" 



```xml
<Create ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="Test Mailbox">

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

##### Read Permission delete activity log 

```xml
<Delete ObjectType="ArchiveView:ManualSecurityDesc" ObjectName="Test Mailbox">
	<Property Name="RawSid">
		<Current Value="S-gi1-5-21-742064545-3663393136-722983120-1175"/>
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
</Delete>
```


## Search Log


###### RAW SQL Log

```sql
AuditID	Status	AuditDate	UserName	CategoryName	SubCategoryName	ArchiveName	info	MachineName
3645906	SUCCESS	2020-12-10 12:00:27.993	testdom\EVSA	Search	Searches	Test Mailbox	Query 'pvid:(1F97AD858297CE6498FB95BCA277A90D51110000evserver1 OR 1AC1AAED1548A5847BA892AFF8195DF911110000evserver1 OR 1D255D1F0A8859A42BA203E04FF3C5BC51110000evserver1 OR 159F66F4AFA22424984FC14A5F769214F1110000evserver1 OR 177E90A76D133E14EB4FDFFB8CD8A24CE1110000evserver1 OR 120539E5DFB48274385B24E9CC39CB3BA1110000evserver1 OR 14F723CA9CA162B4996E06F24DC29EFFD1110000evserver1 OR 17E8ABB7A9E777242B5316CB4809B07FB1110000evserver1) AND (NOT sens:2) AND text:("TEST") AND (auth:("from@agilis.com.tr")) AND date:(2018-01-01..2020-12-16) AND (reto:("to@agilis.com.tr")) AND (recc:("cc@agilis.com.tr")) AND (recp:("all@agilis.com.tr"))', matching '0' entries, viewing range '1' to '100' GLSEV01
```



**Username** kısmında belirtilen hesap **Search** işlemini gerçekleştiren, **ArchiveName** kısmında belirtilen hesap ise Search'ün gerçekleştirildiği hesabı temsil eder. 

- **Username**
	- **ArchiveName**
		- **Search**
			- **info**
			


Yapılan Search'e ait bilgi "**info**" cloumn'unda bulunmaktadır.
	
###### info Cloumn

```sql
... AND text:("TEST") AND (auth:("from@agilis.com.tr")) AND date:(2018-01-01..2020-12-16) AND (reto:("to@agilis.com.tr")) AND (recc:("cc@agilis.com.tr")) AND (recp:("all@agilis.com.tr"))', matching '0' entries, viewing range '1' to '100' 
```

- **text**  : Yapılan aramada kullanılan kelimeleri temsil eder.
- **auth**  : From için girilen değer.
- **date**  : Aramanın tarih aralığı
- **reto**  : To kısmına girilen değer.
- **recc**  : CC kısmına girilen değer
- **recp**  : All recipient için girilen değer.
- **matching**  :  arama sonucu elde edilen item sayısını içerir.

