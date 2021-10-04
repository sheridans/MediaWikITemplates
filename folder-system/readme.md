# Mediawiki Folder System

Mediawiki templates related to Providing a Folder System in Mediawiki talk at EMWCon by Rich Evans.

Link to YouTube Video:
https://www.youtube.com/watch?v=QYeBM2Mwyto

## Notes
### Update 1:
One of the extensions missing is "mediawiki/header-footer" to enable the header/footer functionality giving access to the "MediaWiki:Hf-nsheader-" pages. I also had to find the SimpleBatchUpload Modification which can be done by replacing the content of "extensions/SimpleBatchUpload/res/ext.SimpleBatchUpload.js" with https://raw.githubusercontent.com/ankostis/SimpleBatchUpload/rename-files/res/ext.SimpleBatchUpload.js.

### Update 2:
It's almost working other than the replace function doesn't seem to be working for whatever reason atm with link showing "[[:{{#replace:File:SCL61-test.txt|File:|Media:}}|{{#replace:File:SCL61-test.txt|File:|}}]]"

### Update 3:
In LocalSettings.php you also need to add the line "$wgPFEnableStringFunctions = true;" which has sorted the issues with the parser string functions not working.
