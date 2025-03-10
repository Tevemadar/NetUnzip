# NetUnzip

Small JavaScript snippet to read .zip archives without downloading.

Features, restrictions:

* STORE (0) and DEFLATE (8) methods are supported
* no encryption
* comment and extra fields are supported for files and directory entries
* comment is not supported for the .zip archive itself as it shifts the positions inside the file
* the location of the .zip archive can be simple text or an ```async``` function (this is for supporting tempurls).

Links for the live example page:

* [https://tevemadar.github.io/NetUnzip](https://tevemadar.github.io/NetUnzip) - large, 852 MB archive hosted on EBRAINS. It's a DeepZoom Image pyramid contained in a single archive, 8481 entries. The demo downloads 701 kilobytes of data for listing the files, and shows a truncated list only
* [https://tevemadar.github.io/NetUnzip?testcomp.zip](https://tevemadar.github.io/NetUnzip?testcomp.zip) - small demo with the compressed .zip archive provided right here
* [https://tevemadar.github.io/NetUnzip?testuncomp.zip](https://tevemadar.github.io/NetUnzip?testuncomp.zip) - small demo with the uncompressed .zip archive provided right here.
* [https://tevemadar.github.io/NetUnzip?https://data-proxy.ebrains.eu/api/v1/buckets/map-online-quint-test-sept-22/.nesysWorkflowFiles/zippedPyramids/BigTiff_test/Kanin_F6_105_42_s2.dzip](https://tevemadar.github.io/NetUnzip?https://data-proxy.ebrains.eu/api/v1/buckets/map-online-quint-test-sept-22/.nesysWorkflowFiles/zippedPyramids/BigTiff_test/Kanin_F6_105_42_s2.dzip) - huge 35 GB archive (Zip64) hosted on EBRAINS. It's also a DeepZoom Image pyramid, but it contains 275000+ files. While only a truncated list is displayed, getting the Zip directory means downloading 32 MB of data

