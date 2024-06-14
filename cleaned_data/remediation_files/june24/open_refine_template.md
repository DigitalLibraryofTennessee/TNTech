# OpenRefine Template for Tennessee Tech DPLA Ingest

---

## Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```

## Row Template

```
<mods>
{{if(isBlank(cells['dcterms.identifier'].value), '', '<identifier type="local">' + cells['dcterms.identifier'].value + '</identifier>')}}
{{if(isBlank(cells["dcterms.title"].value), '', '<titleInfo><title>' + cells["dcterms.title"].value + '</title></titleInfo>')}}
{{if(isBlank(cells["dcterms.description"].value),'', '<abstract>' + cells['dcterms.description'].value + '</abstract>')}}
{{if(isBlank(cells['dcterms.date'].value), '', '<originInfo><dateCreated>' + cells['dcterms.date'].value + '</dateCreated></originInfo>')}}
{{if(isBlank(cells['dcterms.creator 1'].value), '', '<name><namePart>' + cells['dcterms.creator 1'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.creator 2'].value), '', '<name><namePart>' + cells['dcterms.creator 2'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.rightsHolder'].value), '', '<name><namePart>' + cells['dcterms.rightsHolder'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cph">Copyright holder</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.date'].value), '', '<originInfo><dateCreated>' + cells['dcterms.date'].value + '</dateCreated></originInfo>'))}}
{{if(isBlank(cells['dcterms.subject 1'].value), '', '<subject><topic>' + cells['dcterms.subject 1'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 2'].value), '', '<subject><topic>' + cells['dcterms.subject 2'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 3'].value), '', '<subject><topic>' + cells['dcterms.subject 3'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 4'].value), '', '<subject><topic>' + cells['dcterms.subject 4'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 5'].value), '', '<subject><topic>' + cells['dcterms.subject 5'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 6'].value), '', '<subject><topic>' + cells['dcterms.subject 6'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 7'].value), '', '<subject><topic>' + cells['dcterms.subject 7'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 1'].value), '', '<subject><geographic>' + cells['dcterms.spatial 1'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 2'].value), '', '<subject><geographic>' + cells['dcterms.spatial 2'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.type'].value), '', '<typeOfResource>' + cells['dcterms.type'].value + '</typeOfResource>')}}
{{if(isBlank(cells['dcterms.type.2'].value), '', '<typeOfResource>' + cells['dcterms.type.2'].value + '</typeOfResource>')}}
<location>
<url usage="primary" access="object in context">{{cells['URL'].value}}</url>
<url access="preview">{{cells['Thumbnail URL'].value}}</url>
</location>
{{if(isBlank(cells['dcterms.source'].value), '', '<relatedItem displayLabel="Collection" type="host"><titleInfo><title>' + cells['dcterms.source'].value + '</title></titleInfo></relatedItem>')}}
<recordInfo><recordContentSource>{{cells['dcterms.publisher'].value}}</recordContentSource></recordInfo>
<language>
<languageTerm authority="iso639-2b" type="text">{{cells['dcterms.language'].value}}</languageTerm>
</language>
{{if(isBlank(cells['dcterms.rightsHolder'].value), '', '<name><namePart>' + cells['dcterms.rightsHolder'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cph">Copyright holder</roleTerm></role></name>')}}
<accessCondition type="use and reproduction" xlink:href="{{cells['dcterms.accessRights'].value}}">{{cells['dcterms.rights'].value}}</accessCondition>
</mods>
```

## Row Separator

**LEAVE BLANK**

## Suffix

```
</modsCollection>

```