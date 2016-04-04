TinyMce(The rich text editor) With file/media manager and Custom Template.

Create a folder name tinymce(you sould rename it as your choice) in your plublic directory.
Copy these three folder(js/source/template) in your recently created folder and include tinymce link in your html page. 
```html
<script src="/tinymce/js/tinymce/tinymce.min.js"></script> // Directory started from public directory
```
Example initialization:

```php 
tinymce.init({
            selector: '#tiny_mce_etemplate',
            height: 500,
            theme: "modern",
            plugins: [
                "advlist autolink lists link image charmap print preview hr anchor pagebreak",
                "searchreplace wordcount visualblocks visualchars code fullscreen",
                "insertdatetime media nonbreaking save table contextmenu directionality",
                "emoticons template paste textcolor colorpicker textpattern imagetools filemanager"
            ],
            image_advtab: true,
            toolbar1: "insertfile undo redo | styleselect | bold italic | alignleft aligncenter alignright alignjustify | bullist numlist outdent indent | link image",
            toolbar2: "print preview media | forecolor backcolor emoticons template",
            
            content_css: [
                '//fast.fonts.net/cssapi/e6dc9b99-64fe-4292-ad98-6974f93cd2a2.css',
                '//www.tinymce.com/css/codepen.min.css'
            ],
            templates: [
                {title: 'Default Template 1', description: 'Attorney Media Marketing', url: '/tinymce/template/amn.htm'},
                {title: 'Default Template 2', description: 'High Converting Media', url: '/tinymce/template/hcm.htm'}
            ]
        });
```
