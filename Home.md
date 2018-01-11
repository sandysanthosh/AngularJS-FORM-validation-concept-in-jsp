Welcome to the AngularJS-FORM-validation-concept-in-jsp wiki!


https://scotch.io/tutorials/submitting-ajax-forms-with-jquery

`<form name = "studentForm" novalidate>  `
`<table border = "0">  `
`<tr> ` 
`<div class="form-group">`
  `<label>Name</label>`
  `<input type="text" name="name" class="form-control" ng-model="name" required>`
  `<p ng-show="userForm.name.$invalid && !userForm.name.$pristine" class="help-block">You name is required.</p>`
`</div>`

`<!-- USERNAME -->`
`<div class="form-group">`
  `<label>Username</label>`
  `<input type="text" name="username" class="form-control" ng-model="user.username" ng-minlength="3" ng-maxlength="8">`
  `<p ng-show="userForm.username.$error.minlength" class="help-block">Username is too short.</p>`
  `<p ng-show="userForm.username.$error.maxlength" class="help-block">Username is too long.</p>`
`</div>`

`<!-- EMAIL -->`
`<div class="form-group">`
  `<label>Email</label>`
  `<input type="email" name="email" class="form-control" ng-model="email">`
  `<p ng-show="userForm.email.$invalid && !userForm.email.$pristine" class="help-block">Enter a valid email.</p>`
`</div>`
`</tr>`
`</table>`
`</form>`

`FORM VALIDATION ERROR CHECK:`

* .ng-valid       {  }
* .ng-invalid     {  }
* .ng-pristine    {  }
* .ng-dirty       {  }
* .ng-touched     {  }

* /* really specific css rules applied by angular */
* .ng-invalid-required        {  }
* .ng-invalid-minlength       {  }
* .ng-valid-max-length        {  }

