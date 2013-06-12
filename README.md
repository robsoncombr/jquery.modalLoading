jquery.modalLoading
===================

Copyright (c) 2013 Robson Martins Licensed under the MIT license (http://www.opensource.org/licenses/mit-license.php)

modalLoading jQuery Plugin creates a Loading screen over your page and it allows you to choose the holder container, so you can append the Modal Loading to the document.body ('body') or to a <div> object, see examples below:

Needed includes:

	<script src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
	<script type="text/javascript" src="modalLoading.js"></script>

Simple usage:

To create:
	
	loading = $(selector).modalLoading(height);
	
To Remove:
	
	loading.remove();
 
Examples:

	loading = $(document.body).modalLoading(100);
	loading.remove();

	$('#div-name').modalLoading(100);
	loading.remove();

	$('#div-name').modalLoading();
	loading.remove();

	$(document.body).modalLoading(100, 'New Message...');
	loading.remove();

	$('#div-name').modalLoading(0, 'New Message...');
	loading.remove();

Notes:
- valid height value from 0 to 100, it represents the % of the holder container
- if no height is provided, it will assume the height of its holder container
