## AjaxFileUpload ##

This is a fork version of http://www.phpletter.com/Our-Projects/AjaxFileUpload/

### Improvement and Fix ###

1. Add arguments support   
    You can now use `data` to send addictional arguments, Example:

        $.ajaxFileUpload(
        {
            url: '/',
            secureuri: false,
            data: {                    
                'name': 'carlcarl',
            },
            ...
            ...
        }

2. Fix mimetype problem  
    If you add mimetype in your json response,
    it will add addictional tags '&lt;pre>&lt;/pre>' to your ajax response, which will cause error in original code.                   
    So I fix this.


