
#### 1. Visit our [base.html](https://github.com/sijanonly/angularjs-
handson/blob/master/base.html) file.

#### 2. Let us include following .css and .js files in our base file. NOTE : I
have used the   [CDN for bootstrap](https://www.bootstrapcdn.com/).



   1. `<link rel="stylesheet"
href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" int
egrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7"
crossorigin="anonymous"> `
   2. `<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.5/angula
r.min.js"></script> `



#### 3. Next we configure our web page to be an Angular application.
##### Include  ng-app angular directive to `<html>` tag. i.e ` <html lang="en"
ng-app>`


#### 4. Now, let us initialize data for our application with `ng-init` as follow :
'''
     <div class="row row-content"
          ng-init="
             star=
             {
               name:'Angelina Jolie',
               image: 'images/angelina.jpg',
               dob: 'June 4, 1975',
               description:'Born in Los Angeles, California, on June 4, 
               1975, Angelina Jolie starred in the HBO biopic Gia before 
               earning an Academy Award for best supporting actress for 
               Girl, Interrupted. Jolie has become one of Hollywood top 
               marquee names, having starred in movies like Wanted, Mr. and 
               Mrs. Smith, Salt and Changeling, earning her first lead 
               actress Oscar nod for the latter.'
            }">
'''

#### 5. Here we define a javascript array `star` with keys 'name', 'image',
'dob' and 'description'.


#### 6. Now, we can access the attributes with `{{star.name}}`, `{{star.image}}`
and so on as in following :
'''
    <div class="media">
        <div class="media-left media-middle">
            <a href="#">
            <img class="media-object img-rounded" width="60" height="90" 
             ng-src={{star.image}} alt="Angelina">
            </a>
        </div>
        <div class="media-body">
            <h2 class="media-heading">{{star.name}}
             <span class="label label-danger">superstar</span></h2>
                <blockquote>
                    <p>{{star.description}}</p>
                </blockquote>
                <blockquote>
                    <p>{{star.dob}}</p>
                </blockquote>
        </div>
    </div>
'''


    
