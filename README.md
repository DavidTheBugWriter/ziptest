# ziptest
Bash script to test the integrity of zip files

I use this when downloading masses of zip files. It performs two tests: zip -T and zip -F. zip -T on 
it's own is often likely to be good enough but by adding in the -F check one can be assured the zip is
99.9% likely to be good.

The script creates an intermediate dummy.zip which I don't appear to be able to prevent being created but
I delete it at the end of the script.

invocation: $testzips *.zip
output: "foobar.zip is OK" or a fail message
