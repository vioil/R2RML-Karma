## person.csv

### PyTransforms
#### _vcard_uri_
From column: _UID_
>``` python
return getValue("UID")+"/vcard"
```

#### _email_uri_
From column: _Email_
>``` python
return "email/"+UM.urlencode(getValue("Email"))
```

#### _start_uri_
From column: _vcard_uri_
>``` python
return getValue("UID")+"/start"
```

#### _end_uri_
From column: _vcard_uri_
>``` python
return getValue("UID")+"/end"
```

#### _name_uri_
From column: _start_uri_
>``` python
return getValue("UID")+"/name"
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Email_ | `vcard:email` | `vcard:Email1`|
| _Email_ | `vcard:email` | `vcard:Email1`|
| _FirstName_ | `vcard:givenName` | `vcard:Name1`|
| _FirstName_ | `vcard:givenName` | `vcard:Name1`|
| _FullName_ | `rdfs:label` | `vivo:FacultyMember1`|
| _FullName_ | `rdfs:label` | `vivo:FacultyMember1`|
| _LastName_ | `vcard:familyName` | `vcard:Name1`|
| _LastName_ | `vcard:familyName` | `vcard:Name1`|
| _MidName_ | `vivo:middleName` | `vcard:Name1`|
| _MidName_ | `vivo:middleName` | `vcard:Name1`|
| _ORCID_ | `vivo:scopusId` | `vcard:Individual1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyMember1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyMember1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _date_hired_ | `vivo:dateTime` | `vivo:DateTimeValue2`|
| _date_hired_ | `vivo:hasValue` | `vivo:DateTimeValue1`|
| _date_hiredURI_ | `uri` | `vivo:DateTimeValue2`|
| _date_terminated_ | `vivo:dateTime` | `vivo:DateTimeValue1`|
| _date_terminated_ | `vivo:hasValue` | `vivo:DateTimeValue2`|
| _date_terminatedURI_ | `uri` | `vivo:DateTimeValue1`|
| _email_uri_ | `uri` | `vcard:Email1`|
| _email_uri_ | `uri` | `vcard:Email1`|
| _end_uri_ | `uri` | `vivo:DateTimeValue2`|
| _name_URI_ | `uri` | `vcard:Name1`|
| _name_uri_ | `uri` | `vcard:Name1`|
| _start_uri_ | `uri` | `vivo:DateTimeValue1`|
| _vcard_uri_ | `uri` | `vcard:Individual1`|
| _vcard_uri_ | `uri` | `vcard:Individual1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `vcard:Individual1` | `vcard:hasEmail` | `vcard:Email1`|
| `vcard:Individual1` | `vcard:hasName` | `vcard:Name1`|
| `vivo:DateTimeValue1` | `vivo:dateTimePrecision` | `xsd:http://vivoweb.org/ontology/core#yearMonthDayPrecision`|
| `vivo:DateTimeValue2` | `vivo:dateTimePrecision` | `xsd:http://vivoweb.org/ontology/core#yearMonthDayPrecision`|
| `vivo:FacultyMember1` | `vivo:start` | `vivo:DateTimeValue1`|
| `vivo:FacultyMember1` | `vivo:end` | `vivo:DateTimeValue2`|
| `vivo:FacultyMember1` | `obo:ARG_2000028` | `vcard:Individual1`|
