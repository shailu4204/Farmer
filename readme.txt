how to add bootstrap

npm install bootstrap --save
           

npm install jquery -- save

"styles": [
              "src/styles.css",
             
              "node_modules/bootstrap/dist/css/bootstrap.min.css"
          ],
 "scripts": [
              
              "node_modules/jquery/dist/jquery.min.js",
              "node_modules/bootstrap/dist/js/bootstrap.min.js"
              
            ]



<div class="form-group">

 
          <label>Username</label>
        <br>
            <input [class.is-invalid]="registrationForm.get('userName').invalid && 
    registrationForm.get('userName').touched" formControlName="userName" type="text" class="from-control" placeholder="Enter Username" size="40px">
   
      </div>
      <div *ngIf="registrationForm.get('userName').invalid && registrationForm.get('userName').touched">
        
        <small class="text-danger" *ngIf="registrationForm.get('userName').errors?.required">Username is
          required</small>
        <small class="text-danger" *ngIf="registrationForm.get('userName').errors?.minlength">Username must atleast be 3
          characters</small>
        
      </div>


