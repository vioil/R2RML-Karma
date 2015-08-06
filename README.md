R2RML-Karma
===========

R2RML models for modeling tabular data into semantic web VIVO compliant data. There are R2RML models for modeling person, organization, position and publication data sets. Some examples are shown below:

**person.txt can be used with a CSV or TSV file that has the following columns**

UID  ||	NETID	||	FullName	|| FirstName ||	LastName ||	MidName	|| Email ||	date_hired ||	date_terminated ||	Title ||

Where:

1. UID	is the ID of the person

**positions.txt can be used with a CSV or TSV file that has the following columns**

UID ||	job_title ||	position_type	|| org_name	|| org_ID ||



**aarticles.txt can be used with a CSV or TSV file that has the following columns**

ID ||	uuid||	Title	|| Journal OR Published proceedings ||	journal_abbreviation ||	Publication Date1 ||	year ||	Volume ||	Issue ||	pages ||	DOI	|| ISSN || isbn ||	pubmed ||	pubmedcentral ||	abstract

Where:

1. ID	is the ID of the article
2. uuid	is the ID of the person
3. Title is the title of the article
4. Journal OR Published proceedings	is the title of the journal
5. journal_abbreviation	is the journal abbriviated title
6. Publication Date1	is the publication date of the article
7. year is the year of publication
8. Volume	is the volume number of the journal
9. Issue is the issue number of the journal
10. pages	is the number of the pages
11. Pagination (start page)
12. Pagination (end page)
13. DOI is the article unique identifier
14. ISSN	is the journal unique identifier 
15. isbn	
16. pubmed	is the Pubmed ID of the journal article
17. pubmedcentral	is the PubMedCentral ID of the journal article
18. abstract is the abstract of the article



**R2RMLAABook.txt can be used with a CSV or Tab separated file that has the following columns**

BookId ||	ISBN ||	BookTitle	|| AuthorName	|| PublishDate ||	InstitutionFacultyId

Where:

1. BookID - is the book unique identifier
2. ISBN 
3. BookTitle - is the title of the book
4. AuthorName
5. PublishDate - is the date of publications
6. InstitutionFacultyId is in fact our local unique identifier for a person 


**R2RMLBookCh.txt can be used with a CSV or TSV file that has the following columns**

BookChapterId	|| Title ||	Author ||	Editor ||	ISBN ||	PublishDate ||	PublishYear	|| PersonName ||	URI	|\ ChapterTitle

Where:

1. BookChapterID - is the chapter unique identifier
2. Title - the title of the Book
3. Author
4. ISBN
5. Publish Year
6. PersonName
7. URI - the unique identifier for the person
8. ChapterTitle - title of the book chapter




