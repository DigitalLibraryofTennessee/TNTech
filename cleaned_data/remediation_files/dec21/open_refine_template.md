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
{{if(isBlank(cells['dcterms.creator 1'].value), '', '<name><namePart>' + cells['dcterms.creator 1'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.creator 2'].value), '', '<name><namePart>' + cells['dcterms.creator 2'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.creator 3'].value), '', '<name><namePart>' + cells['dcterms.creator 3'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>')}}
{{if(isBlank(cells['dcterms.date'].value), '', '<originInfo><dateCreated>' + cells['dcterms.date'].value + '</dateCreated></originInfo>'))}}
{{if(isBlank(cells['dcterms.subject 1'].value), '', '<subject><topic>' + cells['dcterms.subject 1'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 2'].value), '', '<subject><topic>' + cells['dcterms.subject 2'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 3'].value), '', '<subject><topic>' + cells['dcterms.subject 3'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 4'].value), '', '<subject><topic>' + cells['dcterms.subject 4'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 5'].value), '', '<subject><topic>' + cells['dcterms.subject 5'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 6'].value), '', '<subject><topic>' + cells['dcterms.subject 6'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 7'].value), '', '<subject><topic>' + cells['dcterms.subject 7'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 8'].value), '', '<subject><topic>' + cells['dcterms.subject 8'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 9'].value), '', '<subject><topic>' + cells['dcterms.subject 9'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 10'].value), '', '<subject><topic>' + cells['dcterms.subject 10'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 11'].value), '', '<subject><topic>' + cells['dcterms.subject 11'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 12'].value), '', '<subject><topic>' + cells['dcterms.subject 12'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 13'].value), '', '<subject><topic>' + cells['dcterms.subject 13'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 14'].value), '', '<subject><topic>' + cells['dcterms.subject 14'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 15'].value), '', '<subject><topic>' + cells['dcterms.subject 15'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 16'].value), '', '<subject><topic>' + cells['dcterms.subject 16'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 17'].value), '', '<subject><topic>' + cells['dcterms.subject 17'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 18'].value), '', '<subject><topic>' + cells['dcterms.subject 18'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 19'].value), '', '<subject><topic>' + cells['dcterms.subject 19'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 20'].value), '', '<subject><topic>' + cells['dcterms.subject 20'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 21'].value), '', '<subject><topic>' + cells['dcterms.subject 21'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 22'].value), '', '<subject><topic>' + cells['dcterms.subject 22'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 23'].value), '', '<subject><topic>' + cells['dcterms.subject 23'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 24'].value), '', '<subject><topic>' + cells['dcterms.subject 24'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 25'].value), '', '<subject><topic>' + cells['dcterms.subject 25'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 26'].value), '', '<subject><topic>' + cells['dcterms.subject 26'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.subject 27'].value), '', '<subject><topic>' + cells['dcterms.subject 27'].value + '</topic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 1'].value), '', '<subject><geographic>' + cells['dcterms.spatial 1'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 2'].value), '', '<subject><geographic>' + cells['dcterms.spatial 2'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 3'].value), '', '<subject><geographic>' + cells['dcterms.spatial 3'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 4'].value), '', '<subject><geographic>' + cells['dcterms.spatial 4'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 5'].value), '', '<subject><geographic>' + cells['dcterms.spatial 5'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 6'].value), '', '<subject><geographic>' + cells['dcterms.spatial 6'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 7'].value), '', '<subject><geographic>' + cells['dcterms.spatial 7'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.spatial 8'].value), '', '<subject><geographic>' + cells['dcterms.spatial 8'].value + '</geographic></subject>')}}
{{if(isBlank(cells['dcterms.type'].value), '', '<typeOfResource>' + cells['dcterms.type'].value + '</typeOfResource>')}}
<location>
<url usage="primary" access="object in context">{{cells['URL'].value}}</url>
<url access="preview">{{cells['Thumbnail URL'].value}}</url>
</location>
{{if(isBlank(cells['language'].value), '', '<language><languageTerm authority="iso639-2b" type="text">' + cells['language'].value + '</languageTerm></language>')}}
{{if(isBlank(cells['language2'].value), '', '<language><languageTerm authority="iso639-2b" type="text">' + cells['language2'].value + '</languageTerm></language>')}}
{{if(isBlank(cells['dcterms.source'].value), '', '<relatedItem displayLabel="Collection" type="host"><titleInfo><title>' + cells['dcterms.source'].value + '</title></titleInfo></relatedItem>')}}
<recordInfo><recordContentSource>{{cells['dcterms.publisher'].value}}</recordContentSource></recordInfo>
{{if(isBlank(cells['dcterms.rightsHolder'].value), '', '<name><namePart>' + cells['dcterms.rightsHolder'].value + '</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cph">Copyright holder</roleTerm></role></name>')}}
<accessCondition type="use and reproduction" xlink:href="{{cells['dcterms.rights.uri'].value}}">{{cells['dcterms.rights'].value}}</accessCondition>
</mods>
```

## Row Separator

**LEAVE BLANK**

## Suffix

```
</modsCollection>

```