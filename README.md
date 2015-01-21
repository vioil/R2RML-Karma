R2RML-Karma
===========

R2RML models for modeling tabular data into semantic web VIVO compliant data

R2RML-articlesAANEW.txt can be used with a CSV or Tab separated file that has the following columns:

ID ||	Title	|| Journal OR Published proceedings	|| Publication date	|| Volume	|| Issue ||	Pagination (start page)	|| Pagination (end page)	|| DOI	|| PersonName	|| URI ||	ISSN ||	eISSN			

Where:

1. ID - is the article ID
2. Title - is the journal article title
3. Journal OR Published proceedings - is the title of the Journal OR Published proceedings
4. Publication date - is the date of pubications
5. Volume
6. Issue - is the issue number
7. Pagination (start page)
8. Pagination (end page)
9. DOI
10. URI - is in fact our local unique identifier for a person 
11. ISSN
12. eISSN


R2RMLAABook.txt can be used with a CSV or Tab separated file that has the following columns:

BookId ||	ISBN ||	BookTitle	|| AuthorName	|| PublishDate ||	InstitutionFacultyId

Where:

1. BookID - is the book unique identifier
2. ISBN 
3. BookTitle - is the title of the book
4. AuthorName
5. PublishDate - is the date of publications
6. InstitutionFacultyId is in fact our local unique identifier for a person 


R2RMLBookCh.txt can be used with a CSV or TSV file that has the following columns:

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

Edit on January 21st 2015:
Pubsdate.ttl.txt can be used with a CSV or TSv file that has the following columns:

ID ||	uuid||	Title	|| Journal OR Published proceedings ||	journal_abbreviation ||	Publication Date1 ||	Volume ||	Issue ||	pages ||	DOI	|| ISSN || isbn ||	pubmed ||	pubmedcentral ||	abstract

Where:

1. ID	is the ID of the article
2. uuid	is the ID of the person
3. Title is the title of the article
4. Journal OR Published proceedings	is the title of the journal
5. journal_abbreviation	is the journal abbriviated title
6. Publication Date1	is the publication date of the article
7. Volume	is the volume number of the journal
8. Issue is the issue number of the journal
9. pages	is the number of the pages
10. DOI is the article unique identifier
11. ISSN	is the journal unique identifier 
12. isbn	
13. pubmed	is the Pubmed ID of the journal article
14. pubmedcentral	is the PubMedCentral ID of the journal article
15. abstract is the abstract of the article


