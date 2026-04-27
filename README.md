I dont want to maintain a commit history and I use github to serve my resume to my website.

I use this command - git checkout --orphan temp_branch && git add -A && git commit -m "Initial commit" && git branch -D main && git branch -m main && git push -f origin main

Convert resume markdown to docx using pandoc with reference template (renders bullets correctly in Word):

pandoc -o reference.docx --print-default-data-file reference.docx && pandoc "Kshitij Desai - Resume.md" --reference-doc=reference.docx -o "Kshitij Desai - Resume.docx"