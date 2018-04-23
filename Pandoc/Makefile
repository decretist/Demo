all:	humc394.docx dhcolloq.docx

humc394.docx:	humc394.md
	pandoc -o humc394.docx --filter pandoc-citeproc --reference-doc=myref.docx humc394.md

dhcolloq.docx:	dhcolloq.md
	pandoc -o dhcolloq.docx --filter pandoc-citeproc --reference-doc=myref.docx dhcolloq.md

myref.docx:
	pandoc --print-default-data-file reference.docx > myref.docx

clean:
	rm -i humc394.docx dhcolloq.docx
