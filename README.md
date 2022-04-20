# Swift Submit JQuery Plugin

Version 3



## Initialization

```javascript

$("form").swiftSubmit(options,validationRules, onBeforeSend, onSuccess, onError, onComplete);

options must be a valid object and can have the following values-
var options = {
            format: "",   //default is "auto"
            form: "",
            action: "", //submit url
            method: "",  //default is "POST"
            redirect: boolean, //default is false
            redirectURL: "",
            resetForm: boolean, //default is true
        }

function validationRule() {
    if (something == wrong) {
        //show alert or perform any task
        return false; //must return false finally
    }
    
    if (anotherThing == wrong) {
        //show alert or perform any task
        return false; //must return false finally
    }

    //if all validations are fine, then must return true at the end.
    return true;
}
```

### Submit button configuration

Submit button can be input or button. But it must have type and class attribute as follows

```html
<!-- Both input or button must have the class .form-submit-button -->

<!--if input, then must have type="submit"--> 
<input type="submit" class="form-submit-button" value="Submit">

<!--if button, then must have type="button"--> 
<button type="button" class="form-submit-button">Submit</button>
```

