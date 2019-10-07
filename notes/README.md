## Notes on angular tutorial

### Anatomy of an angular component

```
import {Component, OnInit} from '@angular/core';
@Component({
    selector:'app-root',
    templateUrl:'./app.component.html',
    styleUrls:['./app.component.css']
})

export class AppComponent implements OnInit{
    name:string ='Brad';
    age:number=37;

    constructor(**services are imported here**){}
    ngOnInit(){
        //runs when component is created
    }
}
```

- Just like react and vue you have functionality, style and view
- you have properties in typescript

### Angular CLI

```
ng new myapp
ng serve
ng build
```

## State management

- With angular it it less necesarry to use Redux/rxjs
- Application level state can be used with ngrx
