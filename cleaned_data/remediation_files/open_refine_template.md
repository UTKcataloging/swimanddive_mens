# Open Refine Template for Men's Swimming and Diving Guides


## Template

#### Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```
####Body

```
<mods>
<identifier type="local">{{cells["adminDB"].value}}</identifier> 
{{if(isBlank(cells["title"].value),'', '<titleInfo><title>' + cells['title'].value + '</title></titleInfo>')}}
<titleInfo supplied="yes"><title>{{cells['title_supplied'].value}}</title></titleInfo>
<originInfo><dateIssued>{{cells['date_text'].value}}</dateIssued>
<dateIssued encoding="edtf" keyDate="yes">{{cells['date_text'].value}}</dateIssued>
<publisher>University of Tennessee, Knoxville. Department of Athletics</publisher>
</originInfo>
<physicalDescription><extent>{{cells['extent'].value}}</extent><form authority="aat" valueURI="{{cells['form_URI'].value}}">{{cells['form'].value}}</form><internetMediaType>image/jp2</internetMediaType><digitalOrigin>reformatted digital</digitalOrigin></physicalDescription>
<subject><name authority="naf" valueURI="http://id.loc.gov/authorities/names/no2018031459"><namePart>Tennessee Volunteers (Swimming and diving team)</namePart></name></subject>
<subject><name><namePart>{{cells['subject_name'].value}}</namePart></name></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh85131207"><topic>Swimming</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh85038594"><topic>Diving</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh85028338"><topic>College sports</topic></subject>
<subject authority="naf" valueURI="http://id.loc.gov/authorities/names/n79109786"><geographic>Knoxville (Tenn.)</geographic><cartographics><coordinates>35.96064, -83.92074</coordinates></cartographics></subject>
<language><languageTerm type="text" authority="iso639-2b">English</languageTerm></language>
<typeOfResource>text</typeOfResource>
<typeOfResource>still image</typeOfResource>
<relatedItem displayLabel="Project" type="host"><titleInfo><title>University of Tennessee Men's Swimming-Diving Media Guides</title></titleInfo></relatedItem>
<location><physicalLocation valueURI="http://id.loc.gov/authorities/names/no2014027633">University of Tennessee, Knoxville. Special Collections</physicalLocation></location>
<recordInfo><recordContentSource valueURI="http://id.loc.gov/authorities/names/n87808088">University of Tennessee, Knoxville. Libraries</recordContentSource><languageOfCataloging><languageTerm type="text" authority="iso639-2b">English</languageTerm></languageOfCataloging><recordOrigin>
Created and edited in general conformance to MODS Guidelines (Version 3.5).
</recordOrigin></recordInfo>
<accessCondition type="use and reproduction" xlink:href="{{cells['rights_URI'].value}}">{{cells['rights'].value}}</accessCondition>
</mods>

```

#### Suffix

```
</modsCollection>
```