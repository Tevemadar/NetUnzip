# NetUnzip

Small JavaScript snippet to read .zip archives without downloading.

Features, restrictions:

* STORE (0) and DEFLATE (8) methods are supported
* no encryption
* comment and extra fields are supported for files and directory entries
* comment is not supported for the .zip archive itself as it shifts the positions inside the file
* the location of the .zip archive can be simple text or an ```async``` function (this is for supporting tempurls).

Links for the live example page:

* [https://tevemadar.github.io/NetUnzip](https://tevemadar.github.io/NetUnzip) - large demo with a 852 MB archive hosted on HumanBrainProject. It's a DeepZoom Image pyramid contained in a single archive, 8481 entries. The demo downloads 701 kilobytes of data for listing the files, but building the table with that many lines may take a significant amount of time (10-second range)
* [https://tevemadar.github.io/NetUnzip?testcomp.zip](https://tevemadar.github.io/NetUnzip?testcomp.zip) - small demo with the compressed .zip archive provided right here
* [https://tevemadar.github.io/NetUnzip?testuncomp.zip](https://tevemadar.github.io/NetUnzip?testuncomp.zip) - small demo with the uncompressed .zip archive provided right here.

