# blog
no frills blog framework using markdown to generate html

# requirements
* apache2 with apache-mod-markdown configured to display index.md files by default
```/etc/apache2/mods-enabled/markdown.conf
<Location>               
    AddHandler markdown .md                        
    DirectoryIndex index.md                     
    MarkdownCss ./style.css                 
    MarkdownHeaderFile /var/www/blog/header.html   
    MarkdownFooterFile /var/www/blog/footer.html                                                   
</Location>    
```
