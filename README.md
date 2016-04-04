TinyMce With file manager and Custom Teplate


Here is the example initialization for tinyMce

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
