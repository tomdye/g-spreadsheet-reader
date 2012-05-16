g-spreadsheet-reader
====================

google spreadsheet reader amd module for dojo 1.7+

Require the module with Dojo 1.7+ amd require.
Need to set your spreadsheet as shared and then 'publish to the web'.

The spreadsheet key is given when you share it.

use as follows:

require(["um/GSpreadsheetIO"], function (gSpreadsheetIO) {

  gSpreadsheetIO.setKey( /* spreadsheet key */ );
  gSpreadsheetIO.setPage( /* sheet number */ );
  
  gSpreadsheetIO.fetch().then(function(results) {
      /* Loop though the results and do what you want! */
      /* results is a json array of rows from your spreadsheet using the headings from the spreadsheet */
	});
  
});

Enjoy!