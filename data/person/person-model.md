## person.tsv

### PyTransforms
#### _authorship_uri_
From column: _UID_
>``` python
return getValue("UID")+"/individual"
```

#### _email_uri_
From column: _Email_
>``` python
return "email/"+SM.sha1_hash(getValue("Email"))
```

#### _name_uri_
From column: _UID_
>``` python
return "name/"+SM.sha1_hash(getValue("UID")+getValue("FullName"))
```

#### _position_uri_
From column: _Title_
>``` python
return "postion/"+getValue("UID")+"/"+SM.fingerprint_string(getValue("Title")).lower()
```

#### _postion_start_
From column: _date_hired_
>``` python
return getValue("position_uri")+"/start"
```

#### _position_end_
From column: _date_terminated_
>``` python
return getValue("position_uri")+"/end"
```

#### _title_2_
From column: _Title_
>``` python
return getValue("Title")
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _DOI_ | `bibo:doi` | `bibo:AcademicArticle1`|
| _Email_ | `vcard:email` | `vcard:Email1`|
| _Email_ | `vcard:email` | `vcard:Email1`|
| _FirstName_ | `vcard:givenName` | `vcard:Name1`|
| _FirstName_ | `vcard:givenName` | `vcard:Name1`|
| _Full Authors_ | `vlocal:fullAuthorList` | `bibo:AcademicArticle1`|
| _FullName_ | `rdfs:label` | `vivo:FacultyMember1`|
| _FullName_ | `rdfs:label` | `vivo:FacultyMember1`|
| _ID_ | `uri` | `bibo:AcademicArticle1`|
| _ISSN_ | `bibo:issn` | `bibo:AcademicArticle1`|
| _Issue_ | `bibo:issue` | `bibo:AcademicArticle1`|
| _Journal OR Published proceedings_ | `rdfs:label` | `bibo:Journal1`|
| _LastName_ | `vcard:familyName` | `vcard:Name1`|
| _LastName_ | `vcard:familyName` | `vcard:Name1`|
| _Mesh Terms_ | `vlocal:meshTerms` | `bibo:AcademicArticle1`|
| _MidName_ | `vivo:middleName` | `vcard:Name1`|
| _MidName_ | `vivo:middleName` | `vcard:Name1`|
| _NETID_ | `vlocal:netID` | `vivo:FacultyMember1`|
| _NETID_ | `vlocal:netID` | `vivo:FacultyMember1`|
| _ORCID_ | `vivo:scopusId` | `vcard:Individual1`|
| _Pagination (end page)_ | `bibo:pageEnd` | `bibo:AcademicArticle1`|
| _Pagination (start page)_ | `bibo:pageStart` | `bibo:AcademicArticle1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:Position1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:Position1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyMember1`|
| _Title_ | `vivo:hrJobTitle` | `vivo:FacultyPosition1`|
| _Title_ | `rdfs:label` | `bibo:AcademicArticle1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _UID_ | `uri` | `vivo:FacultyMember1`|
| _Volume_ | `bibo:volume` | `bibo:AcademicArticle1`|
| _abstract_ | `bibo:abstract` | `bibo:AcademicArticle1`|
| _authorship_uri_ | `uri` | `vivo:Authorship1`|
| _authorship_uri_ | `uri` | `vcard:Individual1`|
| _date_hired_ | `vivo:dateTime` | `vivo:DateTimeValue2`|
| _date_hired_ | `vivo:hasValue` | `vivo:DateTimeValue1`|
| _date_hired_ | `vivo:hasValue` | `vivo:DateTimeValue2`|
| _date_hiredURI_ | `uri` | `vivo:DateTimeValue2`|
| _date_terminated_ | `vivo:hasValue` | `vivo:DateTimeValue2`|
| _date_terminated_ | `vivo:hasValue` | `vivo:DateTimeValue1`|
| _date_terminated_ | `vivo:dateTime` | `vivo:DateTimeValue1`|
| _date_terminatedURI_ | `uri` | `vivo:DateTimeValue1`|
| _email_uri_ | `uri` | `vcard:Email1`|
| _email_uri_ | `uri` | `vcard:Email1`|
| _journal_abbreviation_ | `vivo:abbreviation` | `bibo:Journal1`|
| _name_URI_ | `uri` | `vcard:Name1`|
| _name_uri_ | `uri` | `vcard:Name1`|
| _org_ID_ | `uri` | `vcard:Organization1`|
| _org_name_ | `rdfs:label` | `vcard:Organization1`|
| _pages_ | `bibo:numPages` | `bibo:AcademicArticle1`|
| _position_end_ | `uri` | `vivo:DateTimeValue2`|
| _position_type_ | `rdfs:label` | `vivo:Position1`|
| _position_uri_ | `uri` | `vivo:Position1`|
| _position_uri_ | `uri` | `vivo:Position1`|
| _postion_start_ | `uri` | `vivo:DateTimeValue1`|
| _pubmed_ | `bibo:pmid` | `bibo:AcademicArticle1`|
| _pubmedcentral_ | `vivo:pmcid` | `bibo:AcademicArticle1`|
| _title_2_ | `rdfs:label` | `vivo:Position1`|
| _vcard_uri_ | `uri` | `vcard:Individual1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `vcard:Individual1` | `vcard:hasEmail` | `vcard:Email1`|
| `vcard:Individual1` | `vcard:hasName` | `vcard:Name1`|
| `vivo:DateTimeValue1` | `vivo:dateTimePrecision` | `xsd:http://vivoweb.org/ontology/core#yearMonthDayPrecision`|
| `vivo:DateTimeValue2` | `vivo:dateTimePrecision` | `xsd:http://vivoweb.org/ontology/core#yearMonthDayPrecision`|
| `vivo:FacultyMember1` | `obo:ARG_2000028` | `vcard:Individual1`|
| `vivo:FacultyMember1` | `obo:RO_0000053` | `vivo:Position1`|
| `vivo:Position1` | `vivo:start` | `vivo:DateTimeValue1`|
| `vivo:Position1` | `vivo:end` | `vivo:DateTimeValue2`|
| `vivo:Position1` | `vivoext:personInPosition` | `vivo:FacultyMember1`|
