## positions.csv

### PyTransforms
#### _position_uri_
From column: _UID_
>``` python
return "position/"+getValue("UID")+"_"+getValue("org_ID")+"_"+getValue("position_type").replace(" ","_")
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Email_ | `vcard:email` | `vcard:Email1`|
| _FirstName_ | `vcard:givenName` | `vcard:Name1`|
| _FullName_ | `rdfs:label` | `vivo:FacultyMember1`|
| _LastName_ | `vcard:familyName` | `vcard:Name1`|
| _MidName_ | `vivo:middleName` | `vcard:Name1`|
| _ORCID_ | `vivo:scopusId` | `vcard:Individual1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyMember1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyPosition1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _date_hired_ | `vivo:dateTime` | `vivo:DateTimeValue2`|
| _date_hired_ | `vivo:hasValue` | `vivo:DateTimeValue2`|
| _date_hiredURI_ | `uri` | `vivo:DateTimeValue2`|
| _date_terminated_ | `vivo:dateTime` | `vivo:DateTimeValue1`|
| _date_terminated_ | `vivo:hasValue` | `vivo:DateTimeValue1`|
| _date_terminatedURI_ | `uri` | `vivo:DateTimeValue1`|
| _email_uri_ | `uri` | `vcard:Email1`|
| _job_title_ | `vivo:hrJobTitle` | `vivo:FacultyMember1`|
| _name_URI_ | `uri` | `vcard:Name1`|
| _org_ID_ | `uri` | `vcard:Organization1`|
| _org_name_ | `rdfs:label` | `vcard:Organization1`|
| _position_type_ | `rdfs:label` | `vivo:Position1`|
| _position_uri_ | `uri` | `vivo:Position1`|
| _vcard_uri_ | `uri` | `vcard:Individual1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `vivo:Position1` | `vivo:relates` | `vivo:FacultyMember1`|
| `vivo:Position1` | `vivo:relates` | `vcard:Organization1`|
