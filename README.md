```javascript
import Pristine from '../node_modules/c3rpristinejs/src/pristine.js';

window.onload = function () {
    var form = document.getElementById("form");
    var pristine = new Pristine(form, {errorClass: 'invalid', successClass: 'valid'});

    form.addEventListener('submit', function (e) {
        e.preventDefault();
        if(pristine.validate()){
        //     $.ajax({
        //         url: 'app/lead.php',
        //         type: 'POST',
        //         data: $(this).serialize(),
        //
        //         success: function(data){
        //             if(data.status === 'success'){
        //                 $('.form-box').addClass('d-none');
        //                 $('.thx').removeClass('d-none');
        //
        //                 $('html, body').animate({
        //                     scrollTop: $(".thx").offset().top - 200
        //                 }, 1000);
        //             }else{
        //                 alert(data.message);
        //             }
        //         }
        //     });
        }
    });
};
```
