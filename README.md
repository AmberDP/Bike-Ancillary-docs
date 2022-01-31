# bike-ancillary

## Flow diagram
Start with our [flow diagram](https://drive.google.com/file/d/1tiLWoqP_GxfrIRk0ueaLKTCn-qOGUBZm/view?usp=sharing) to understand how you have to integrate our API 

## Backend documentation
We created a [postman API](https://documenter.getpostman.com/view/3410894/UVRBmkmm) collection that you can copy and play with.


## Auto-generated product page 
Product page can be a pain to integrate on your website as you need to create one product page per country and languages. That's why we developed the 3 ways to easily integrate a product page auto generate by Qover on your website [edit here in jsfiddle](https://jsfiddle.net/harryqover/bx5go9fq/latest)
### popup product page [edit here in jsfiddle](https://jsfiddle.net/harryqover/bx5go9fq/latest)
```html
<p>Keep your bike in tune, protect it against theft, and get help whenever and wherever you need it. <a onclick="showModalPopUp()">Learn more about our insurance.</a></p>
<script>
  var popUpObj;
function showModalPopUp() {
  popUpObj = window.open("https://bike.qoverme.com/widget/product-page?lang=en&key=pk_F2654BC3CEC684D9ED1E&brand=Venilu&depreciation=false&damageDeductible=DAMAGE_DEDUCTIBLE_STANDARD_10PC&theftDeductible=THEFT_DEDUCTIBLE_STANDARD_10PC&country=BE", "ModalPopUp", "width=400," + "height=900");
  popUpObj.focus();
  LoadModalDiv();
}
</script>
```


### redirection link
```html
<a href="https://bike.qoverme.com/widget/product-page?lang=en&key=pk_F2654BC3CEC684D9ED1E&depreciation=false&damageDeductible=DAMAGE_DEDUCTIBLE_STANDARD_10PC&theftDeductible=THEFT_DEDUCTIBLE_STANDARD_10PC&country=BE" target="_blank" class="cardLink">Insurance Belgium</a>
```
### iframe
```html
<iframe src="https://bike.qoverme.com/widget/product-page?lang=en&key=pk_F2654BC3CEC684D9ED1E&countryDefault=BE" title="description" width="400" height="800"></iframe>
```
